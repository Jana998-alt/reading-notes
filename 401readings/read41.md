# React IV

## Dynamic Routes

dynamic routing is needed when there are many instances that hold the same type of information, but with different values. for example: users profiles. to dynamically generate react components for any profile using the same template, we use dynamic routing.
there are 2 extra items that should be added to the component.js file, other than the main rendering function: a function that returns all the possible different values, and a function to fetch data for the selected value.

## Implement getStaticPaths

**let’s set up the files:**

* Create a file called [id].js inside the pages/posts directory.
* Also, remove first-post.js inside the pages/posts directory — we’ll no longer use this.

***The returned list is not just an array of strings — it must be an array of objects. Each object must have the params key and contain an object with the id key (because we’re using [id] in the file name). Otherwise, getStaticPaths will fail.***

## Implement getStaticProps

**It will return the post data based on id:**

    export function getPostData(id) {
    const fullPath = path.join(postsDirectory, `${id}.md`)
    const fileContents = fs.readFileSync(fullPath, 'utf8')

    // Use gray-matter to parse the post metadata section
    const matterResult = matter(fileContents)

    // Combine the data with the id
    return {
        id,
        ...matterResult.data
    }
    }

**open pages/posts/[id].js and replace this line:**

    import { getAllPostIds } from '../../lib/posts'

**with the following code:**

    import { getAllPostIds, getPostData } from '../../lib/posts'

    export async function getStaticProps({ params }) {
    const postData = getPostData(params.id)
    return {
        props: {
        postData
        }
    }
    }

**let's update the Post component to use postData. In pages/posts/[id].js replace the exported Post component with the following code:**

    export default function Post({ postData }) {
    return (
        <Layout>
        {postData.title}
        <br />
        {postData.id}
        <br />
        {postData.date}
        </Layout>
    )
    }

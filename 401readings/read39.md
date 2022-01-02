# React III
## NextJs

Next.jsis a React Framework that provides a solution to the problems below that you face when building using only react.

- Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
- You need to do production optimizations such as code splitting.
- You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
- You might have to write some server-side code to connect your React app to your data store.


### Assets

Next.js can serve static assets, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.

### Metadata
you can modify the metadata of the page, such as the <title> HTML tag.

### CSS Styling
Next.js has built-in support for styled-jsx, but you can also use other popular CSS-in-JS libraries such as styled-components or emotion.

Writing and Importing CSS
Next.js has built-in support for CSS and Sass which allows you to import .css and .scss files.

Using popular CSS libraries like Tailwind CSS is also supported.

Global Styles
CSS Modules are useful for component-level styles.
  
  
## React Context for Beginners

 react context is the way that allows for react components to share data between them, which also helps us avoid the problem of props drilling(which is when you pass props down multiple levels to a nested component, through components that don't need it.).
  
There are four steps to using React context:

1. Create context using the createContext method.
2. Take your created context and wrap the context provider around your component tree.
3. Put any value you like on your context provider using the value prop.
4. Read that value within any component by using the context consumer.

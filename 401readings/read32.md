# Permissions & Postgresql

## DRF Permissions

The security of a webpage is done through 2 steps: authentication and authorization. 

there is view level permissions, and object-level permissions.

- these run before the code of the view in django. 
Permissions in REST framework are always defined as a list of permission classes: IsAuthenticated, request.user and request.auth. 

- Object level permissions are used to determine if a user should be allowed to act on a particular object.

for example :

```
def get_object(self):
    obj = get_object_or_404(self.get_queryset(), pk=self.kwargs["pk"])
    self.check_object_permissions(self.request, obj)
    return obj

```

### setting the permission policy: 
The default permission policy is set globally, using the DEFAULT_PERMISSION_CLASSES setting: 

``` 
REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}
```

an example of a permission class: 

```
from rest_framework import permissions

class BlocklistPermission(permissions.BasePermission):
    """
    Global permission check for blocked IPs.
    """

    def has_permission(self, request, view):
        ip_addr = request.META['REMOTE_ADDR']
        blocked = Blocklist.objects.filter(ip_addr=ip_addr).exists()
        return not blocked
```

REST framework has three different methods to customize access restrictions on a case-by-case basis:

- queryset/get_queryset()
- permission_classes/get_permissions():
- serializer_class/get_serializer()
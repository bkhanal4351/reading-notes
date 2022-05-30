# Permissions & Postgresql

# Permissions
Authentication or identification by itself is not usually sufficient to gain access to information or code. For that, the entity requesting access must have authorization.

How permissions are determined
  - Permissions in REST framework are always defined as a list of permission classes.

Before running the main body of the view each permission in the list is checked. If any permission check fails, an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.

When the permission checks fail, either a "403 Forbidden" or a "401 Unauthorized" response will be returned, according to the following rules:

  - The request was successfully authenticated, but permission was denied. — An HTTP 403 Forbidden response will be returned.
  - The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers. — An HTTP 403 Forbidden response will be returned.
  - The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers. — An HTTP 401 Unauthorized response, with an appropriate WWW-Authenticate header will be returned.

  Object level permissions
    - REST framework permissions also support object-level permissioning. Object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.

  Setting the permission policy
  - The default permission policy may be set globally, using the DEFAULT_PERMISSION_CLASSES setting. 

# API Reference

AllowAny
  - The AllowAny permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.

IsAuthenticated
  - The IsAuthenticated permission class will deny permission to any unauthenticated user, and allow permission otherwise.

IsAdminUser
  - The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.

IsAuthenticatedOrReadOnly
  - The IsAuthenticatedOrReadOnly will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.

Notes taken from (https://www.django-rest-framework.org/api-guide/permissions/)

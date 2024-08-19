## interface UserGroup
The UserGroup interface defines one method that can be implemented to controll access based on the roles of different users. A class that extends the `UserGroup` interface can also define other methods to check for different groups of users in the system.

The interface can be imported as follows:

```typescript

import  { UserGroup } from 'zero/user-group'

```

*NPM Dependencies*
* `None`

### 1. `isAdmin()`

Parameters:
* `user`: `ZeroUser` - An object that extends the [`ZeroUser`](./zero-user.md) interface.

Returns:
* `boolean`
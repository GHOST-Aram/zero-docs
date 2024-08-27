## interface `RouterConfig`

The `RouterConfig` interface defines objects and constructors that are required for routing configuring in a system. 

The interface can be imported as follows:

```typescript

import { RouterConfig } from 'zero/zero/types'

```

The following objects are defined in the `RouterConfig` interface:

* `applicationName`: `string` -  the name of the component being congfigured.

* `connectionPool`: `ConnectionPool` - an object of the [ConnectionPool](../db/connection.-pool.md) class

* `dBName`: `string` - The database name of the specific in the system 

* `dataSchema`: `Schema`<any>, - model schema of the component data.

* `DataAccess`: `DataAccessConstructor`<DataAccess>, -  The constructor of the component's data access class

* `Controller`: `ControllerConstructor`<Controller>, - the constructor of the component's controller class

* `GhostRouter`: `GhostRouterConstructor`<GhostRouter> - the constructor of the component's routing class. The routing class that extends the [`GhostRouter`](../routing/router.md) class

* `authenticator`: `Authenticator` - an instance of the [`Authenticator`](../auth/auth.md) class

* `modelName`: `string` - the name of the component's data model

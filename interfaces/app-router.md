## interface `AppRouter`

The `AppRouter` interface defines fields and a method that can be implemented by the Routing class an app.

The `AppRouter` interface can be imported as follows

```javascript

import { AppRouter } from 'zero/routing'
```

*NPM Dependencies*
* `express`

The `AppRouter` interface defines the following fields and methods:

* `router`: `Router` -  Express `Router` object
* `controller`: `Controller` - A class that extends the [`Controllable`](../bases/controllable.md) interface

* `authenticator`: `Authenticator` - An object of the [`Authenticator`](../auth/auth.md) class
* `registerRoutes`: ()=> `Router` 
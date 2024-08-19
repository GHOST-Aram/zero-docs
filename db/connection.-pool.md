## class `ConnectionPool`

The `ConnectionPool` pool class creates and manages a mongoose [connection pool](https://mongoosejs.com/docs/connections.html). The class provides methods for getting the intial connection and swtiching between different databases in the same cluster.

The class can be imported as follows:
```typescript

import { ConnectionPool } 'zero/db'
import ConnectionPool from 'zero/db/connection'

```

*NPM Dependencies*
* `mongoose`

The `ConnectionPool` class implements a constructor with one parameter described below

* `initialDbUri`: `string` -  Mongodb connection string

The class implements the following methods:

### 1. `getInitialConnection()`

Parameters:
* None

Returns:

* `Connection`: [`mongoose.Connection](https://mongoosejs.com/docs/api/connection.html#Connection())

### 2. `switchConnection()`

Parameters:
* `newdBName`: `string` - the name of the database in the to be connected to in the same cluster as the initial database.

Returns:

* `Connection`: [`mongoose.Connection](https://mongoosejs.com/docs/api/connection.html#Connection())
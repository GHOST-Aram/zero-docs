## class `DB`

The `DB` class encapsulate methods for performing operations related to database configurations. The class implements a constructor method with one parameter described below:

Constructor Parameters:
* `connection`: `Connection`  -  A `mongoose.Connection` object.

The class can be imported as shown in the code snippet below:

```typescript

import { DB } from 'zeo/db'
```

*NPM Dependencies*
* `mongoose`

The class implements the following method:

### 1. `createModel()`

Parameters:
* `modelName`:`string`, - The name of the data model
* `schema`: `Schema<any>` - an object of type `mongoose.Schema`

Returns:
* `mongoose.Model<any>`


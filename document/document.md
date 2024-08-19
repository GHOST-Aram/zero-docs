## class `Document`

The `Document` class encapsulates methods that are used to evaluate data documents fetched from the Database. 

This class does not implement a constructor.

The class and the instance of the `Document` class can be imported as follows:

```typescript

import { Document } from 'zero/document'
import { document } from 'zero/document'

```

*NPM Dependencies*
* `mongoose`

The class implements the following methods:

### 1. `exists()`

Parameters:
* `doc`: `HydratedDocument<any>` | `null` -  mongoose [`HydratedDocument`](https://mongoosejs.com/docs/typescript.html) type or null if the document is null.

Returns:
* `boolean`

### 2. `isOwnedByCurrentUser()`

Parameters:
* `creatorId`: `string` -  the ID of the user that created the document.
* `currentUserId`: `string` - the ID of the user that is currently in session and is inquiring about this document.

Returns:
* `boolean`
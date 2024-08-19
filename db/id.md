## the `ID` module
The `ID` module implements a function that can be used to create an `ObjectId` from a hexadecimal string.

Them method can be imported as follows:

```typescript
import { createObjectId } from 'zero/db'
```

*NPM Dependencies*
* `mongoose`

The following is the description of the function signature:

### 1. `createObjectId()`

Parameters:
* `hexId`: `string` -  a 24 character hexadecimal ID

Returns:
* `mongoose.Types.ObjectId`
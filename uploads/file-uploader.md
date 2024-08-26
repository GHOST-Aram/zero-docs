## class `FileUploader`
The `FileUploader` class encapsulates utility methods that assist in managing uploaded file in requests. 

The class and its instance can be imported as follows:

```typescript

import { FileUploader } from 'zero/uploads/ulpoad'
import fileUploader from 'zero/uploads/upload'

```

*NPM Dependencies*
* multer

The following methods are implemented in the `FileUploader` class:

### 1. `uploadSingleFile()`

Parameters:
* `name`: `string` -  name of the file to be uploaded as labeled in the input data.

Returns:
* Express Request handler

### 2. `uploadMultipleFiles()`

Parameters:
* `listName`: `string` -  the name of the array of files as labeled in the input data.

Returns:
* Express Request handler
git 
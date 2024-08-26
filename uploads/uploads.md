### the `uploads` module

The `uploads` module exports are used to handle file uploads. The module exports a class, an instance of a class and a function. The module exports cam be imported as follows:

```typescript

import { fileUploader } from 'zero/uploads'
import { FileUploader } from 'zero/ulpoads'
import { createFileBuffer } from 'zero/uploads'

```

*NPM Dependencies*
* multer

The exports from this module are documented as follows:

* [`FileUploader`](./file-uploader.md) class
* Function [`createFileBuffer`](./create-file-buffer.md)
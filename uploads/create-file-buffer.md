## function `createFileBuffer`

The function `createFileBuffer` is used to create an object that is used to store file data in the database. The function is singularly exported from its file and can be imported as follows:

```typescript
import { createFileBuffer } from  'zero/uploads'
import createFileBuffer from 'zero/uploads/file-buffer'
```

*NPM Dependencies*
* multer
* express

Parameters:
* `file`:`Express.Multer.File` - uploaded file from request.

Returns:
An Object literal containing the following properties.
* `name`: `string`,
* `data`: `Buffer`,
* `contentType`: `string`

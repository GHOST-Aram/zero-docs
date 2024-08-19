## interface `RequestData`
The `RequestData` interface defines the properties of an object that contains all the data provided by a user in the requst object.

The interface can be imported as follows:

```typescript

import { RequestData } from 'zero/request/types'

```

*NPM Dependencies* 
* `express`
* `@types/express`
* `multer`


The `RequestData` interface defines the following properties

* `referenceId`: `string`
* `reqBody`: `any` 
* `user`:`any`
* `currentUserId`: `string`
* `file`: `Express.Multer.File`
* `files`: `Express.Multer.File`[]
* `query`: `any`

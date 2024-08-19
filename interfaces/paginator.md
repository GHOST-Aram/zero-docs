## interface `Paginator`

The Paginator interface defines the properties of an object that specifies the number documents should be returned during a data fetching operation.

The interface can be imported as follows:

```typescript

import  { Paginator } from 'zero/http/types'

```

*NPM Dependencies*
* None

An object of the paginator interface includes the following properties:

* `skipDocs`: `number`- the number of documents to be skipped in a collection during a search query.

* `limit`: `number` -  the number of documents to be returned by a search query.


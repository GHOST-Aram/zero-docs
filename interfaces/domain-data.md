## interface DomainData

The DomainData interface defines methods that are used to process input data in every app in the system. The methods work on the data received from request body. 

The interface can be imported as follows:

```typescript

import  { DomainData } from 'zero/domain-data'

```

*NPM Dependencies*
* None

The following methods are defined in the DomainData interface.


* `aggregateInputDocument :(reqData: RequestData) => {}`
* `createUniqueSearchDocument: (inputData: any) => {}`

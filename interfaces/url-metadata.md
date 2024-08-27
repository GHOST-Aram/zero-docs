## interface `URLMetadata`

The `URLMetadata` interface defines properties of an object used to configure urls of components in a system entry point.

The interface can be imported as follows:

```typescript

import { URLMetadata } from 'zero/zero/types'

```

The interface defines the following properties:
* `path`: `string` - the path to a component in the system 
* `router`: `Router` -  The router object of the component that is accessible through the above path. 
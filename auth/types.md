## type `tokenPayloadCreator`

The type `tokenPayloadCreator` defines the signature to the function that created token payload for JWT token. The method has one parameter and returns a [`TokenPayload`](../interfaces/token-payload.md). 

The type can be imported as follows:

```typescript

import { tokenPayloadCreator } from 'zero/auth/types'

```

*NPM Dependencies*
* None

The type is defined as follows:

`type tokenPayloadCreator = (user: any) => TokenPayload`


## the `testing` module

The testing module exports objects for configuring, setting up and running tests on HHTP responses. 

The exports from the `testing` module can be imported as follows:

```typescript

import { app } from 'zero/testing'
import { Authenticator } from 'zero/testing'
import { user } from 'zero/testing'
import { MockDataAccess } from 'zero/testing'
import { assert } from 'zero/testing'

```

- The `app` exported from the `testing` module is an `Express.Application` object

- The `Authenticator` is a mock for the [Authenticator](../auth/auth.md) class
- The `user` is a mock for an object of the [`TokenPayload`](../interfaces/token-payload.md) interface
- `MockDataAccess` is the mock for [`GenericDataAccess`](../bases/generic-data-access.md) class
- `assert` is an instance of the [`ResponseAssertion`](./response-assetion.md) class
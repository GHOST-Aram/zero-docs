## interface `Controllable`
The Controllable interface defines the required methods that every Controller class in the system must implement. The methods in the Controllable interface follow the [`Express` Route handler method](https://expressjs.com/en/guide/routing.html) signatures. All methods in this interface are asynchronous. 

### 1. `addNew()`
Parameters:
* `domainData`: `DomainData` - An object of the [DomainData](../interfaces/domain-data.ts) interface.

Returns:
* `(req: Request, res: Response, next: NextFunction)` => `Promise<void>` - an asynchronous Express Route handler method.

### 2. `getOne()`

Paramters:

* `req`: `Request` - Express Request object
* `res`: `Response` - Express Response object 
* `next`: `NextFunction` - Express Next function.

Returns:

* `Promise<void>`

### 3. `getMany()`

Parameters:
* `searchablePaths`: `string`[] -  Array of keys in the data schema that can be used to search for documents in the app's db collection.

Returns:
* `(req: Request, res: Response, next: NextFunction)` => `Promise<void>` -  Express route handler method

### 4. `updateOne()`

Parameters:
* `domainData`: `DomainData` -  An instance of a class that implements the [`DomainData`](../interfaces/domain-data.md) interface.
* `userGroup`: `UserGroup` - An object that extends the [`UserGroup`](../interfaces/user-group.md) interface

Returns:
* ` (req: Request, res: Response, next: NextFunction)` => `Promise<void>` -  An asynchronous Express Route handler method.


### 5. `modifyOne()`:

Parameters:

* `domainData`: `DomainData` -  An instance of a class that implements the [`DomainData`](../interfaces/domain-data.md) interface.
* `userGroup`: `UserGroup` - An object that extends the [`UserGroup`](../interfaces/user-group.md) interface

Returns:
* ` (req: Request, res: Response, next: NextFunction)` => `Promise<void>` -  An asynchronous Express Route handler method.

### 6. `deleteOne()`

Parameters
* `userGroup`: `UserGroup` - An object that extends the [`UserGroup`](../interfaces/user-group.md) interface

Returns:
* ` (req: Request, res: Response, next: NextFunction)` => `Promise<void>` -  An asynchronous Express Route handler method.
## class `GenericController`
The `GenericController` class implements the [`Controllable`](./controllable.md) interface and extends the [`HttpResponse`](../http/http-response.md) class. The class accepts a generic type `T` that extends or implements the [`Accessible`](./accessible.md) interface.

The `GenericController` class methods are used to process requests and send responses. The class implements a `constructor` method with two parameters. 

**Constructor Parameters**

* `dataAccess`: `T`- an instance of a class that implements the [`Accessible`](./accessible.md) interface. 
* `microserviceName`: `T` - is the paramter of the super class constructor, i.e [`HttpResponse`](../http/http-response.md).

The `GenericController` class implement all the methods in the [`Controllable`](../bases/accessible.md) interface and other methods listed below:

### 1. `async createAndRespond()`

Parameters:
* `document`: `any` -  an object containing input data for creating new documents
* `res`: `Response` - An Object of the Express Response interface.

Returns:
* `void`

### 3. `async updateAndRespond()`

Paramters:
* `updateData`: `UpdateData` -  An object of the [`UpdateData`](../interfaces/update-data.md) interface

Returns:
* `void`

### 4. `async deleteAndRespond()`

Parameters:
* `referenceId`: `string`
* `res`: `Response`

Returns:
* `void`

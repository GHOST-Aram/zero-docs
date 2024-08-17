## interface `Accessible`

The Accessible interface defines the required methods that every data access class in the system must implement. All methods in this interface are asynchronous.  

The interface describes the following methods:

### 1.  `createNew()`

Paramters:
* `data`: `any` - a object for creating a new document in the DB

Returns: 
* `Promise<HydratedDocument<any>>`

### 2. `findByReferenceId()`

Parameters:
* `refId`: `string`

Returns:
* `Promise<HydratedDocument<any> | null>`

### 3. `findBySearchDocument()`

Parameters:

* `searchDoc`: `any`
* `paginator`: [`Paginator`](../interfaces/paginator.md)

Returns:
* `Promise<HydratedDocument<any>[]>`

### 4. `findExistingDocument()`

Parameters:

* `searchDoc`: `any` - an object containing properties and values used to search for documents within a collection.

Returns:
* `Promise<HydratedDocument<any>>`

### 5. `findWithPagination()`

Parameters:
* `paginator`: [`Paginator`](../interfaces/paginator.md)

Returns:
* `Promise<HydratedDocument<any>[]>`

### 6. `findByIdAndUpdate()`

Parameters:

* `id`: `string`, 
* `updateDoc`: `any` -  an object containing properties and values for the update operation

Returns: 
* `Promise<HydratedDocument<any> | null>`

### 7. `findByIdAndDelete()`

Parameters:

* `id`: `string`

Returns:
* `Promise<HydratedDocument<any> | null>`

### 8. `findByCreatorId()`

Parameters:

* `creatorId`: `string` -  ID of the user that created the documents being searched
* `paginator` : [`Paginator`](../interfaces/paginator.md)

Returns:
* `Promise<HydratedDocument<any>[]>`
## class `GenericDataAccess`
The `GenericDataAccess` class implements the [`Accessible`](./accessible.md) interface. This class is used as a data access layer in apps that require database access and operations. 

The `GenericDataAccess` class takes two generic type parameters listed below:

* `T extends Model<any>` -  Any type that extends the type [`mongoose.Model`](https://mongoosejs.com/docs/api/model.html).
* `RawData` -  A JavaScript object interface that defines the properties of a model schema.

The class implements a `constructor` method with one parameter:
* `model`: `T` -  a data model

The `GenericDataAccess` class implements all the methods in the [`Accessible`](./accessible.md) interface.
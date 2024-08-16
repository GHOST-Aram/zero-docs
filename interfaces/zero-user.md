## `interface ZeroUser`

An interface that defines the properties that must exist in a user object of an application that is build on the Zero library. 

The ZeroUser interface includes the following properties:

```typescript

profilePicture?: {
    name: string,
    data: Buffer,
    contentType: string
}
pictureUrl?: string
fullName: string
userGroup: string
email: string
password: string
_id?: string

```
## `interface TokenPayload`
This interface defines the structure of the object that contains user data that will be included in the signed JWT. 

The `TokenPayload` interface includes the following properties:

```typescript

fullName: string,
email: string,
username?: string,
id: string,
userGroup: string
```
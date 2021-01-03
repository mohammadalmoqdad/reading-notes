1. Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
- user, photographer, photo
- the user may get more than one photo
- the user may have a photo session with more than one user
- photographer may make a photo session for more than one user
- more than on photo can be taken by the photographer
- more than one photo the user can get



2. 2. What is the advantage of an ORM, like Mongoose?
- Its static nature means it does not require refreshing. It is easy to test. ROM is more reliable than RAM since it is non-volatile in nature and cannot be altered or accidentally changed.

3. How does the repository pattern compare with an ORM?
- Repositories deal with Domain/Business objects (from the app point of view), an ORM handles db objects. A business objects IS NOT a db object, first has behaviour, the second is a glorified DTO, it only holds data. ... You can also check this post about more details about the repository pattern.

4. Name 3 cloud based NoSQL Databases: 
1. Couchbase.
2. Amazon DynamoDB.
3. MongoDB.


 * phases are the stages a computer program undergoes, from initial creation to deployment and execution. The phases are edit time, compile time, link time, distribution time, installation time, load time, and run time.

 * A **collection** — sometimes called a container — is simply an object that groups multiple elements into a single unit. ... If you've used the Java programming language — or just about any other programming language — you're already familiar with collections.

 *  Repository pattern is a kind of container where data access logic is stored

 * **mongoose midleware** are functions which are passed control during execution of asynchronous functions. Middleware is specified on the schema level and is useful for writing plugins.

 * **ORM** a programming technique for converting data between incompatible type systems using object-oriented programming languages


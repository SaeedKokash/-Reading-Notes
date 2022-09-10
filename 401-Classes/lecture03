# Readings: SQL database, ORM, Sequelize #

## What's the difference between SQL and NoSQL? ##
| SQL | noSQL |
| ----------- | ----------- |
| Data use Schemas | Schema-less |
| Relations | No/Few Relations |
| Data is distributed acroos multiple tables | Data is typically merged / nested in a few collections |
| Horizontal scaling is difficult/impossible; Vertical scalling is possible | Both horizontal and vertical scaling is possible |
| Limitaitons for lots of (thousands) read & write queries per second | Great performace for mass (simple) read & write requests |


## What is Sequlize and how to use it with Node js? ##
Sequelize is a Node.js-based Object Relational Mapper that makes it easy to work with MySQL, MariaDB, SQLite, PostgreSQL databases, and more. An Object Relational Mapper performs functions like handling database records by representing the data as objects.

### INSTALL DEPENDENCIES ###
```
npm install sequelize sqlite3
# or
yarn add sequelize sqlite3
```

### DEFINE MODELS ###
```
import { Sequelize, Model, DataTypes } from 'sequelize';

const sequelize = new Sequelize('sqlite::memory:');
const User = sequelize.define('User', {
  username: DataTypes.STRING,
  birthday: DataTypes.DATE,
});
```

### PERSIST AND QUERY ###
```
const jane = await User.create({
  username: 'janedoe',
  birthday: new Date(1980, 6, 20),
});

const users = await User.findAll();
```

### Quick Example ###
```
const { Sequelize, Model, DataTypes } = require('sequelize');
const sequelize = new Sequelize('sqlite::memory:');

class User extends Model {}
User.init({
  username: DataTypes.STRING,
  birthday: DataTypes.DATE
}, { sequelize, modelName: 'user' });

(async () => {
  await sequelize.sync();
  const jane = await User.create({
    username: 'janedoe',
    birthday: new Date(1980, 6, 20)
  });
  console.log(jane.toJSON());
})();
```

## What is an ORM, how does it work, and how should I use one? ##
Object-Relational Mapping (ORM) is a technique that lets you query and manipulate data from a database using an object-oriented paradigm. When talking about ORM, most people are referring to a library that implements the Object-Relational Mapping technique, hence the phrase "an ORM".

An ORM library is a completely ordinary library written in your language of choice that encapsulates the code needed to manipulate the data, so you don't use SQL anymore; you interact directly with an object in the same language you're using.

For **example** , here is a completely imaginary case with a pseudo language:

You have a book class, you want to retrieve all the books of which the author is "Linus". Manually, you would do something like that:
```
book_list = new List();
sql = "SELECT book FROM library WHERE author = 'Linus'";
data = query(sql); // I over simplify ...
while (row = data.next())
{
     book = new Book();
     book.setAuthor(row.get('author');
     book_list.add(book);
}
```

With an ORM library, it would look like this:

```
book_list = BookTable.query(author="Linus");
```

The mechanical part is taken care of automatically via the ORM library.

### Pros and Cons ###

**Using ORM saves a lot of time because**

- DRY: You write your data model in only one place, and it's easier to update, maintain, and reuse the code.
- A lot of stuff is done automatically, from database handling to I18N.
- It forces you to write MVC code, which, in the end, makes your code a little cleaner.
- You don't have to write poorly-formed SQL (most Web programmers really suck at it, because SQL is treated like a "sub" language, when in reality it's a very powerful and complex one).
- Sanitizing; using prepared statements or transactions are as easy as calling a method.

**Using an ORM library is more flexible because**

- It fits in your natural way of coding (it's your language!).
- It abstracts the DB system, so you can change it whenever you want.
- The model is weakly bound to the rest of the application, so you can change it or use it anywhere else.
- It lets you use OOP goodness like data inheritance without a headache.

**But ORM can be a pain**

- You have to learn it, and ORM libraries are not lightweight tools;
- You have to set it up. Same problem.
- Performance is OK for usual queries, but a SQL master will always do better with his own SQL for big projects.
- It abstracts the DB. While it's OK if you know what's happening behind the scene, it's a trap for new programmers that can write very greedy statements, like a heavy hit in a for loop.

### *[Source](https://stackoverflow.com/questions/1279613/what-is-an-orm-how-does-it-work-and-how-should-i-use-one#:~:text=An%20ORM%20library%20is%20a,same%20language%20you're%20using.)*  ###

<hr>
<hr>

## Preparation Materials ## 
- [SQL database](https://www.techtarget.com/searchdatamanagement/definition/SQL)
- [Sequelize](https://sequelize.org/)
- [ORM](https://www.techopedia.com/definition/24200/object-relational-mapping--orm)
- [CRUD system](https://zellwk.com/blog/crud-express-mongodb/)

# BookLibrary
This is a simple Spring application with an API for adding and storing information about books.
## ✨ Features
- Adding a new book.
- Getting information about a book by id.
- Getting information about all books.

## 🛠️ Technologies
- Java
- Spring Boot
- MySQL

## 🔑 API Specification
### Methods
The application has several methods which are given below:
| Method    | URL                           | Description                                         |
| --------- | ----------------------------- | --------------------------------------------------- |
| `GET`     | `/books/`                     | Returns list of books.    |
| `POST`    | `/books/`                     | Creates a new book.       |
| `GET`     | `/books/{id}`                 | Returns a book by id      |
#### `GET` /books/
Example of a response:
```
{[
    {
        'id': 1,
        'name': "Spring in Action",
        'year': 2005
    }, 
    ...
]}
```
#### `POST` /books/
Input parameters:
| Type      | Name      | Nullable | Description         | Example           |
| --------- | --------- | -------- | ------------------- | ----------------- |
| `String`  | `name`    | `true`   | Book name              | Spring in Action                 |
| `Integer` | `year`    | `true`   | Year of book release   | 2005         |


Example of successful response:
```
{
    'id': 1
}
```

#### `GET` /books/{id}
Input parameters:
| Type      | Name      | Nullable | Description         | Example           |
| --------- | --------- | -------- | ------------------- | ----------------- |
| `Integer` | `id`      | `false`  | Book Id             | 1                 |

Example of successful response:
```
{
    'id': 1,
    'name': "Spring in Action",
    'year': 2005
}
```

## Author
### 👤 **Denis Bezrukov**
- Email: [ds.bezrukov@icloud.com](mailto:ds.bezrukov@icloud.com)
- Telegram: [@x_bezrukov_x](https://t.me/x_bezrukov_x)
- Github: [@xbezrukovx](https://github.com/xbezrukovx)

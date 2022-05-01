# graphql-tmp

## What is this?
A simple GraphQL API to GET and POST books and authors data.

## How to run
    
    npm i && npm run devStart

## How to use

### 1. Return list of all books


    query {
        books {
            id,
            authorid,
            name
        }
    }

### 2. Return list of all authors

    
        query {
            authors {
                id,
                name
            }
        }

### 3. Return certain book

    
        query {
            book(id: 1) {
                id,
                authorid,
                name
            }
        }

### 4. Return certain author


        query {
            author(id: 1) {
                id,
                name
            }
        }

### 5. Add certain book


        mutation {
            addBook(name: "New book", authorid: 1) {
                id,
                name
            }
        }

### 6. Add certain author

    
            mutation {
                addAuthor(name: "New author") {
                    id,
                    name
                }
            }

To learn more about how to use GraphQL, please visit [GraphQL Documentation](https://graphql.org/learn/queries/).

## Credits
Allief Nuriman
#这是一个 spring-boot-graphql simple demo

基于:

- spring-boot 2.0.0
- graphql-spring-boot-starter 4.0.0
- graphql-java-tools 4.3.0

run server:
    
    ./run.sh

graphql default endpoint: /graphql

    http://127.0.0.1:10001/graphql
    
exmple:
    
    request:
    
    {
      findAllBooks {
        id
        title
      }
    }
       
    response:
    
    {
      "data": {
        "findAllBooks": [
          {
            "id": 1,
            "title": "SUN"
          },
          {
            "id": 2,
            "title": "SUN1"
          },
          {
            "id": 3,
            "title": "SUN3"
          },
          {
            "id": 4,
            "title": "java"
          }
        ]
      }
    }

graphql 图形工具ui:<br>
    [An in-browser IDE for exploring GraphQL](https://github.com/graphql/graphiql)<br>
    [An App GraphQL](https://github.com/skevy/graphiql-app)

git commit -m "first commit"
git remote add origin git@gitee.com:geng_hz/spring-boot-graphql.git
git push -u origin master
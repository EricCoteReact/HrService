# hrservice

[![LoopBack](https://github.com/strongloop/loopback-next/raw/master/docs/site/imgs/branding/Powered-by-LoopBack-Badge-(blue)-@2x.png)](http://loopback.io/)



npm install -g @loopback/cli

lb4 app hrsvc

cd hrsvc

lb4 model
? Model class name: employee
? Please select the model base class: Entity
? Allow additional (free-form) properties? No


id (number, id prop, required)
firstName (string, required)
lastName  (string, not required)

lb4 datasource
? Datasource name: db
? Select the connector for db: In-memory db (supported by StrongLoop)
? window.localStorage key to use for persistence (browser only):
? Full path to file for persistence (server only): ./data/db.json

------create empty file:  ./data/db.json  

lb4 repository
? Please select the datasource DbDatasource
? Select the model(s) you want to generate a repository Employee
? Please select the repository base class
> DefaultCrudRepository





lb4 controller
? Controller class name: employee
? What kind of controller would you like to generate? REST Controller with CRUD functions
? What is the name of the model to use with this CRUD repository? Employee
? What is the name of your CRUD repository? EmployeeRepository
? What is the type of your ID? number
? What is the base HTTP path name of the CRUD operations? /employees

Change port from 3000 to 3001 in index.js
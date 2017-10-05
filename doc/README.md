## tDBResultsToJSON

+ Version 1.0 

Converts a database result set to a generic JSON string

---

### Overiew of job flow

![Alt text](job_overview.png?raw=true "Job - Flow Diagram")

### Setting up the datbaase components

1. Use a DBConnection component
2. The schema will include one column of type Object which is set to pass the ResultSet to the next component

![Alt text](tmysqlrow_01.png?raw=true "tMysqlRow - Schema")

![Alt text](tmysqlrow_02.png?raw=true "tMysqlRow - Advanced settings")

### Passing the database conneciton object

3. Pass the DB connection object by calling a global get

![Alt text](tmap_01.png?raw=true "tMap - Passing the Connection Object")

### Configuring the features of the tDBResultsToJSON component

4. Define if the DATA, STRUCTURE, or BOTH should be inlcuded in the JSON
5. Define how to handle NULL values

![Alt text](tdbresultstojson_01.png?raw=true "tDBResultsToJSON - Basic settings")

6. Change the advanced setting when including STRUCTURE based on the type of database platform

![Alt text](tdbresultstojson_02.png?raw=true "tDBResultsToJSON - Advanced settings")

### JSON produced from SQL query

![Alt text](job_run_01.png?raw=true "Job - Run console")

![Alt text](job_run_02.png?raw=true "Job - Run JSON")

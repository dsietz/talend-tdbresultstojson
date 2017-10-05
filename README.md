[![License](https://img.shields.io/aur/license/yaourt.svg)](https://opensource.org/licenses/gpl-license)

## tDBResultsToJSON

+ Version 1.0 

Converts a database result set to a generic JSON string

---

### Overiew of job flow

![Alt text](/doc/job_overview.png?raw=true "Job - Flow Diagram")

### Setting up the datbaase components

1. Use a DBConnection component
2. The schema will include one column of type Object which is set to pass the ResultSet to the next component

![Alt text](/doc/tmysqlrow_01.png?raw=true "tMysqlRow - Schema")

![Alt text](/doc/tmysqlrow_02.png?raw=true "tMysqlRow - Advanced settings")

### Passing the database conneciton object

3. Pass the DB connection object by calling a global get

![Alt text](/doc/tmap_01.png?raw=true "tMap - Passing the Connection Object")

### Configuring the features of the tDBResultsToJSON component

4. Define if the DATA, STRUCTURE, or BOTH should be inlcuded in the JSON
5. Define how to handle NULL values

![Alt text](/doc/tdbresultstojson_01.png?raw=true "tDBResultsToJSON - Basic settings")

6. Change the advanced setting when including STRUCTURE based on the type of database platform

![Alt text](/doc/tdbresultstojson_02.png?raw=true "tDBResultsToJSON - Advanced settings")

### JSON produced from SQL query

![Alt text](/doc/job_run_01.png?raw=true "Job - Run console")

![Alt text](/doc/job_run_02.png?raw=true "Job - Run JSON")

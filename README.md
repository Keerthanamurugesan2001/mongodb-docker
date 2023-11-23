# mongodb

Mongo Express is added to access use [localhost:8081](http://localhost:8081/)

username: `admin`
password: `pass`

**STEP 1**
Clone the Project using this command
```
git clone <URL>
```

**STEP 2**
Run the docker compose file in `detach` mode
```
docker compose up -d
```

**STEP 3**
Check in the `terminal` using this command
```
docker ps
```
the mongodb would exposed in the port `27017`

# Connecting the database
To connect the mongo use this `uri`

```
mongodb://<USERNAME>:<PASSWORD>@localhost:27017/?retryWrites=true&w=majority
```
change the `USERNAME` and `PASSWORD` with correct credentials

For the reference check this [StackOverFlow](https://stackoverflow.com/questions/75827552/keep-alive-query-failed/75994590#75994590)

# Other GitGub Repositories
* [mongodb-sample-dataset](https://github.com/neelabalan/mongodb-sample-dataset/)

# Load Data
Run the below commands to load the sample data
```
python -m venv env
```
```
source env\bin\activate
```
```
pip install -r requirements.txt
```
```
python load_data.py
```

# commands
### Connect Container Shell
```
docker exec -it mongo mongo -u <username> -p <password> --authenticationDatabase admin
```

### Create Dtabase
```
use <DATABASE_NAME>
```

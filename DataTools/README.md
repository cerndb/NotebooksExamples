# Data Tools Examples

[![SWAN](https://swan.web.cern.ch/sites/swan.web.cern.ch/files/pictures/open_in_swan.svg)](https://swan-k8s.cern.ch/user-redirect/download?projurl=https://github.com/cerndb/NotebooksExamples.git)
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cerndb/NotebooksExamples)

This contains a few example notebooks of popular frameworks and libraries for dealing with data.
Scale out data solutions, such as Spark and Dask, are not covered here.  
For Apache Spark see [SparkTraining](https://sparktraining.web.cern.ch/)  

For the relational database examples, CERN users can contact Oracle and DBOD services to get access to databases for testing, if needed.  
It's also possible to start test databases using container technology.

Running a test Oracle instance on container:
- Run Oracle Free on a container from gvenzl dockerhub repo https://github.com/gvenzl/oci-oracle-free
  - see also https://github.com/gvenzl/oci-oracle-free
  - `docker run -d --name mydb1 -e ORACLE_PASSWORD=oracle -p 1521:1521 gvenzl/oracle-free:latest`
  - Wait till the DB is started, it will take a few minutes. Check progress with: `docker logs -f mydb1`
  - install the Python library for connecting to Oracle: `pip install oracledb`

This is how you can set up an PostgreSQL instance for testing using a Docker image
 - `docker run --name some-postgres -p 5432:5432 -e POSTGRES_PASSWORD=mysecretpassword -d postgres`
 - wait till the DB is started, check logs at: `docker logs -f some-postgres`
 - install the Python library for connecting to PostgreSQL: `pip install psycopg2-binary`

## Contents

* [Pandas examples with plots](Pandas_examples_with_plots.ipynb)
* [Numpy examples with plots](Numpy_examples_with_plots.ipynb)
* [Queries to Oracle database](Query_Oracle.ipynb)
* [Queries to PostgreSQL database](Query_PostgreSQL.ipynb)

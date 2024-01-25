##  MSSQL
*port*: 1433
*user*: sa
*password*: l@bs#school1

Είχα πρόβλημα με τα permissions και έτρεξα:
> mkdir -p mssql/data
> mkdir -p mssql/log
> mkdir -p mssql/secrets
> ls -ll  //checks current permissions
> chgrp -R 0 mssql  //Added the root group to directories
> chmod -R g=u mssql
> chown -R 10001:0 mssql  //added non-root user to directories

*Πηγή*: https://stackoverflow.com/questions/65601077/unable-to-run-sql-server-2019-docker-with-volumes-and-get-error-setup-failed-co
## Postgress
Έχω δύο εγκαταστάσεις:
*port*: 5432
*user*: world
*password*: world123

*port*: 5432
*user*: postgres
*password*: example

## MySQL
*port*: 3306
*user*: root
*password*: example


## maria DB
*port*: 3307
*user*: root
*password*: 
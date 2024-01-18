Είχα πρόβλημα με τα permissions και έτρεξα:
> mkdir -p mssql/data
> mkdir -p mssql/log
> mkdir -p mssql/secrets
> ls -ll  //checks current permissions
> chgrp -R 0 mssql  //Added the root group to directories
> chmod -R g=u mssql
> chown -R 10001:0 mssql  //added non-root user to directories

Πηγή: https://stackoverflow.com/questions/65601077/unable-to-run-sql-server-2019-docker-with-volumes-and-get-error-setup-failed-co

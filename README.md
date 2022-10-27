# AWS-Database-Migration
This  steps through some of the variables defined in specifying migration from on-premises to AWS using the DMS. The eentire process of the migration is muhc more extensive than just the architecture diagrams and the environment variables. I'll detail these steps in a seperate article, for a thorough guide. 

This however just serves as...a repository of the scripts used. 

The application simulated in this project is Wordpress. Its implimnetation coommonly requires a web server and database setup. Thus, a LAMP server with mariadb implimentation is used. 
The requirements of your appliication's setup are mainly what will be used when specifying your bootstrap scripts or launch templates for your Auto scaling groups.

For  Wordpress in this case, specifyinng the DB password, username and endpoint, are such requiremeents of its setup. Replacing the said variables in wordpress' config file (wp-config) would be a common use case.

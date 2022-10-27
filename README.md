# AWS-Application-Scaling
This  steps through some of the variables defined in specifying scaling of an application. This application will use a lanch template which the scaling group will use to provision additional intances, as well as an <a href = "https://aws.amazon.com/elasticloadbalancing/"> application load balancer </a> attached to provide instance health check and of course, load balancing.

<a href= "https://aws.amazon.com/efs/"> EFS (Elastic File System) </a> is used to store the media files used by the application. 

The entire process of setting up auto-scaling in AWS is much more extensive than just the architecture diagrams and the environment variables. I'll detail these steps in a seperate article, for a thorough guide. If the green ec2 instance representattion confuses, please bare with me. Just wanted the architecture diagram to be aesthetically pleasing ツ 

This however just serves as...a repository of the scripts used. 

The application simulated in this project is Wordpress. Its implimnetation commonly requires a web server and database setup. Thus, <a href = "https://www.youtube.com/watch?v=tzBgFog6NmY&ab_channel=IBMTechnology">a LAMP (Linux Apache MySQL PHP) server</a> with mariadb implimentation is used. 
The requirements of your appliication's setup are mainly what will be used when specifying your bootstrap scripts or launch templates for your Auto scaling groups.

For  Wordpress in this case, specifying the DB password, username and endpoint, are such requiremeents of its setup. Replacing the said variables in wordpress' config file (wp-config) would be a common use case.


![App Evolution Diagram](AWS-App-Scaling.drawio.svg)
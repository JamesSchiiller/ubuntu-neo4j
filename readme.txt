1. CloudFormation fails to run `update-rc.d neo4j defaults`, starting neo4j upon restart, even if specified in template (SOMEONE HELP FIX! PLEASE!).

In the meantime, ssh into instance and run, 

ubuntu@ip-172-31-62-107:/var/log$ sudo update-rc.d neo4j defaults
ubuntu@ip-172-31-62-107:/var/log$ sudo reboot

2. Navigate to elasticip:7474

3. Default username: neo4j, password: neo4j

4. Set new password

5. Insert some test data via interactive web console, 

CREATE (n:Person { name: 'James', title: 'Developer' })

REFERENCES:

neo4j install process from: 

https://ronniethedba.wordpress.com/2016/10/28/installing-standalone-neo4j-in-ubuntu-16/

cloudformation template started from: 

https://github.com/neo4j-contrib/ec2neo







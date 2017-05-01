## Java EE 7 Tutorial: Java Message Service (JMS) API

Example taken from [Practical Java EE 7 Development using WildFly application server](http://www.itbuzzpress.com/ebooks/java-ee-7-development-on-wildfly.html)
___
#### - **jms-basic**

An example of calls between EJBs occurs when communication is done through the JMS API.

1. To activate the message flow in a aplication server WildFly it is necessary to start a full instance of the application server with the following command:
   ><HOME_WILDFLY/bin>$ ./standalone.sh -c standalone-full.xml

2. *JMS Connection Factories* and *JMS Destinations* available on the application server can be viewed, created and modified through the administration interface WildFly (Configuration > Subsystems > Messaging - ActiveMQ > default > Queues / Topics).

   For a correct execution it is necessary to create a new target queue **"java:/jms/queue/exampleQueue"** in your aplication server from the administration console. Queue is used in *MDBSample and* *MessageSender* classes.

3. Deploy your aplication on a aplication server and in a web browser enter the following URL: http://localhost:8080/javaee7-jms-basic/

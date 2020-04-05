# activemq-example

This is an example of how to use the Java JMS api with ActiveMQ executing both Pub/Sub and Queue based messaging.

# Building

Run:
> mvn clean install

After installed, we have a jar file in target folder of project with the name `activemq-example-1.0-SNAPSHOT.jar`

# How to run the example
There are two Java classes: com.gpcoder.Listener and com.gpcoder.Publisher. They are designed to exchange messages using either a Queue or a Topic (pub/sub).

You can run multiple Publishers and/or multiple Listeners.

### Start the JMS Consumers and Producer for Topic-based Messaging

> java -cp target/activemq-example-1.0-SNAPSHOT.jar com.gpcoder.Consumer Topic

>java -cp target/activemq-example-1.0-SNAPSHOT.jar com.gpcoder.Producer Topic

### Start the JMS Consumers and Producer for Queue-based Messaging

> java -cp target/activemq-example-1.0-SNAPSHOT.jar com.gpcoder.Consumer Queue

> java -cp target/activemq-example-1.0-SNAPSHOT.jar com.gpcoder.Producer Queue

### Shutdown JMS Consumer and Producer

To shutdown the Publisher and Listener enter `close` or `Ctrl + c`

Refer: https://gpcoder.com/6790-ket-noi-jms-client-voi-activemq/
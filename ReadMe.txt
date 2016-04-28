Sample Camel SMTP Project using Spring / Camel Boot and OSGi
=========================================

Prerequisites:

(1) Update src/main/resources/mail.properties with your from/to email addresses.
(2) Insert your SMTP email credentials into the email.uri field (in mail.properties).  For this example
I'm using GMAIL (hence SMTPS).

To build this project use

    mvn install

You can run this project using he following Maven goal:

    mvn camel:run

To deploy the project in OSGi. For example using Apache ServiceMix
or Apache Karaf. You will run the following command from its shell:

    osgi:install -s mvn:com.mycompany/camel-spring-smtp/1.0.0-SNAPSHOT

For more help see the Apache Camel documentation

    http://camel.apache.org/

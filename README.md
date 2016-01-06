# web-spring-java-simple
A simple Spring app

# Stack to use

FROM codenvy/ubuntu_jdk8

or


FROM codenvy/debian_jdk8

# How to run

Command #1 Build and copy war

mvn -f ${current.project.path} clean install

cp ${current.project.path}/target/*.war $TOMCAT_HOME/webapps/ROOT.war

Command #2 Run Tomcat

$TOMCAT_HOME/bin/catalina.sh run

Command #3 Stop Tomcat

#TOMCAT_HOME/bin/catalina.sh stop

Command #4 Tomcat Debug Mode

$TOMCAT_HOME/bin/catalina.sh jpda run
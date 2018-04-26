FROM tomcat:9-jre8

RUN wget http://search.maven.org/remotecontent?filepath=com/netflix/eureka/eureka-server/1.8.7/eureka-server-1.8.7.war

ADD server.xml /usr/local/tomcat/conf

RUN mv ./*.war ./webapps/eureka.war

RUN /usr/local/tomcat/bin/catalina.sh start

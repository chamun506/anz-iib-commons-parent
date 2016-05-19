# iib-maven-plugin
** Download the Plug-In to a directory such as /root/temp
- mvn org.apache.maven.plugins:maven-dependency-plugin:2.8:get -DrepoUrl=http://www.vadosity.com:8080/nexus/ -Dartifact=ch.sbb.maven.plugins:iib-maven-plugin:9.0-SNAPSHOT -Ddest=iib-maven-
plugin-9.0-20160205.025406-86.jar

** Install the IBM IntegrationAPI.jar in your local repository
- mvn install:install-file -DgroupId=com.ibm.broker.config  -DartifactId=proxy -Dversion=10.0.0.4 -Dpackaging=jar -Dfile="/root/IIB/iib-10.0.0.4/common/classes/IntegrationAPI.jar"

** Install the Plug-In in your local repository
- mvn install:install-file -Dfile=/root/temp/iib-maven-plugin-9.0-20160205.025406-86.jar -DgroupId=ch.sbb.maven.plugins -DartifactId=iib-maven-plugin -Dversion=9.0-SNAPSHOT -Dpackaging=jar






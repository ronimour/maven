# Generate Maven Wrapper in a specific version

mvn -N io.takari:maven:wrapper -Dmaven=3.6.0

# Generate Maven project from Archetype

mvn archetype:generate -DarchetypeGroupÍd=org.apache.maven.archetype -DarchetypeArtifactId=maven-archetype-simple -DarchetypeVersion=1.3

# Install dependency --> Oracle JDBC 7 driver example

mvn install:install-file -Dfile=./ojdbc7.jar -DgroupId=com.oracle -DartifactId=ojdbc -Dversion=12.1.0.1 -Dpackaging=jar

# Activating/Desactivating build profiles --> desactivating pageclound and activing nexus_distro

mvn clean deploy -P \!packagecloud,nexus_distro
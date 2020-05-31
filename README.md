# Generate Maven Wrapper in a specific version

mvn -N io.takari:maven:wrapper -Dmaven=3.6.0

# Generate Maven project from Archetype

mvn archetype:generate -DarchetypeGroupÍd=org.apache.maven.archetype -DarchetypeArtifactId=maven-archetype-simple -DarchetypeVersion=1.3

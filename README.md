Maven repository
================

Configuration
-------------

To add this repository to your [Maven][maven] project, add the following lines to your `pom.xml` or `settings.xml` file.

### Dependency repository

	<repositories>
		<repository>
			<id>cloudreports-snapshot-repo</id>
			<url>https://github.com/alessandroleite/maven-repository/raw/master/snapshots</url>
			<snapshots>
				<enabled>true</enabled>
			</snapshots>
		</repository>

		<repository>
			<id>cloudreports-repo</id>
			<url>https://github.com/alessandroleite/maven-repository/raw/master/releases</url>
			<snapshots>
				<enabled>false</enabled>
			</snapshots>
		</repository>
	</repositories>
	
### Plugin repository

	<pluginRepositories>
		<pluginRepository>
			<id>cloudreports-snapshots</id>
			<name>CloudReports Maven Plugin Repository</name>
			<url>https://github.com/alessandroleite/maven-repository/raw/master/snapshots</url>
			<layout>default</layout>
			<snapshots>
				<enabled>true</enabled>
			</snapshots>
		</pluginRepository>

		<pluginRepository>
			<id>cloudreports-releases</id>
			<name>CloudReports Maven Plugin Repository</name>
			<url>https://github.com/alessandroleite/maven-repository/raw/master/releases</url>
			<layout>default</layout>
			<snapshots>
				<enabled>false</enabled>
			</snapshots>
			<releases>
				<updatePolicy>never</updatePolicy>
			</releases>
		</pluginRepository>
	</pluginRepositories>
	
	
Configuration
-------------

* [CloudReports](https://github.com/thiagotts/CloudReports/)
* [CloudReports Maven Plugin](https://github.com/alessandroleite/cloudreports-maven-plugin)
* [CloudSim](http://www.cloudbus.org/cloudsim/)
* [Flanagan's Java Scientific Library](http://www.ee.ucl.ac.uk/~mflanaga/java/)


The following artifacts are available
-------------

	<dependency>
	     	<groupId>cloudreports</groupId>
		<artifactId>cloudreports</artifactId>
		<version>1.1</version>				
	</dependency>					
						

Maven Plugins
-------------
		<plugin>
			<groupId>cloudreports</groupId>
			<artifactId>cloudreports-maven-plugin</artifactId>
			<version>1.0.0-SNAPSHOT</version>		
		</plugin>
			
Deploy
-------------

```
mvn deploy:deploy-file
-Durl=file:PATH_TO_LOCAL/maven-repository/releases -Dfile=YOUR_FILE -DgroupId=GROUP_ID -DartifactId=ARTIFACT_ID -Dversion=VERSION -Dpackaging=PACKAGING
```			
			
[maven]:http://maven.apache.org/			
[cloudreports]:https://github.com/thiagotts/CloudReports/
[cloudreports-maven-plugin]:https://github.com/alessandroleite/cloudreports-maven-plugin
[cloudsim]:http://www.cloudbus.org/cloudsim/
[flanagan]:http://www.ee.ucl.ac.uk/~mflanaga/java/

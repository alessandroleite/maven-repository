Maven repository
================

Configuration
-------------

To add this repository to your Maven project, add the following lines to your `pom.xml` or `settings.xml` file.

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


Dependencies
-------------

			<dependency>
				<groupId>cloudreports</groupId>
				<artifactId>cloudreports</artifactId>
				<version>1.1</version>				
			</dependency>
			
			<dependency>
				<groupId>org.cloudbus</groupId>
				<artifactId>cloudsim</artifactId>
				<version>3.1</version>
				<scope>compile</scope>
			</dependency>
			
			<dependency>
			    <groupId>org.flanagan</groupId>
			    <artifactId>flanagan</artifactId>
			    <version>1.0</version>
			</dependency>							
			
[cloudreports]:https://github.com/thiagotts/CloudReports/
[cloudreports-maven-plugin]:https://github.com/alessandroleite/cloudreports-maven-plugin
[cloudsim]:http://www.cloudbus.org/cloudsim/
[flanagan]:http://www.ee.ucl.ac.uk/~mflanaga/java/
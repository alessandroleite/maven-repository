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
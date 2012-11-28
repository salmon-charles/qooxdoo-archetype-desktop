[qooxdoo-archetype home page]: http://qxmaven.charless.org/archetype

# Qooxdoo Archetype Desktop

The qooxdoo-archetype-desktop is a maven archetype to create a qooxdoo application within a maven project.

Creating, building and running a qooxdoo Rich Internet Application is as simple as:
```shell
$ mvn archetype:generate -DgroupId=org.test -DartifactId=appname -Dversion=0.1-SNAPSHOT -DarchetypeGroupId=org.qooxdoo -DarchetypeArtifactId=qooxdoo-archetype-desktop -DarchetypeVersion=1.6
$ cd appname
$ mvn jetty:run
```

Visit the [qooxdoo-archetype home page] project page for full documentation.

# Getting started

## Prerequisite

* Java
* Maven or Eclipse with m2e
* (Recommanded) Python

### Using an external python interpreter
This is the recommended way so far. 
Make sure python binary is on your path or specify the full path to the binary in the pom file.

```xml
<properties>
	<!-- Python settings -->
	<python.lin>python</python.lin>  <!-- Path to python interpreter on linux -->
	<python.win>python</python.win>  <!-- Path to python interpreter on windows -->
	<python.mac>python</python.mac>  <!-- Path to python interpreter on mac -->	
</properties>	
```

### Using the build-in Jyhton
**WARNING: THIS IS AN EXPERIMENTAL FEATURE !**

The first run can be very long; however, once the cache has been created, further runs are faster. 

Open the pom and set the `useEmbeddedJython` property to `true`.

```xml
<plugin>
	<groupId>org.qooxdoo</groupId>
	<artifactId>qooxdoo-maven-plugin</artifactId>
	<version>2.0-RC1</version>
	<extensions>true</extensions>
	<configuration>
		<useEmbeddedJython>true</useEmbeddedJython> <!-- Try a true value to enable the (EXPERIMENTAL) embedded Jython -->
	</configuration>
</plugin>
```

## Create the application

### Using the maven command line

```shell
$ mvn archetype:generate -DgroupId=org.test -DartifactId=appname -Dversion=0.1-SNAPSHOT -DarchetypeGroupId=org.qooxdoo -DarchetypeArtifactId=qooxdoo-archetype-desktop -DarchetypeVersion=1.6
$ cd appname
```

### Using Eclipse

You need to install the maven eclipse plugin first (m2e).

    1. Go to File/New/Other...
    2. Select Maven/Maven Project
       1. New Maven Project/Select project name and location page: 
           -   click Next
       2. New Maven Project/Select an Archetype page:
           -   Catalog: Select All catalogs
           -   Filter: type qooxdoo
           -   The qooxdoo-archetype-desktop should appear; select it and click Next
       3. New Maven Project/Enter an artifact id. page:
           -   enter project definition and click Next

## Build and run the application

### Using the maven command line

```shell
$ mvn jetty:run
```

Then open a browser : <http:///localhost:8080>

### Using Eclipse
           
On the project that has been created in Eclipse:

    1. Right-click the project and select `Run as/Maven build...`
    2. In `Goals`, write `jetty:run`
    3. Click `Run`

Then open a browser : <http:///localhost:8080>




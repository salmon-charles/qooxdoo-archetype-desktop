[qooxdoo-archetype home page]: http://qxmaven.charless.org/doku.php?id=artifacts:qooxdoo-maven-archetypes

# Qooxdoo Archetype Gui

The qooxdoo-archetype-gui is a maven archetype to create a qooxdoo application within a maven project.

Visit the [qooxdoo-archetype home page] project page for full documentation.

# Getting started

## Using the maven command line

			$ mvn archetype:generate -DgroupId=org.test -DartifactId=appname -Dversion=0.1-SNAPSHOT -DarchetypeGroupId=org.qooxdoo -DarchetypeArtifactId=qooxdoo-archetype-gui -DarchetypeVersion=1.5
			$ cd appname
			$ mvn package

Then open a browser : *file:///path/to/appname/target/qooxdoo/appname/build/index.html*

To build the development version:

			$ mvn -Dbuild.type=dev package

Then go to *file:///path/to/appname/target/qooxdoo/appname/source/index.html*

## Using Eclipse

You need to install the maven eclipse plugin first (m2e).

    1. Go to File/New/Other…
    2. Select Maven/Maven Project
       1. **New Maven Project/Select project name and location page**: 
           - click Next
       2. **New Maven Project/Select an Archetype page**:
           - Catalog: Select All catalogs
           - Filter: type qooxdoo
           - The qooxdoo-archetype-gui should appear; select it and click Next
       3. **New Maven Project/Enter an artifact id. page**:
           - enter project definition and click Next
           
The project will be created in Eclipse:
     - Right-click the project and select *Run as/Maven package*






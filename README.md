[project page]: http://salmon-charles.github.com/qooxdoo-archetype-desktop/

# Qooxdoo Archetype Desktop

The qooxdoo-archetype-desktop is a maven archetype to create a qooxdoo application within a maven project.

Creating, building and running a qooxdoo Rich Internet Application is as simple as:
```shell
$ mvn archetype:generate -DgroupId=org.test -DartifactId=appname -Dversion=0.1-SNAPSHOT -DarchetypeGroupId=org.qooxdoo -DarchetypeArtifactId=qooxdoo-archetype-desktop -DarchetypeVersion=2.0-RC1
$ cd appname
$ mvn jetty:run
```

Visit the [project page] for full documentation.

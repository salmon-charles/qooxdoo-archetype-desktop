# Version 2.1
- Added maven site documentation

- Changed qooxdoo-sdk and qooxdoo-maven-plugin version to 2.1

# Version 2.0-RC1

The archetype has been renamed from "qooxdoo-archetype-gui" to "qooxdoo-archetype-desktop"

- New properties:
  
  1. qooxdoo.build.job : name of the build job 
  2. qooxdoo.test.job : name of the job to build the testrunner
  3. qooxdoo.test.view : name of the view used for the testrunner
  4. qooxdoo.application.testDirectory  => ${project.basedir}/src/test/qooxdoo

- Changed properties values:

  1. qooxdoo.application.resourcesDirectory   => ${project.basedir}/src/main/resources/qooxdoo
  2. qooxdoo.application.translationDirectory => ${project.basedir}/src/main/resources/qooxdoo/translation
  3. qooxdoo.application.outputDirectory      => ${project.build.directory}/qooxdoo
  4. qooxdoo.application.cacheDirectory       => ${project.build.directory}/qooxdoo/cache

- Changed properties names
  1. python => qooxdoo.build.python

- Changed project structure :
  - translation => ${project.basedir}/src/main/resources/qooxdoo/translation
  - cache => ${project.build.directory}/qooxdoo/cache
  - test (NEW) => ${project.basedir}/src/test/qooxdoo/__artifactId__/test
  
  
  

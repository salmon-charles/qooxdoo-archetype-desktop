# Version 1.6

- New properties:
  
  1. qooxdoo.build.job : name of the build job 

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
  
- To discuss:
  1. Relative path
  2. Translation in build process ?
  3. Unit tests ?
  
  
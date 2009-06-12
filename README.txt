This provides a set of common targets for Gant usage.

Usage:

In your project's build.gant file, add the following line:

includeTargets << new File("${gant_common}/common.gant")

where "gant_common" points to the directory of this project.

common.gant expects to find a build.properties file with at least these two entries in it:

project.name=myprojectname
project.version=######

Finally, common.gant uses Ivy for dependency management, so an ivy.xml is required.


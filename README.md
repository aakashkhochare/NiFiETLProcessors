# NiFiETLProcessors
This repository contains the source code for ETL Processors from[1] implemented using NiFi and Edgent.
The Edgent jars are maintained in the /NiFiETLProcessors/repo directory. 

1. Add all the jars in the /NiFiETLProcessors/repo directory to your local maven repository. 
Eg: Adding edgent.api.function.jar to the local repo
```
 mvn install:install-file  "-Dfile=<path-to-edgent.api.function.jar>/edgent.api.function.jar" "-DgroupId=edgent.api" "-DartifactId=function" "-Dpackaging=jar" "-Dversion=1.0"
```
You may check the /NiFiETLProcessors/pom.xml for the version

2. ``` mvn install ```
3. Place all the JARs from /NiFiETLProcessors/repo and /NiFiETLProcessors/target/NifiWithEdgent-1.0.nar into <path-to-your-nifi-folder>/lib
4. Restart NiFi

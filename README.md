# Open PHACTS RSC SureCHEMBL dataset / linksets 

This repository contains the [SureChEMBL](https://www.surechembl.org/) 
linksets as generated
by [Royal Society of Chemistry](http://www.rsc.org/) for the 
[Open PHACTS](http://www.openphacts.org/) project.


## Requirements

* [Git Large File Storage](https://help.github.com/articles/versioning-large-files/)
* [Apache Maven 3](http://maven.apache.org/download.cgi)

## License

[Creative Commons Attribution-ShareAlike 3.0 Unported](http://creativecommons.org/licenses/by-sa/3.0/)

See the [VoID file](ops-rsc-surechembl-dataset/data/void_2016-02-24.ttl) for details.

## Building

    mvn clean install
    
Will generate these [Research Object bundles](http://w3id.org/bundle/):
 
* ops-rsc-surechembl-dataset/target/ops-rsc-surechembl-dataset-0.20160224.0-SNAPSHOT.data.zip
* ops-rsc-surechembl-linksets/target/ops-rsc-surechembl-linksets-0.20160224.0-SNAPSHOT.data.zip
  
## Maven repository

These artifacts are also available from the 
[data.openphacts.org Maven repository](http://data.openphacts.org/artifactory/data/), 
under the group Id 
[org.openphacts.data](http://data.openphacts.org/artifactory/data/org/openphacts/data/).


Use in your pom.xml:

```xml

  <dependencies>
    <dependency>
      <groupId>org.openphacts.data</groupId>
      <artifactId>ops-rsc-surechembl-linkset</artifactId>
      <version>0.20160224.0-SNAPSHOT</version>
      <type>data.zip</type>
    </dependency>
    <!-- or.. -->
    <dependency>
      <groupId>org.openphacts.data</groupId>
      <artifactId>ops-rsc-surechembl-dataset</artifactId>
      <version>0.20160224.0-SNAPSHOT</version>
      <type>data.zip</type>
    </dependency>
  </dependencies>

  <repositories>
    <repository>
      <id>ops</id>
      <name>Open PHACTS repository</name>
      <url>http://repository.mygrid.org.uk/artifactory/ops/</url>
      <releases />
      <snapshots />
    </repository>
  </repositories>
```

The `<version>` above might not be the latest, see the 
[GitHub releases](https://github.com/openphacts/ops-rsc-surechembl-dataset/releases)
for the latest version.


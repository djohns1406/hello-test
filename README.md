HERE Open Location Platform Data and Pipeline Examples

Copyright (c) 2017 - 2018 HERE Europe B.V.

Introduction
============
This repository contains the examples for HERE's Open Location Platform.   

* **Shared Utilities**   
Provides some tools that are useful across all the example projects.    
* **Sensor Data Ingestion Interface (SDII) Streaming Pipeline - Java**   
A streaming pipeline application written in Java. It reads from a stream of automotive _**SDII**_ messages, does some simple processing then writes results to another catalog.   
_see: flink-sdii-read-write-java_    
* **Sensor Data Ingestion Interface (SDII) Streaming Pipeline - Scala**   
A Scala version of the _Sensor Data Ingestion Interface (SDII) Streaming Pipeline_ example.    
_see: flink-sdii-read-write-scala_    
* **Data Library Examples**   
Provides Java examples of utilizing the standalone Data Client API to access the Open Location Platform Data Service.   
* **Traffic**   
Provides Java examples of reading and interpreting data from Open Location Platform Traffic Catalogs.    
* **Weather**   
Provides Java examples of reading and interpreting data from Open Location Platform Weather Catalogs.    
* **Reality Based Index Attribute Retriever**   
Provides Java examples of retrieving attributes from selected Reality Based Index Catalog layers

Development Setup
=================

Prerequisites
-------------

1. Requires Java 1.8
2. Requires Maven 3
3. Requires Python 2.7
4. An [Open Location Platform][1] Account.


Build instructions
------------------

With your [Open Location Platform][1] Account:

1. [Download your maven **settings.xml** file from your Open Location Platform account.](#download-maven-settings-file)
2. [Create an Open Location Platform Application Key, then download its **credentials.properties** file.](#create-an-app-key-and-download-credentials-file)
3. Open a command prompt at the working tree's root directory and type:

    `$ mvn clean install    `

    To build the project without running any examples.

    To run, see build instructions in each example's README file.

##### Download maven *settings* file
1. Login to the [Open Location Platform][1].
2. Click the arrow next to your name at the top right.
3. Select [**Access credentials**][2].
4. Click **Repository** tab.
5. Click **Generate Credentials** button.
7. Click **Download settings.xml**.
8. Place **settings.xml** file in your maven home directory     
      ```~/.m2/settings.xml```

##### Create an App Key and download credentials file
1. Login to the [Open Location Platform][1].
2. Click the arrow next to your name at the top right.
3. Select [**Access credentials**][2].
4. Click **Apps and keys** tab
5. Click **Register new app** button.
6. Enter an **APP NAME** and **APP DESCRIPTION**.
7. Click **Next** button.
8. Click **Create A Key** button.
9. Click **Download** button - a **credentials.properties** file will be downloaded.
10. Click **Done** button.
11. Move the credentials.properties file to your home directory under the folder
".here".    
   `~/.here/credentials.properties`   

## License

Unless otherwise noted in `LICENSE` files for specific files or directories, the [LICENSE](LICENSE) in the root applies to all content in this repository.    

[1]: https://platform.here.com/
[2]: https://platform.here.com/profile/access-credentials

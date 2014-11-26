jai-imageio
===========

This project provides modules to build OSGi Bundles and native Fragments for 
[Java Advanced Imaging (JAI) and JAI ImageIO](http://en.wikipedia.org/wiki/Java_Advanced_Imaging) Java Extension. At the moment native support is available for

 * Windows 32bit
 * Linux 32bit 
 * Linux 64bit

and non-native support for all other platforms. Minimum required JRE is 1.6
 
How to build
------------

Maven 3.0.x required. Eclipse plugin projects, fragements, features, and repository
are build with [Eclipse Tycho](https://eclipse.org/tycho).

1. Download Java Advanced Imaging jar's and native libs

  ```
    mvn clean install -f pom-libs.xml
  ```

1. Build Bundles, Fragements, Features and P2 Repository

  ```
    mvn clean install -f pom.xml
  ```

How to use the update site
--------------------------

Upload the resutling folder from the repository project <repository-project>/target/repository 
to your http server. 

You can also use the following Eclipse P2 update site:

http://udig.refractions.net/files/update-jai

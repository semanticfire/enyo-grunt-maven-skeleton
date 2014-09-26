enyo-grunt-maven-skeleton
======

This is the maven wrapper for the [enyo-grunt-skeleton](https://github.com/semanticfire/enyo-grunt-skeleton) project.
It allows you to use maven to build and zip the project results.

You can also integrate the build in to e.g. Jenkins CI

Requirements
------------
* npm
* node
* bower ( global install )
* grunt ( global install )
 
Building
--------
This will result in a .ZIP file in target, which contains the dist contents, you can copy it over to e.g. PhoneGap Build

`mvn package`

Cleaning
--------
This will clean up target and target-grunt , note the src/main/webapp/static will not be cleaned see Remarks


`mvn clean`


Remarks
-------

The src is completely untouched, if you want to test from the src/main/webapp/static folder you will need to setup the project there as well see [enyo-grunt-skeleton](https://github.com/semanticfire/enyo-grunt-skeleton) for instructions.
All changes made to the src/main/webapp/static contents will be copied over when running the `mvn package`

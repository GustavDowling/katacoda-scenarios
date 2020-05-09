We will begin by installing pit

## Task

First we need a Maven project. In this tutorial we will use the project "TriangleType" by Gustav Dowling.

To clone his repository we run:

`git clone [url here] && cd TriangleType`{{execute}}

This project includes a simple program in App.java with testcases in [fix]

`mvn run [whatever]`{{execute}}

To install the PIT plugin add this to your pom.xml file under the "plugins" tag

`<plugin>
    <groupId>org.pitest</groupId>
    <artifactId>pitest-maven</artifactId>
    <version>LATEST</version>
</plugin>`


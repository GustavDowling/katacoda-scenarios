We will begin by installing pit

## Task

First we need a Maven project. In this tutorial we will use the project "TriangleType" by Gustav Dowling.

To clone his repository we run:

`git clone https://github.com/GustavDowling/MutationTesting.git && cd MutationTesting && cd TriangleType`{{execute}}

This project includes a simple program in App.java with testcases in AppTest.java . Compile and run the program once.

`mvn package`{{execute}}

`mvn exec:java -Dexec.mainClass="tutorial.App"`{{execute}}

The program takes 3 integer lengths of sides of triangles and outputs if the triangle is "scalene" (all sides are of  different lengths), "equilateral" (all sides are of equal length), "isosceles" (two sides of equal length) , "invalid side length" (a side is of length 0 or lower) or "not a triangle" (one side is larger than or equal to the two other sides combined).

To install the PIT plugin add this to your pom.xml file under the "plugins" tag

`<plugin>
    <groupId>org.pitest</groupId>
    <artifactId>pitest-maven</artifactId>
    <version>LATEST</version>
</plugin>`

You can copy and paste this in the text editor here in Katacoda. Then compile the application and run the mutationtest.

`mvn package`{{execute}}

`mvn org.pitest:pitest-maven:mutationCoverage`{{execute}}



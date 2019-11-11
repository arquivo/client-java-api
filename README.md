
# TextSearch API Client

## Requirements

[Eclipse](http://www.eclipse.org) as IDE (if you want to use another, you must adapt the following instructions)

OR use javac

## Instructions for importing the library

1. In Eclipse (or the IDE to choose), create a new project (File -> New -> Java Project);


2. With the project created, you should replace the src and libs folders created by the existing folders in client-java-api.
	
	
3. **NOTE**: If you encounter multiple Class Not Found errors, make sure that the Libraries in the libs folder are in the Build Path of the project.
	

## Use
 
To use the created API, you can refer to the Main.java file in the package main to see some examples.

As a simple example, the code below allows you to query (and print) the first 25 versions of preserved web pages returned by the TextSearch platform:

```java
int limit = 25;
String versionsSTR = TextSearchConn.getVersions( Constants.queryTestSimple , 0 , limit );
System.out.println( versionsSTR );
```

## Libraries used 

* [GSON](http://code.google.com/p/google-gson/)
* [HTTP Client 4.2.3 Apache](http://hc.apache.org/downloads.cgi)
* [Junit](https://github.com/junit-team/junit)

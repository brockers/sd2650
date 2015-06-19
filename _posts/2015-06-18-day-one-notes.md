---
layout: post
title: "Day one notes"
date: 2015-06-18 17:00:00
categories: unit01
---

Below are some of the notes taken from the whiteboard at the end of the day.  

## Java Rules

* One class to a file
* Files are named the same as their classes
* All files should have the following structure:
	* package declaration
	* import statements
	* class declaration
		* class variables
* Package names are lowercase
* public static void main(String[] args)

## Java Command-line Workflow

To compile java files from the command line.

* Edit the file-name.java file
* "Compile" the file with javac
	* javac file-name.java
* Run newly created application with java
	* java file-name

If creating your own library additional steps are required.

* Create a folder for your library (this will be the basename of your package)
* Edit package library-folder/package-name.java
* Build your java binary
	* cd library-folder
	* javac package-name.java
* Create a jar file of the package folder
	* cd ..
	* jar -cf library.package-name.jar library/
* Build your main java library adding the jar file classpath
	* javac -cp library.package-name.jar file-name.java
* Run java app
	* java file-name

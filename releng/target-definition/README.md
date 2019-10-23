10. Exercise: Using a target platform for the build
10.1. Create project and target definition file

Create a new project of type General in the releng folder called target-definition.

Right-click on the new project and select the New  Other  Plug-in Development  Target Definition menu entry. Name the file eclipse-2019-03.target.
# The name is actually important. It must be the name of the Maven artifact id followed by .target.

Add the Eclipse RCP SDK and Equinox Target Components to your target definition file.

Activate the target definition file in the Eclipse IDE.
	

Of course, Tycho requires that the target platform definition actually works for development. If you have compile errors after activation in the Eclipse IDE, it will also not work for the automatic build.

10.2. Create pom file for the target definition file

Create a pom file in your target-definition project.

<project>
    <modelVersion>4.0.0</modelVersion>
    <parent>
        <groupId>com.vogella.tycho</groupId>
        <artifactId>com.vogella.tycho.releng</artifactId>
        <version>1.0.0-SNAPSHOT</version>
    </parent>
    <groupId>com.vogella.tycho</groupId>
    <artifactId>eclipse-2019-03</artifactId>
    <version>1.0.0-SNAPSHOT</version>
    <packaging>eclipse-target-definition</packaging>

</project>

to simplify this, just copy your eclipse again and point to it
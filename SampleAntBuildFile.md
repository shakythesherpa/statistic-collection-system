Here I have added a sample ant build.xml.



&lt;project name="HelloWorld" default="compile" basedir="."&gt;


> 

&lt;property name="srcJava" value="SourceCode" /&gt;


> 

&lt;property name="buildDir" value="bin" /&gt;



> 

&lt;target name="init"&gt;


> > <!-- Create the build directory structure used by compile -->
> > 

&lt;mkdir dir="${buildDir}"/&gt;


> > 

&lt;/target&gt;




> 

&lt;target name="cleanBuildDirs" description="clean up"&gt;


> > 

&lt;delete dir="${buildDir}/" /&gt;



> 

&lt;/target&gt;



> 

&lt;target name="compile" depends="init"&gt;


> > 

&lt;javac srcdir="${srcJava}" destdir="${buildDir}"/&gt;



> 

&lt;/target&gt;





&lt;/project&gt;


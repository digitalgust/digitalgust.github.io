## miniJVM website

this site shows gits of miniJVM


### miniJVM libaries 

These lists of jars used to miniJVM, if there is a jar named A.jar, put it in /binary/libex/, append it to cli -classpath.
```
    mini_jvm -bootclasspath ../lib/minijvm_rt.jar -cp ../libex/A.jar  com.main.class.Name
```
## Janino java compiler
   [Janino](http://janino-compiler.github.io/janino/)       
Janino is a super-small, super-fast Java compiler.   
Janino can not only compile a set of source files to a set of class files like JAVAC, but also compile a Java expression, a block, a class body, one .java file or a set of .java files in memory, load the bytecode and execute it directly in the same JVM.   
[janino.jar](https://github.com/digitalgust/digitalgust.github.io/blob/main/lib/janino.jar?raw=true)    
[commons-compiler.jar](https://github.com/digitalgust/digitalgust.github.io/blob/main/lib/commons-compiler.jar?raw=true)    
```
    #compile /binary/res/BpDeepTest.java
    mini_jvm -bootclasspath ../lib/minijvm_rt.jar -cp ../libex/janino.jar:../libex/commons-compiler.jar   org.codehaus.janino.Compiler  ../res/BpDeepTest.java
```




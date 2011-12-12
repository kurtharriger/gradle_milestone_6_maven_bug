> gradle build
:compileJava
[ant:javac] /Users/kurtharriger/code/gradle-bug/src/main/java/Application.java:1: package org.apache.hadoop.conf does not exist
[ant:javac] import org.apache.hadoop.conf.Configuration;
[ant:javac]                              ^
[ant:javac] 1 error


# JAR is resolved correctly

> gradle dependencies
:dependencies

------------------------------------------------------------
Root project
------------------------------------------------------------

archives - Configuration for archive artifacts.
No dependencies

compile - Classpath for compiling the main sources.
\--- org.apache.hadoop:hadoop-core:0.20.2-cdh3u0 [default]
     +--- com.cloudera.cdh:hadoop-ant:3.0 [compile,master,runtime]
     +--- commons-cli:commons-cli:1.2 [compile,master,runtime]
     +--- xmlenc:xmlenc:0.52 [compile,master,runtime]
     +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime]
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime]
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime]
     +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     +--- commons-net:commons-net:1.4.1 [compile,master,runtime]
     |    \--- oro:oro:2.0.8 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty:6.1.26 [compile,master,runtime]
     |    +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime]
     |    \--- org.mortbay.jetty:servlet-api:2.5-20081211 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime] (*)
     +--- tomcat:jasper-runtime:5.5.23 [compile,master,runtime]
     |    +--- commons-el:commons-el:1.0 [compile,master,runtime]
     |    |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime]
     +--- tomcat:jasper-compiler:5.5.23 [compile,master,runtime]
     |    +--- javax.servlet:jsp-api:2.0 [compile,master,runtime]
     |    |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     |    \--- ant:ant:1.6.5 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-mapper-asl:1.5.2 [compile,master,runtime]
     |    \--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime] (*)
     +--- javax.servlet.jsp:jsp-api:2.1 [compile,master,runtime]
     +--- commons-el:commons-el:1.0 [compile,master,runtime] (*)
     +--- net.java.dev.jets3t:jets3t:0.6.1 [compile,master,runtime]
     |    +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime] (*)
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     +--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     +--- hsqldb:hsqldb:1.8.0.7 [compile,master,runtime]
     +--- oro:oro:2.0.8 [compile,master,runtime] (*)
     \--- org.eclipse.jdt:core:3.1.1 [compile,master,runtime]

default - Configuration for default artifacts.
\--- org.apache.hadoop:hadoop-core:0.20.2-cdh3u0 [default]
     +--- com.cloudera.cdh:hadoop-ant:3.0 [compile,master,runtime]
     +--- commons-cli:commons-cli:1.2 [compile,master,runtime]
     +--- xmlenc:xmlenc:0.52 [compile,master,runtime]
     +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime]
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime]
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime]
     +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     +--- commons-net:commons-net:1.4.1 [compile,master,runtime]
     |    \--- oro:oro:2.0.8 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty:6.1.26 [compile,master,runtime]
     |    +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime]
     |    \--- org.mortbay.jetty:servlet-api:2.5-20081211 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime] (*)
     +--- tomcat:jasper-runtime:5.5.23 [compile,master,runtime]
     |    +--- commons-el:commons-el:1.0 [compile,master,runtime]
     |    |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime]
     +--- tomcat:jasper-compiler:5.5.23 [compile,master,runtime]
     |    +--- javax.servlet:jsp-api:2.0 [compile,master,runtime]
     |    |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     |    \--- ant:ant:1.6.5 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-mapper-asl:1.5.2 [compile,master,runtime]
     |    \--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime] (*)
     +--- javax.servlet.jsp:jsp-api:2.1 [compile,master,runtime]
     +--- commons-el:commons-el:1.0 [compile,master,runtime] (*)
     +--- net.java.dev.jets3t:jets3t:0.6.1 [compile,master,runtime]
     |    +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime] (*)
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     +--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     +--- hsqldb:hsqldb:1.8.0.7 [compile,master,runtime]
     +--- oro:oro:2.0.8 [compile,master,runtime] (*)
     \--- org.eclipse.jdt:core:3.1.1 [compile,master,runtime]

runtime - Classpath for running the compiled main classes.
\--- org.apache.hadoop:hadoop-core:0.20.2-cdh3u0 [default]
     +--- com.cloudera.cdh:hadoop-ant:3.0 [compile,master,runtime]
     +--- commons-cli:commons-cli:1.2 [compile,master,runtime]
     +--- xmlenc:xmlenc:0.52 [compile,master,runtime]
     +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime]
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime]
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime]
     +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     +--- commons-net:commons-net:1.4.1 [compile,master,runtime]
     |    \--- oro:oro:2.0.8 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty:6.1.26 [compile,master,runtime]
     |    +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime]
     |    \--- org.mortbay.jetty:servlet-api:2.5-20081211 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime] (*)
     +--- tomcat:jasper-runtime:5.5.23 [compile,master,runtime]
     |    +--- commons-el:commons-el:1.0 [compile,master,runtime]
     |    |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime]
     +--- tomcat:jasper-compiler:5.5.23 [compile,master,runtime]
     |    +--- javax.servlet:jsp-api:2.0 [compile,master,runtime]
     |    |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     |    \--- ant:ant:1.6.5 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-mapper-asl:1.5.2 [compile,master,runtime]
     |    \--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime] (*)
     +--- javax.servlet.jsp:jsp-api:2.1 [compile,master,runtime]
     +--- commons-el:commons-el:1.0 [compile,master,runtime] (*)
     +--- net.java.dev.jets3t:jets3t:0.6.1 [compile,master,runtime]
     |    +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime] (*)
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     +--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     +--- hsqldb:hsqldb:1.8.0.7 [compile,master,runtime]
     +--- oro:oro:2.0.8 [compile,master,runtime] (*)
     \--- org.eclipse.jdt:core:3.1.1 [compile,master,runtime]

testCompile - Classpath for compiling the test sources.
\--- org.apache.hadoop:hadoop-core:0.20.2-cdh3u0 [default]
     +--- com.cloudera.cdh:hadoop-ant:3.0 [compile,master,runtime]
     +--- commons-cli:commons-cli:1.2 [compile,master,runtime]
     +--- xmlenc:xmlenc:0.52 [compile,master,runtime]
     +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime]
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime]
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime]
     +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     +--- commons-net:commons-net:1.4.1 [compile,master,runtime]
     |    \--- oro:oro:2.0.8 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty:6.1.26 [compile,master,runtime]
     |    +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime]
     |    \--- org.mortbay.jetty:servlet-api:2.5-20081211 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime] (*)
     +--- tomcat:jasper-runtime:5.5.23 [compile,master,runtime]
     |    +--- commons-el:commons-el:1.0 [compile,master,runtime]
     |    |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime]
     +--- tomcat:jasper-compiler:5.5.23 [compile,master,runtime]
     |    +--- javax.servlet:jsp-api:2.0 [compile,master,runtime]
     |    |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     |    \--- ant:ant:1.6.5 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-mapper-asl:1.5.2 [compile,master,runtime]
     |    \--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime] (*)
     +--- javax.servlet.jsp:jsp-api:2.1 [compile,master,runtime]
     +--- commons-el:commons-el:1.0 [compile,master,runtime] (*)
     +--- net.java.dev.jets3t:jets3t:0.6.1 [compile,master,runtime]
     |    +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime] (*)
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     +--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     +--- hsqldb:hsqldb:1.8.0.7 [compile,master,runtime]
     +--- oro:oro:2.0.8 [compile,master,runtime] (*)
     \--- org.eclipse.jdt:core:3.1.1 [compile,master,runtime]

testRuntime - Classpath for running the compiled test classes.
\--- org.apache.hadoop:hadoop-core:0.20.2-cdh3u0 [default]
     +--- com.cloudera.cdh:hadoop-ant:3.0 [compile,master,runtime]
     +--- commons-cli:commons-cli:1.2 [compile,master,runtime]
     +--- xmlenc:xmlenc:0.52 [compile,master,runtime]
     +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime]
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime]
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime]
     +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     +--- commons-net:commons-net:1.4.1 [compile,master,runtime]
     |    \--- oro:oro:2.0.8 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty:6.1.26 [compile,master,runtime]
     |    +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime]
     |    \--- org.mortbay.jetty:servlet-api:2.5-20081211 [compile,master,runtime]
     +--- org.mortbay.jetty:jetty-util:6.1.26 [compile,master,runtime] (*)
     +--- tomcat:jasper-runtime:5.5.23 [compile,master,runtime]
     |    +--- commons-el:commons-el:1.0 [compile,master,runtime]
     |    |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime]
     +--- tomcat:jasper-compiler:5.5.23 [compile,master,runtime]
     |    +--- javax.servlet:jsp-api:2.0 [compile,master,runtime]
     |    |    \--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     |    \--- ant:ant:1.6.5 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime]
     +--- org.codehaus.jackson:jackson-mapper-asl:1.5.2 [compile,master,runtime]
     |    \--- org.codehaus.jackson:jackson-core-asl:1.5.2 [compile,master,runtime] (*)
     +--- javax.servlet.jsp:jsp-api:2.1 [compile,master,runtime]
     +--- commons-el:commons-el:1.0 [compile,master,runtime] (*)
     +--- net.java.dev.jets3t:jets3t:0.6.1 [compile,master,runtime]
     |    +--- commons-httpclient:commons-httpclient:3.1 [compile,master,runtime] (*)
     |    +--- commons-codec:commons-codec:1.4 [compile,master,runtime] (*)
     |    \--- commons-logging:commons-logging:1.1.1 [compile,master,runtime] (*)
     +--- javax.servlet:servlet-api:2.5 [compile,master,runtime] (*)
     +--- hsqldb:hsqldb:1.8.0.7 [compile,master,runtime]
     +--- oro:oro:2.0.8 [compile,master,runtime] (*)
     \--- org.eclipse.jdt:core:3.1.1 [compile,master,runtime]

(*) - dependencies omitted (listed previously)

BUILD SUCCESSFUL

# However jar is not added to classpath during build

> gradle --debug clean build | tee build.out
...
> grep classpath -A1 build.out | grep hadoop-core
>

This is an example, based on a real-life project, which demonstrates an efficient way to run GWT applications under Eclipse and "DevMode", but without Jetty runtime JAR parsing issues.

for example:

Error scanning entry META-INF/versions/9/org/apache/logging/log4j/util/Base64Util.class from jar file:/.../eclipse-gwt-recipe/modules/gwt-web-eclipse/target/eclipse-gwt-recipe.web.gwt.eclipse-0.0.1-SNAPSHOT/WEB-INF/lib/log4j-api-2.13.3.jar
at org.eclipse.jetty.annotations.AnnotationParser.parseJar(AnnotationParser.java:913)
... 6 more
Caused by: java.lang.IllegalArgumentException at org.objectweb.asm.ClassReader.<init>(Unknown Source)
at org.objectweb.asm.ClassReader.<init>(Unknown Source) at org.objectweb.asm.ClassReader.<init>(Unknown Source)
at org.eclipse.jetty.annotations.AnnotationParser.scanClass(AnnotationParser.java:973)
at org.eclipse.jetty.annotations.AnnotationParser.parseJarEntry(AnnotationParser.java:956)
at org.eclipse.jetty.annotations.AnnotationParser.parseJar(AnnotationParser.java:909)
... 6 more

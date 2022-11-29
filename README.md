# jogl-text-renderer

Improvement of JOGL TextRenderer submitted [long time ago but never merged in JOGL](https://github.com/sgothel/jogl/pull/47).

This improvement
- makes text rendering more clean (reduce blurry effect)
- reduce memory footprint of font cache

To get it in your project, add this dependency to your Maven project :

```xml
<dependency>
  <groupId>org.jzy3d</groupId>
  <artifactId>jogl-text-renderer</artifactId>
  <version>2.4-SNAPSHOT</version>
</dependency>
```

Which requires you add this to this list of Maven repositories in your Maven project :

```xml
<repositories>
  <repository>
    <id>jzy3d-snapshots</id>
    <name>Jzy3d Snapshots</name>
    <url>https://maven.jzy3d.org/snapshots/</url>
  </repository>
  <repository>
    <id>jzy3d-releases</id>
    <name>Jzy3d Releases</name>
    <url>https://maven.jzy3d.org/releases/</url>
  </repository>
</repositories>
```

The `TextRenderer` in this module has exactly the same name than the existing one in JOGL distro. While I could get `jogl-text-renderer` loaded first in my IDE classpath, it may be overriden by the original text renderer when you run on your setup!

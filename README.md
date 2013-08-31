jniloader
=========

Simple (for the end user) native library loader.

The static method in `JniLoader` enables developers to ship native
libraries in jar files which are extracted and loaded at runtime,
making native loading transparent for the end-user (as long as
they are on a platform supported by you).

Native libraries can also be placed in `java.library.path` for
slightly faster startup times (tens of milliseconds during JVM startup).


Installation
============

The latest release is available from Maven Central, e.g.:

```xml
<dependency>
  <groupId>com.github.fommil</groupId>
  <artifactId>jniloader</artifactId>
  <version>1.0</version>
</dependency>
```


Snapshots are distributed on Sonatype's Snapshot Repository:

```xml
<dependency>
  <groupId>com.github.fommil</groupId>
  <artifactId>jniloader</artifactId>
  <version>1.1-SNAPSHOT</version>
</dependency>
```

If the above fails, ensure you have the following in your `pom.xml`:

```xml
    <repositories>
        <repository>
            <id>sonatype-snapshots</id>
            <url>https://oss.sonatype.org/content/repositories/snapshots/</url>
            <releases>
                <enabled>false</enabled>
            </releases>
            <snapshots>
                <enabled>true</enabled>
            </snapshots>
        </repository>
    </repositories>
```


Donations
=========

Please consider supporting the maintenance of this open source project with a donation:

[![Donate via Paypal](https://www.paypal.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=B2HW5ATB8C3QW&lc=GB&item_name=jniloader&currency_code=GBP&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted)


Contributing
============

Contributors are encouraged to fork this repository and issue pull
requests. Contributors implicitly agree to assign an unrestricted licence
to Sam Halliday, but retain the copyright of their code (this means
we both have the freedom to update the licence for those contributions).


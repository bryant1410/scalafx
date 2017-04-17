ScalaFX is a UI DSL written within the Scala Language that sits on top of JavaFX
8 and JavaFX 2.2. This means that every ScalaFX application is also a
valid Scala application. By extension it supports full interoperability with
Java and can run anywhere the Java Virtual Machine (JVM) and JavaFX 8 or JavaFX 2.2
are supported.

[![Join the chat at https://gitter.im/scalafx/scalafx](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/scalafx/scalafx?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![Build Status](https://travis-ci.org/scalafx/scalafx.svg?branch=master)](https://travis-ci.org/scalafx/scalafx)   [![Maven Central](https://maven-badges.herokuapp.com/maven-central/org.scalafx/scalafx_2.11/badge.svg)](https://maven-badges.herokuapp.com/maven-central/org.scalafx/scalafx_2.11) [![Scaladoc](http://javadoc-badge.appspot.com/org.scalafx/scalafx_2.11.svg?label=scaladoc)](http://javadoc-badge.appspot.com/org.scalafx/scalafx_2.11) [![Reference Status](https://www.versioneye.com/java/org.scalafx:scalafx_2.11/reference_badge.svg?style=flat)](https://www.versioneye.com/java/org.scalafx:scalafx_2.11/references)

ScalaFX was originally created by Stephen Chin, Java Champion, Oracle JavaOne
program chair; and Sven Reimers, a member of the Netbeans Dream Team.

There are two branches of ScalaFX: v.8.0 supporting JavaFX 8 (Java 8) and
v.2.2 supporting JavaFX 2.x (Java 7).

ScalaFX binaries are published in the Maven Central repository:
[http://search.maven.org/#search|ga|1|scalafx](http://search.maven.org/#search%7Cga%7C1%7Cscalafx)

To use ScalaFX with SBT and Java 8 add following dependency (to use
the latest scalafx you might need Java version at least 1.8.40):

```scala
libraryDependencies += "org.scalafx" %% "scalafx" % "8.0.102-R11"
```

With Java 7 use:

```scala
libraryDependencies += "org.scalafx" %% "scalafx" % "2.2.76-R11"
```

For latest development version:

```scala
libraryDependencies += "org.scalafx" %% "scalafx" % "8.0.102-R12-SNAPSHOT"
```

The [ScalaFX Organization page](https://github.com/scalafx) on GitHub contains several sample
project that illustrate use of ScalaFX.
The simplest one, and recommended to start with, is [`scalafx-hello-world`](https://github.com/scalafx/scalafx-hello-world).

Snapshot releases are also regularly published on Sonatype. To use a snapshot
build you may need to add "Sonatype OSS Snapshots" resolver to you SBT
configuration:

```scala
resolvers += Opts.resolver.sonatypeSnapshots
```

If you just want to download a recent snapshot build you can also use Travis CI build site
https://travis-ci.org/scalafx/scalafx

ScalaFX source code is using the SBT build system.
For information on building with SBT see `README-SBT.txt`.

The official web site for ScalaFX is http://scalafx.org.


# Software License

This software licensed under BSD Open Source.

The License text for this software can be found in [LICENSE.txt](LICENSE.txt) in the root
folder of the project.


# Software Required

The following software is needed to build ScalaFX:

  1. [SBT](http://www.scala-sbt.org/) v.0.13.5 or better
  2. [Scala](http://www.scala.org/)
    - ScalaFX 8.0 builds with Scala 2.10.2 or newer.
    - ScalaFX 2.2 builds with either Scala version 2.9.3+, 2.10.+, or 2.11.+

It works with Windows, MacOS X and Linux ports.


# Project Structure

The current project structure looks like this:

    ./archive
    ./project
    ./scalafx
    ./scalafx-demos

Where `.` is a the root folder of the project.

The `archive` folder is reserved for remnants of the previous single module
build system.

The `scalafx` folder is the sub project for the ScalaFX Framework.

The `scalafx-demos` is the sub project for the ScalaFX Framework Demonstrations (some are a bit out of date, help needed here :).

The `project` folder is reserved for Scala SBT.


# Source Code Branching Policy

The current development is for ScalaFX 8 and it is done on the `master` branch. Releases are done on the `stable` branch. Releases are tagged with version number. Pull requests are only accepted off a brunch created from the `master` branch. When working on a pull request, create a separate branch for each feature or bug fix. This way the main development branch is not blocked by a pull request and pull requests are easier to merge individually.

The ScalaFX 2.2 development is no longer active. For those who need it, the code is on the `SFX-2` branch and past releases are on the `SFX-2-stable` branch. 


# Credits

You can find the full list of committers, developers and contributors in
the file [MAINTAINERS.txt](MAINTAINERS.txt).

# Community
We request all the team members to follow the [Typelevel Code of Conduct](http://typelevel.org/conduct.html) in our mailinglist, issue discussion, Gitter room or any of ScalaFX meetups.

For more info on Contribute, check our [Contributing page](http://http://www.scalafx.org/docs/contributing/).

# Software engineering methods and tools lab work 3

**Project building systems**: *apache ant*, *maven*, *make*.

**Project testing**: *JUnit*


# Project structure

* **WebLabWork3** - folder with nested project which *ant* will look into
* **build.xml** - ant build script
* **build.properties** - properties to configure ant script
* **dependencies** - WebLabWork3 dependencies jars
* **music** - music folder for *music* target


# Usage

First, you must have installed ***Apache Ant*** and ***Java 1.8+ JDK*** on your computer
(It's better to set **ANT_HOME** and **JAVA_HOME** environment variables).

Second, replace *build.properties.origin* with *build.properties* by replacing "???" with
your properties (or not only "???")

Third, now you can type next commands in the root folder of this project (all these 
descriptions you can also find in the *build.xml* file):

```bash
ant                       # acts similar as the "ant build" command
```

```bash
ant compile               # compile project source classes
```

```bash
ant build                 # compile sources and pack to an executable war archive
```

```bash
ant clean                 # clean compiled classes and temporary files
```

```bash
ant test                  # launch project JUnit tests
```

```bash
ant scp                   # send built project to server via scp
```

```bash
ant xml                   # validate all project's xml files
```

```bash
ant music                 # play music after building the sources
```

```bash
ant native2ascii          # use native2ascii transform with localization files
```

```bash
ant report                # in case of all tests passed save xml junit report, add it to repository and commit
```

```bash
ant history               # create diff of files changed after last revision that can be built
```

```bash
ant team                  # get 4 last git revisions, build them and zip
```

```bash
ant diff                  # checks working copy status. Makes commit if changes doesn't contain files from property file
```
---
published: true
title: FOSSLight Dependency Scanner
---
# FOSSLight Dependency Scanner

<img src="https://img.shields.io/pypi/l/fosslight_dependency" alt="License" /> <img src="https://img.shields.io/pypi/v/fosslight_dependency" alt="Current python package version." /> <img src="https://img.shields.io/pypi/pyversions/fosslight_dependency" /> [![REUSE status](https://api.reuse.software/badge/github.com/fosslight/fosslight_dependency_scanner)](https://api.reuse.software/info/github.com/fosslight/fosslight_dependency_scanner)
    
[**FOSSLight Dependency Scanner**](https://github.com/fosslight/fosslight_dependency_scanner)utilizes the open source software for analyzing each package manager dependencies. We choose the open source software for each package manager that shows not only the direct dependencies but also the transitive dependencies including the information of dependencies such as oss name, oss version and license name.    
    
The list of supported Package Managers is as follows.     
- [Gradle](https://gradle.org/) (Java)
- [Maven](http://maven.apache.org/) (Java)
- [NPM](https://www.npmjs.com/) (Node.js)
- [PIP](https://pip.pypa.io/) (Python)
- [Pub](https://pub.dev/) (Dart with flutter)
- [Cocoapods](https://cocoapods.org/) (Swift/Obj-C)


## User Guide
  - [Prerequisite](#-prerequisite)
    - [NPM](#npm)
    - [Gradle](#gradle)
    - [Android-gradle](#android-gradle)
    - [Pypi](#pypi)
    - [Maven (optional)](#maven-optional)
    - [Pub](#pub)
    - [Cocoapods](#cocoapods)
  - [How to install](#-how-to-install)
  - [How to run](#-how-to-run)
  - [Result](#-result)


## 📋 Prerequisite
Because we utilizes the different open source software to analyze the dependencies of each package manager, you need to set up the below [Prerequisite](#-prerequisite) steps according to package manager to analyze.

### NPM

1. Install the NPM License Checker to analyze the npm dependencies.

```
$ npm install -g license-checker
```

2. Run the command to install the dependencies. (optional)

```
$ npm install
```

> - If the 'package.json' file exists in the input directory, it will be executed automatically by FOSSLight Dependency Scanner. So you can skip it.
> - If the 'node_modules' directory already exists, you can run FOSSLight Dependency Scanner by setting the input directory to the path where node_modules is located.

### Gradle

1. Add the License Gradle Plugin in build.gradle file.

```
plugins {
    id 'com.github.hierynomus.license' version '0.15.0'
}

downloadLicenses {
    includeProjectDependencies = true
    dependencyConfiguration = 'runtimeClasspath'
}
```

> - If the gradle version is 4.6 or lower, then add the 'runtime' instead of 'runtimeClasspath' in the dependencyConfiguration.

2. Run the 'downloadLicenses' task.

```
$ gradle downloadLicenses
```

### Android (gradle)

1. Add the Android License Plugin in build.gradle file.

```
buildscript {
    repositories {
        jcenter()
    }

    dependencies {
        classpath 'com.lge.android.licensetools:android-dependency-scanning:0.4.0'
    }
}

apply plugin: 'com.lge.android.licensetools'
```

2. Run the 'generateLicenseTxt' task.

```
$ gradle generateLicenseTxt
```


### Pypi

You can run this tool with virtual environment for separating the project dependencies from system global dependencies.

1. Create and activate the virtual environment

```
// virtualenv example
$ virtualenv -p /usr/bin/python3.6 venv
$ source venv/bin/activate

// conda example
$ conda create --name {venv name}
$ conda activate {venv name}
```

2. Install the dependencies in the virtual environment.

```
// If you install the dependencies with requirements.txt...
$ pip install -r requirements.txt
```


### Maven (optional)

> - If the 'pom.xml' is located in the input directory, FOSSLight Dependency Scanner will automatically add and execute the license-maven-plugin. So you can skip the prerequisites below.

1. Add the license-maven-plugin into pom.xml file.

```
<project>
  ...
  <build>
  ...
    <plugins>
    ...
      <plugin>
        <groupId>org.codehaus.mojo</groupId>
        <artifactId>license-maven-plugin</artifactId>
        <version>2.0.0</version>
        <executions>
          <execution>
            <id>aggregate-download-licenses</id>
            <goals>
              <goal>aggregate-download-licenses</goal>
            </goals>
          </execution>
        </executions>
      </plugin>
    </plugins>
    ...
  </build>
  ...
</project>
```

2. Run the license-maven-plugin task.

```
$ mvn license:aggregate-download-licenses
```

### Pub

1. Run the flutter_oss_licenses.

```
$ flutter pub get
$ flutter pub global activate flutter_oss_licenses
$ flutter pub global run flutter_oss_licenses:generate.dart
```

### Cocoapods

1. Install the pod package through Podfile.

```
$ pod install
```


## 🎉 How to install

FOSSLight Dependency Scanner can be installed using pip3.    
It is recommended to install in the [python 3.6 + virtualenv](etc/guide_virtualenv.md) environment.

```
$ pip install fosslight-dependency
```

## 🚀 How to run

You can run the FOSSLight Dependency Scanner with options based on your package manager.

```
$ fosslight_dependency
```

| Option | Argument                                         | Description                                                                                 |
| ------ | ------------------------------------------------ | ------------------------------------------------------------------------------------------- |
| -m     | npm, maven, gradle, pip, pub, cocoapods, android | (optional) <br> package manager for your project                                            |
| -p     | (path)                                           | (optional) <br> input directory                                                             |
| -o     | (path)                                           | (optional) <br> output file directory                                                       |
| -a     | conda example: 'conda activate (venv name)'      | (pypi only required) <br> virtual environment activate command                              |
| -d     | conda example: 'conda deactivate'                | (pypi only required) <br> virtual environment deactivate command                            |
| -c     | (customized output directory name)               | (gradle, maven only optional) <br> customized build output directory name (default: target) |
| -n     | (app name)                                       | (android only optional) <br> app directory name (default: app)                              |
| -v     | N/A                                              | release version                                                                             |

Note that input directory should be the top directory of the project where the manifest file of the package manager is located.
For example, if your project uses the NPM package manager, then the input directory should be the path where 'package.json' file is located.
The manifest file of each package manager is as follows:

| Package manager | Npm          | Pip              | Maven   | Gradle       | Pub          | Cocoapods | Android |
| --------------- | ------------ | ---------------- | ------- | ------------ | ------------ | --------- | ------- |
| Manifest file   | package.json | requirements.txt | pom.xml | build.gradle | pubspec.yaml | Podfile   | gradlew |

In other words, the input directory('-p' option) should be designated as the top directory of the project where the package manager's manifest file exists as above.
The manifest file of android project is 'build.gradle' as same as the gradle project. But for differentiating with other java projects, it checks 'gradlew' files.


## 📁 Result

FOSSLight Dependency Scanner creates the result file that has xlsx extension (Microsoft Excel file).

It prints the OSS information based on manifest file(package.json, pom.xml) of dependencies (including transitive dependencies).
For a unique OSS name, OSS name is printed such as (package_manager):(oss name) or (group id):(artifact id).

| Package manager                | OSS Name                 | Download Location                                                                                  | Homepage                                            |
| ------------------------------ | ------------------------ | -------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| Npm                            | npm:(oss name)           | Priority1. repository in package.json <br> Priority2. npmjs.com/package/(oss name)/v/(oss version) | npmjs.com/package/(oss name)                        |
| Pip                            | pypi:(oss name)          | pypi.org/project/(oss name)/(version)                                                              | homepage in (pip show) information                  |
| Maven<br>& Gradle<br>& Android | (group_id):(artifact_id) | mvnrepository.com/artifact/(group id)/(artifact id)/(version)                                      | mvnrepository.com/artifact/(group id)/(artifact id) |
| Pub                            | pub:(oss name)           | pub.dev/packages/(oss name)/versions/(version)                                                     | homepage in (pub information)                       |
| Cocoapods                      | cocoapods:(oss name)     | source in (pod spec information)                                                                   | cocoapods.org/(oss name)                            |
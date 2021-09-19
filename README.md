### CI-CD
# **Build - Using Gradle**
## Install Gradle and set **gradle** command in `/etc/profile.d/gradle.sh`
- `sudo apt update`
- `sudo apt install openjdk-8-jdk`
  > Installing dependency
- `wget https://services.gradle.org/distributions/gradle-5.0-bin.zip -P /tmp`
- `sudo unzip -d /opt/gradle /tmp/gradle-*.zip`
- `sudo vi /etc/profile.d/gradle.sh`
  > setting gradle command to work
- `export GRADLE_HOME=/opt/gradle/gradle-5.0;`
  `export PATH=${GRADLE_HOME}/bin:${PATH};`
- `sudo chmod 755 /etc/profile.d/gradle.sh`
- `source /etc/profile.d/gradle.sh`
- `gradle -v`
***
## Gradle & Gradle Wrapper
- `gradle wrapper` - to run graddle wrapper
- `gradle init` - command, which will create **`build.gradle`** and graddle wrapper setup.
- `./gradlew build` - sample gradle wrapper command
- we need to set tasks in **`build.gradle`** depends on our requirement
  > checkout **`build.gradle`** in code-block
## Automated testing
- **unit test** - for testing small piece of code
- **integration test** - test larger portions of application integrated with each other
- **smoke / sanity test** - high level integration test that verify basic, large scale things like weather or not the application runs, application endpoint return 500 error

- clone the `cicd-gradle-automation-testing` folder for testing how Automation works
***

## You can clone `sample-build-jenkins` Branch for checking Build Steps using Jenkins as Gradle Build

***

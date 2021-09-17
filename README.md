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

***

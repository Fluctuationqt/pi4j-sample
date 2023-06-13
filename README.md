# pi4j-sample

Repo with a mvn project pi4j sample for a Raspberry Pi

## Prerequisite - Setup Maven (SKIP this if already setup)
```
wget https://downloads.apache.org/maven/maven-3/3.9.2/binaries/apache-maven-3.9.2-bin.tar.gz
cd /opt && sudo tar -xzvf /home/pi/Downloads/apache-maven-3.6.1-bin.tar.gz
```
`nano ~/.bashrc` -> Add the following lines and save the file:
```
export M2_HOME=/opt/apache-maven-3.2.5
export "PATH=$PATH:$M2_HOME/bin"
```
`source ~/.bashrc`
Run `mvn -v` to verify the install was successful

## Clone and run the project

```
git clone https://github.com/Fluctuationqt/pi4j-sample
cd pi4j-sample
mvn clean install
sudo java -jar target/pi4j-sample-1.0-SNAPSHOT.jar
```


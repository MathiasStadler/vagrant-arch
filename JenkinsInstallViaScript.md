# JenkinsInstallViaScript

## clone

```bash
git clone https://github.com/edx/jenkins-configuration
cd jenkins-configuration
```

## install java und pip

```bash
# java
sudo pacman -S extra/jdk8-openjdk

#pip
sudo pacman -S python-pip
```

## run requirements and plugins

```bash
export JENKINS_VERSION="jenkins_2.164.2"
export JENKINS_WAR_SOURCE="http://repo.jenkins-ci.org/releases/"
export CONFIG_PATH=${pwd}/test_data
export TEST_SHARD="shard_2"
export CONTAINER_NAME="jenkins_of_scripts"
make clean requirements plugins
```

## build container

```bash
export JENKINS_VERSION="jenkins"
export JENKINS_WAR_SOURCE="http://mirrors.jenkins.io/war-stable/2.164.2"
export CONFIG_PATH=${pwd}/test_data
export TEST_SHARD="shard_2"
export CONTAINER_NAME="jenkins_of_scripts"
make build
```

## run container

```bash
## run
export JENKINS_VERSION="jenkins"
export JENKINS_WAR_SOURCE="http://mirrors.jenkins.io/war-stable/2.164.2"
export CONFIG_PATH=${pwd}/test_data
export TEST_SHARD="shard_2"
export CONTAINER_NAME="jenkins_of_scripts"
make run
```
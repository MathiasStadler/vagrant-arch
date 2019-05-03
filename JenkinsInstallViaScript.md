# JenkinsInstallViaScript

## clone

```bash
git clone https://github.com/edx/jenkins-configuration
```

## prepare

```bash
export JENKINS_VERSION="jenkins_2.164.2"
export JENKINS_WAR_SOURCE="http://repo.jenkins-ci.org/releases/"
export CONFIG_PATH=${pwd}/test_data
export TEST_SHARD="shard_2"
export CONTAINER_NAME="jenkins_of_scripts"
make clean requirements plugins
```

## build

```bash
export JENKINS_VERSION="jenkins"
export JENKINS_WAR_SOURCE="http://mirrors.jenkins.io/war-stable/2.164.2"
export CONFIG_PATH=${pwd}/test_data
export TEST_SHARD="shard_2"
export CONTAINER_NAME="jenkins_of_scripts"
make build
```

## run

```bash
## run
export JENKINS_VERSION="jenkins"
export JENKINS_WAR_SOURCE="http://mirrors.jenkins.io/war-stable/2.164.2"
export CONFIG_PATH=${pwd}/test_data
export TEST_SHARD="shard_2"
export CONTAINER_NAME="jenkins_of_scripts"
make run
```
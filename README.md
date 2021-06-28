# TestServerHookGradle

**Recommended to use [sya-ri/minecraft-server-gradle-plugin](https://github.com/sya-ri/minecraft-server-gradle-plugin).**

## Installation

1. Open Terminal
2. Run Command
```shell
wget https://github.com/sya-ri/TestServerHookGradle/archive/master.zip
unzip master.zip
rm master.zip
mv TestServerHookGradle-master _test_server
cd _test_server
sh install_server.sh
```

## Setting IntelliJ Task

### Create Shell Script Task
```yml
Name: Test
Script path: <Paste Project Path>/_test_server/start.sh
Working direcotry: <Paste Project Path>/_test_server
Before Launch: 
  - Run Gradle Task:
      Gradle project: <Paste Your Project Name>
      tasks: shadowJar
```

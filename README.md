# scgraph
Static Call Graph Generator

# Project Initiation

1. ~/.m2/settins.xml
```xml
<settings>
    <pluginGroups>
        <pluginGroup>org.jenkins-ci.tools</pluginGroup>
    </pluginGroups>
    <profiles>
        <profile>
            <id>jenkins</id>
            <activation>
                <activeByDefault>true</activeByDefault>
            </activation>
            <repositories>
                <repository>
                    <id>repo.jenkins-ci.org</id>
                    <url>http://repo.jenkins-ci.org/public/</url>
                </repository>
            </repositories>
            <pluginRepositories>
                <pluginRepository>
                    <id>repo.jenkins-ci.org</id>
                    <url>http://repo.jenkins-ci.org/public/</url>
                </pluginRepository>
            </pluginRepositories>
        </profile>
    </profiles>
</settings>
```

1. create command
```
$ mvn -cpu hpi:create
```
or
```
$ mvn -cpu org.jenkins-ci.tools:maven-hpi-plugin:1.84:create
```

ref: https://blog.codecentric.de/en/2012/08/tutorial-create-a-jenkins-plugin-to-integrate-jenkins-and-nexus-repository/

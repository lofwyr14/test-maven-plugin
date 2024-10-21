# Test the maven-release-plugin

There is a bug https://issues.apache.org/jira/browse/MRELEASE-378

## How to reproduce

```
mvn release:prepare -DdryRun=true
```

The plugin should find the SNAPSHOT version in the pom.xml for 
```
org.apache.maven.shared:maven-shared-utils:3.4.3-SNAPSHOT
```
and should fail, or ask what to do.

It is a dependency of a plugin.

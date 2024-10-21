# Test the maven-release-plugin

There is a bug https://issues.apache.org/jira/browse/MRELEASE-378

## How to reproduce

```
mvn release:prepare -DdryRun=true
```
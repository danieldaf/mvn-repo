# Como integrar este 'repo' de maven temporal

```xml
<repositories>
  <repository>
    <id>mvn-repo</id>
    <url>https://raw.githubusercontent.com/danieldaf/mvn-repo/master</url>
    <releases>
      <enabled>true</enabled>
    </releases>
    <snapshots>
      <enabled>true</enabled>
    </snapshots>
  </repository>
</repositories>

<properties>
  <sobio-api-client.version>20220801.2d456c4</sobio-api-client.version>
</properties>

<dependencies>
  <dependency>
    <groupId>ar.com.sdc.sobio</groupId>
    <artifactId>sobio-api-client</artifactId>
    <version>${sobio-api-client.version}</version>
  </dependency>
</dependencies>
```

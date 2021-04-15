# Matrix API
Since the original repo didn't have any documentation, I've compiled what I've found in the source code here.

### Import with Maven
Replace {VERSION} with the latest release version
```xml
<repository>
            <id>jitpack.io</id>
            <url>https://jitpack.io</url>
        </repository>
<dependency>
            <groupId>com.github.CaledonianEH</groupId>
            <artifactId>matrix-api-repo</artifactId>
            <version>{VERSION}</version>
        </dependency>
```

### Set Matrix as a soft-depend
Matrix must be set as a soft depend to load in the correct order.
```yaml
name: YourPluginHere
version: 1.0
author: author
main: your.main.path.here

softdepend: [Matrix]
```

## How to use the API
This is just a basic overview of using the API. Note that some parts have broken due to not being updated

### Obtaining an instance
To obtain an instance of the API, use the line below. From here you can call the api using ```api```
```java
MatrixAPI api = MatrixAPIProvider.getAPI();
```

## Working HackType methods
Other methods have either been tested and proven to return null, or haven't yet been tested
```java
- HackType.VELOCITY
- HackType.AUTOBOT
- HackType.BADPACKETS
- HackType.BLOCK
- HackType.CHAT
- HackType.HITBOX
- HackType.INTERACT
- HackType.KILLAURA
- HackType.PHASE
```



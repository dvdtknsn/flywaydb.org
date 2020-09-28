---
layout: documentation
menu: configuration
pill: skipDefaultResolvers
subtitle: flyway.skipDefaultResolvers
---

# skipDefaultResolvers

## Description
Whether default built-in resolvers (sql and jdbc) should be skipped. If `true`, only [custom resolvers](/documentation/configuration/resolvers) are used.

## Default
false

## Usage

### Commandline
```
./flyway -skipDefaultResolvers="true" info
```

### Configuration File
```
flyway.skipDefaultResolvers=true
```

### Environment Variable
```
FLYWAY_SKIP_DEFAULT_RESOLVERS=true
```

### API
```
Flyway.configure()
    .skipDefaultResolvers(true)
    .load()
```

### Gradle
```
flyway {
    skipDefaultResolvers = true
}
```

### Maven
```
<configuration>
    <skipDefaultResolvers>true</skipDefaultResolvers>
</configuration>
```
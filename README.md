# WBR Parent POM

Opinionated Maven parent POM for WBR's Spring Boot microservices. Every child
module is expected to be a Spring Boot application.

## Provides

- Spring Boot Maven plugin wired on every child
- Dependency version management (Spring Boot + AWS SDK BOMs, `wbr-spring-boot-starter`)
- Build standards (Java 25, unit + integration test phases via Surefire/Failsafe)
- Code quality gates (JaCoCo coverage, Spotless/Palantir formatting, Checkstyle, SpotBugs, Enforcer)
- Publishing to the WBR Maven release/snapshot repositories

## Usage

Point a service's `pom.xml` at this parent:

```xml
<parent>
    <groupId>com.wbr</groupId>
    <artifactId>wbr-parent</artifactId>
    <version>1.0.0</version>
</parent>
```

---

Maintained by [WBR Technologies](https://wbrtechnologies.com).

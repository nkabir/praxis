## Configuration Management

Configuration is critical for distributed systems but is often an afterthought. Spring 3.1 introduces unified property management that address the issues of configuration nicely.

There are four capabilities that are available to configure a Java application:

* PropertySource
* Java-based Configuration classes
* Bean Definition Profiles
* SpringLDAP

Configuration requires a _bootstrap_ step in which a flag indicates the specific setup that is generated. Our environment is dictated by `runtime.context`. Some examples: `test`, `local`, `staging`, `staging.knyc`

The `runtime.context` indicates which LDAP server to contact for additional configuration details. When an application starts, it first checks the environment's `runtime.context`. It then loads an LDAP configuration based on that context.

[`fimero.core.spring`](https://bitbucket.org/nkabir/fimero-spring/) is a `maven2` project that demonstrates these capabilities.

## Bootstrap

The initial objects are configured via properties files that are loaded from the classpath. Currently, `/fimero` is the location for the properties files:

* `common-config.properties`
* `test-config.properties`
* `local-config.properties`
* `staging.knyc-config.properties`
* `production.knyc-config.properties`

![pojo image](http://dl.dropbox.com/u/59707331/praxis/spring-configuration/spring-properties.png)

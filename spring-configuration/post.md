## Configuration Management

Configuration is critical for distributed systems but is often an afterthought. Spring 3.1 introduces unified property management that address the issues of configuration nicely.

* PropertySource
* Java-based Configuration classes
* Bean Definition Profiles
* SpringLDAP

Configuration requires a _bootstrap_ step in which a flag indicates the specific setup that is generated. Our environment is dictated by `runtime.context`. Some examples: `test`, `local`, `staging`, `staging.knyc`

The `runtime.context` indicates which LDAP server to contact for additional configuration details.

`springx.configuration` is a sample project that demonstrates these capabilities.



How to reproduce the issue:

`mvn package -P openjfx-desktop`

If on Linux for example, let's install the generated debian package:

`sudo dpkg -i webfx-example-application-openjfx/target/javapackager/webfx-example_1.0.0.deb`

After successful installation, trying to run it:

`
webfx-example
`

It doesn't find the main class:

`
Error: Could not find or load main class dev.webfx.platform.shared.services.boot.ApplicationBooter
Caused by: java.lang.ClassNotFoundException: dev.webfx.platform.shared.services.boot.ApplicationBooter
`


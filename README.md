used 4 building and containerizing your applications. 
D.E acts as a client-server application with:

a server with a long-running daemon process dockerd
APIs which specify interfaces that programs can use to talk to and instruct the Docker daemon
a command line interface (CLI) client docker
the CLI uses Docker APIs to control or interact with the Docker daemon through scripting or direct CLI commands. (many other Docker applications use the underlying API and CLI). --> the daemon creates and manages Docker objects, such as images, containers, networks, and volumes.


will work on centOS platforms:
x86_64 / amd64 
arm64 / aarch64
ppc64le

will NOT work on centOS platforms: 
arm (32-bit)
s390x

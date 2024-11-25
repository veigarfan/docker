used 4 building and containerizing your applications. 
D.E acts as a client-server application with:

a server with a long-running daemon process dockerd
APIs which specify interfaces that programs can use to talk to and instruct the Docker daemon
a command line interface (CLI) client docker
the CLI uses Docker APIs to control or interact with the Docker daemon through scripting or direct CLI commands. (many other Docker applications use the underlying API and CLI). --> the daemon creates and manages Docker objects, such as images, containers, networks, and volumes.


will work on centOS platforms:
**x86_64 / amd64**,
**arm64 / aarch64**,
**ppc64le**

will NOT work on centOS platforms: 
**arm (32-bit)**,
**s390x**

# Prerequisites
## OS requirements
to install D.E, you need a maintained version of one of the following CentOS versions:
*CentOS 9 (stream)*
the ``` centos-extras ``` repository must be enabled. this repository is enabled by default. if you have disabled it, you need to re-enable it...........duh!!!!!!!!!

## Uninstall old versions
before you can install D.E, you need to uninstall any conflicting packages.

ur Linux distribution may provide unofficial Docker packages, which may conflict with the official packages provided by Docker. you must uninstall these packages before you install D.E.
```
sudo dnf remove docker \
                  docker-client \
                  docker-client-latest \
                  docker-common \
                  docker-latest \
                  docker-latest-logrotate \
                  docker-logrotate \
                  docker-engine
```
```dnf``` might report that you have none of these packages installed.

images, containers, volumes, and networks stored in ```/var/lib/docker/``` aren't automatically removed when you uninstall Docker.
## Installation methods
you can install D.E in different ways, depending on your needs:

> you can set up Docker's repositories and install from them, for ease of installation and upgrade tasks

> you can download the RPM package, install it manually, and manage upgrades completely manually. (this is useful in situations such as installing Docker on air-gapped systems with no access to the internet)

> in testing and development environments, you can use automated convenience scripts to install Docker (hahahaha)



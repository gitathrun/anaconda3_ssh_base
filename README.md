# Anaconda 3 Docker Image for Remote Docker on Remote Host Python development #

Author: Teng Fu
Contact: teng.fu@teleware.com

## AIM ##

Designed for Python development with VSC or PyCharm and the Python interpreter is located on Remote Docker Container on Remote VM host.

Essentially, the docker container run as SSH server with binding port on VM host, for example (9022:22), 9022 is the vm host port, 22 is the docker container's port.

Developer can access the docker container ssh service by accessing vm host's 9022 port (which is tunneled to container's port 22).

Then developer can use VSC's Remote - SSH or PyCharm's Remote interpreter feature for remote Python development.

Reference:

- [Anaconda dockerhub](https://hub.docker.com/r/continuumio/anaconda3/dockerfile)

- [Dockerize an SSH service](https://docs.docker.com/engine/examples/running_ssh_service/)

- [VSC Remote SSH setup](https://code.visualstudio.com/docs/remote/ssh)

- [PyCharm's remote interpreter](https://www.jetbrains.com/help/pycharm/using-docker-as-a-remote-interpreter.html#config-docker)
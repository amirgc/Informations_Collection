# Detached versus foreground mode

When you start a container you should be able to decide if you want your container to run in a detached mode or foreground mode. In detached mode, which is the default option, the container exits as soon as the root process that was used to run the container exits. For example, the following command can be used to run a container in detached mode:

    docker run -d microsoft/iis powershell
In foreground mode, when the -d option is not specified and with the -it flag the Docker daemon runs the container and attaches the console to the container's standard input, output, and error streams.

An example for this is as follows:

    docker run -it microsoft/iis powershell 

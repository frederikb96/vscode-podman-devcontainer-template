# VS Code Podman Devcontainer Template

You can use this template to create a development environment for your project using Podman and VS Code. It automatically mounts the Wayland socket and the X11 socket to allow GUI applications to run in the container. If you dont want this due to security reasons, you can remove the mounts and variables from the `devcontainer.json` file.

The container is supposed to be run as non-root Podman container, and it maps your current user to the ubuntu user in the container to support file permissions on the mounted volumes well.

## Mounts
There is already an example mount for the `.bash_history` file in the `devcontainer.json` file. You can add more mounts as needed.
Create this file if you use it:
```bash
mkdir -p container
touch container/.bash_history
```

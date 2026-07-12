# Dev Box Image Definitions

Microsoft Dev Box [team customization](https://learn.microsoft.com/azure/dev-box/how-to-customize-dev-box-setup-tasks) image definitions. Each subfolder contains an `imagedefinition.yaml` that a Dev Center catalog picks up to build a customized dev box image.

## Definitions

- [`aliya-devbox`](aliya-devbox/imagedefinition.yaml): Visual Studio 2026 (Community, with the ASP.NET/web and .NET MAUI workloads), Visual Studio Code, Node.js LTS, and Rancher Desktop on a WSL2 backend.

### Containers: Rancher Desktop, not Docker Desktop

`aliya-devbox` installs **Rancher Desktop** (`SUSE.RancherDesktop`) and enables **WSL2** as its backend. Rancher Desktop provides the container engine and a Docker-compatible CLI, so **Docker Desktop is intentionally not installed**.

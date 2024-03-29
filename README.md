# k8s-labtop
scripts to setup a local k8s lab on the laptop

# tasks install
`sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin`

# examples task file usage
basic cluster:
`task cluster-create-basic`
cluster with cilum enterprise:
`task cluster-create-cilium-enterprise`
argocd rollouts demo:
`task demo-argo-rollouts-blue-green`

## Rebuild WSL kernel for Cilium enterprise on windows

a script for this can be found here:  
`https://raw.githubusercontent.com/martijnvdp/bash-code-snippets/main/wsl2/build-wsl2-kernel.sh`
sources: `https://github.com/microsoft/WSL2-Linux-Kernel/releases`

to download and run the script, open a wsl ubuntu terminal and copy this line:
```
curl https://raw.githubusercontent.com/martijnvdp/bash-code-snippets/main/wsl2/build-wsl2-kernel.sh -o ./build-wsl-kernel.sh && sudo chmod +x ./build-wsl-kernel.sh && sudo ./build-wsl-kernel.sh
```
and check with  `uname -r` the version , should have cilium at the end

# refs
- https://nip.io/
- https://taskfile.dev/usage/
- https://github.com/go-task/task
- https://wsl.dev/wslcilium/
- https://harthoover.com/compiling-your-own-wsl2-kernel/
- https://kind.sigs.k8s.io/docs/user/using-wsl2/
- https://docs.cilium.io/en/stable/operations/system_requirements/#linux-kernel

# k8s-labtop
scripts to setup a local k8s lab on the laptop

# tasks install
`sh -c "$(curl --location https://taskfile.dev/install.sh)" -- -d -b /usr/local/bin`

# example task file usage
task cluster-create-basic
task demo-argo-rollouts-blue-green
# refs
https://nip.io/
https://taskfile.dev/usage/
https://github.com/go-task/task

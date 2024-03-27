# Argo rollouts blue green demo

deploy the demo:
`kubectl apply -f demos\argo-rollouts\blue-green`
open a web browser 

# prod
http://blue-green.dev.127.0.0.1.nip.io/

# preview
http://blue-green-preview.dev.127.0.0.1.nip.io

keep both preview and prod open 

open the argo rollouts dashboard:
http://argo-rollouts.127.0.0.1.nip.io

- switch to demo ns: demos-argo-rollouts-bluegreen
- change the color to green
- check the preview page
- promote to production

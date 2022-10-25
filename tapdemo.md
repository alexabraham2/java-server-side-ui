

Developer - Download code from Accelerator, Build it locally, test and checkin the code.

Operators - Run the workload yaml to trigger the supply chain associated with the project

Security - Will able to review the scanned result from TAP UI


































k api-resources --api-group carto.run


k get workloads.carto.run server-side-ui-starter -n my-apps -o yaml | yq  

#Operator perspective : Supply Chain and Resource Templates

Cartographer giver operator few different objects to work with. Supply chain chains together a series of activity
kubectl tree deliverable gitops

k get clustersupplychain -A
k get clustersupplychain scanning-image-scan-to-url -o yaml | yq 'del(.metadata)'








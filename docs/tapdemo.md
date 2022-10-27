














Run Spring Application

- ./mvnw clean compile
- ./mvnw verify
- ./mvnw spring-boot:run


Apply Workload

- tanzu apps workload apply \
  --file config/workload.yaml \
  --namespace my-apps --source-image aatapdemocr.azurecr.io/my-project/build-service/my-project/build-service/java-server-side-ui \
  --local-path . \
  --yes \
  --tail

















k api-resources --api-group carto.run


k get workloads.carto.run server-side-ui-starter -n my-apps -o yaml | yq  

#Operator perspective : Supply Chain and Resource Templates

Cartographer giver operator few different objects to work with. Supply chain chains together a series of activity
kubectl tree deliverable gitops

k get clustersupplychain -A
k get clustersupplychain source-test-scan-to-url -o yaml | yq 'del(.metadata)'








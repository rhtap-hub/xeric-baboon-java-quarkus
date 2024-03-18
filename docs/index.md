# Trusted Application Pipeline Software Template

This application, **xeric-baboon-java-quarkus**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/rhtap-hub/xeric-baboon-java-quarkus ](https://github.com/rhtap-hub/xeric-baboon-java-quarkus ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/rhtap-hub/xeric-baboon-java-quarkus-gitops ](https://github.com/rhtap-hub/xeric-baboon-java-quarkus-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |   
| **rhtap-e2e-demo-development** | The default application during development. Every build will be deployed to this namespace for testing. | 
| **rhtap-e2e-demo-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/rhtap-hub/xeric-baboon-java-quarkus-gitops ) in the components/xeric-baboon-java-quarkus/overlays/prod directory |  
| **rhtap-e2e-demo-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/rhtap-hub/xeric-baboon-java-quarkus-gitops ) in the components/xeric-baboon-java-quarkus/overlays/prod directory | 
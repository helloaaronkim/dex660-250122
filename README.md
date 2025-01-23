# dex660-250122

## Account information
* org id : fb73ebd1-ee34-42a5-86fe-8e98b1bdc39b
* client id : aac68afaee124b3db77324f26d3c53a2
* client secret : D0f62d39d837410C911669124D676233

## Connected Apps information
* Exchange Viewer
  * client id : 120410a7c15940f4b155d7c1c0db5ecc
  * client secret : a7F79Be259E9469f85F4f51F0f62F5aB

* Exchange Contributor
  * client id : 65a864b66f1e4a79b6e308ebbb1b78ae
  * client secret : 10F2Ca0547D84E01AfF1B0CE3a24af07
  
* CloudHub Deployment
  * client id : f4f40a9e1e40439994434fb8aa232eda
  * client secret : 00918B2EF4d6471f88c7197B07b4727f

## cmd

```
// dev
mvn -DmuleDeploy deploy -Dap.client_id=aac68afaee124b3db77324f26d3c53a2 -Dap.client_secret=D0f62d39d837410C911669124D676233 -Dap.ca.client_id=f4f40a9e1e40439994434fb8aa232eda -Dap.ca.client_secret=00918B2EF4d6471f88c7197B07b4727f -Dencrypt.key=secure12345 -Ddeployment.env=dev


// stg
mvn -DmuleDeploy deploy -Dap.client_id=aac68afaee124b3db77324f26d3c53a2 -Dap.client_secret=D0f62d39d837410C911669124D676233 -Dap.ca.client_id=f4f40a9e1e40439994434fb8aa232eda -Dap.ca.client_secret=00918B2EF4d6471f88c7197B07b4727f -Dencrypt.key=secure12345 -Ddeployment.env=stg

// prod
mvn -DmuleDeploy deploy -Dap.client_id=aac68afaee124b3db77324f26d3c53a2 -Dap.client_secret=D0f62d39d837410C911669124D676233 -Dap.ca.client_id=f4f40a9e1e40439994434fb8aa232eda -Dap.ca.client_secret=00918B2EF4d6471f88c7197B07b4727f -Dencrypt.key=secure12345 -Ddeployment.env=prod -Ddeployment.suffix=
```
# k8s-crd-example
This is an example of Kurbernetes Custom Resource Definition for the article written in marcosflobo.com

Here, to can find the [crd.yaml](crd.yaml) and the [example.yaml](example.yaml) which is an object from the previous definition.

Moreover, you can find the instructions to deploy both objects just below

## Deployment
### Deploy CRD
```shell
kubectl apply -f crd.yaml
```
And you will see
```shell
customresourcedefinition.apiextensions.k8s.io/kafkatopics.marcosflobo.com created
```

### Deploy the example
```shell
kubectl apply -f example.yaml
```
And you will see
```shell
kafkatopic.marcosflobo.com/mykafkatopic created
```

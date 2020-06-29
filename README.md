

## Pre-requistes

1. Install Golang `brew install golang` and check version `go version`

2. Check if you have access to kubernetes cluster, else create one.

3. If the kubernetes server version is `>=1.16.0` then we can create `v1` api's for CRD's and controllers.
If not we will have to use `v1beta1` and `v1alpha1` respectively.

4. Install an IDE for faster and better code development. `GOLAND` by jetbrains. Everyone should have access to
this if they have a jetbrains account.

5. Install kustomize `brew install kustomize`


## Steps to create an operator.

- Create a scaffold for the project using the `kubebuilder` command.

- Create API's and controllers.
	
	`kubebuilder create api --group webapp --kind MyWatchlist --version`
	

## References

-

- [Openshift operator sdk tutorial](https://learn.openshift.com/operatorframework/go-operator-podset/)
- [Kustomize Github](https://github.com/kubernetes-sigs/kustomize)
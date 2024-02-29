# What is this
Small kubernetes config for my small barely-working Phoenix LiveView todo list.
Ready to be started in minikube.


# Install and run
1. Ensure you have [minikube](https://minikube.sigs.k8s.io/docs/start/) installed
2. Add  `127.0.0.1 checklister.info` to your `/etc/hosts` file
3. Enable ingress and metrics-server addons for minikube:
```bash
minikube addons enable metrics-server
minikube addons enable ingress
```
4. Start app:
```bash
kubectl apply -f .
```
5. Start ingress tunnel:
```bash
minikube tunnel
```
6. Ensure app is (barely) working on [http://checklister.info/checklists](http://checklister.info/checklists)


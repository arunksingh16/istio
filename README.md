# istio
Repository for Istio deployment and testing

Using pipenv in Mac
```
python3 -m pipenv install 
```

### Istioctl Setup

```
curl -L https://istio.io/downloadIstio | sh -
cd istio-*
export PATH=$PWD/bin:$PATH
```
### Istio deployement and profile setup
Instio profile https://istio.io/latest/docs/setup/additional-setup/config-profiles/

```
istioctl install --set profile=demo -y
istioctl profile dump
kubectl label namespace default istio-injection=enabled

```

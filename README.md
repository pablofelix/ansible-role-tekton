# How to use tekton role
# ======================

 This role installs Tekton Pipelines, Tekton Triggers and Tekton Dashboard on a Openshift cluster.

## Requirements
1- Optional - install venv
```
pip install virtualenv
python3 -m virtualenv venv
```
2- Install python dependencies

```
pip install -r requirements.txt
```
3- Install ansible galaxy dependencies

ansible-galaxy install dependencies
```
 ansible-galaxy collection install community.kubernetes
```
4- Connect to openshift cluster

```
oc login -u <username> -p <password> <cluster-url>
```
5- Export kubeconfig

```
export KUBECONFIG=<path-to-kubeconfig>
```

## Execute role
```
cd tekton
```

```
molecule test 
```

# Mission 2- Install openldap on k8s and authenticate users with website. (not fully working)

This project is a mission2 for nir's bootcamp.
In this repository you will find a github porject with called "onther-ldap" that deploy ldap auth website to k8s cluster.

## Installation:
1. Cread K8s cluster in GCloud/Aws/MiniKube.
2. Install openldap with this command: " helm install my-openldap-stack-ha helm-openldap/openldap-stack-ha --version 4.0.2 "
3. Use the Kubectl port-forward commmand to forward phpldapadmin port to your computer.
4. Login to your openldap from your phpldapadmin website.
5. Create users.
6. Inside another ldap folder configure the files inside the kubernetes folder (config-map.yaml, secret.yaml, ingress.yaml) 
7. Run the command " Kubectl apply -f kubernetes/ ".
8. Use the command " Kubectl port-forward " to forward another-ldap website to your computer.
9. Test the ldap authentication from the browser.
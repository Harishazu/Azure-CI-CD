# Azure-CI-CD

Implementing Continuous Integration (CI)

A front-end web app in Python which lets you vote between two options

A Redis which collects new votes

A .NET worker which consumes votes and stores them

A Postgres database backed by a Docker volume

A Node.js web app which shows the results of the voting in real time

![image](https://github.com/user-attachments/assets/5312bf3a-87e7-41b8-ad1a-a86c63a9a152)





STEP 1  :  Source code is in Github 

   Migrating them to Azure repos via Clone > 
   Click on  Azure repos > Import a repository
    It will import the repository  
    Then we need to change the branch to main and set it as default

   Branches> Select the main branch 


















CONTINUOS DELIVERY 

az aks get-credentials --name azuredevops --resource-group azuredevopsda

Setting up Kubernetes and ARGOCD

Installing argocd
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

kubectl get pods -n argocd
Kubectl get secrets -n argocd
kubectl get secrets -n argocd
kubectl edit secret argocd-initial-admin-secret -n argocd



$base64String = "NjF2QTR0bWZtQVF5VThSbQ=="
$decodedBytes = [System.Convert]::FromBase64String($base64String)
$decodedString = [System.Text.Encoding]::UTF8.GetString($decodedBytes)
echo $decodedString

 To access the argocd server
kubectl get svc -n argocd

It is in cluster mode need to change it to node port mode
kubectl edit svc argocd-server -n argocd

Save it to nodeport 
get the port number

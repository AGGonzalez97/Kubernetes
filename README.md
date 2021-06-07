# Kubernetes
Para realizar esta práctica se han seguido los siguientes pasos:

# 1.- Crear regla en el firewall para abrir los puertos del 5000 al 31001
![20](https://user-images.githubusercontent.com/29304115/121077099-7cc34480-c7d7-11eb-9d51-255ed716206c.PNG)

# 2.- Crear clúster y entrar en Cloud Shell
![20-1](https://user-images.githubusercontent.com/29304115/121077396-dcb9eb00-c7d7-11eb-8a36-ec04e5a003b1.PNG)
![20-2](https://user-images.githubusercontent.com/29304115/121077402-ddeb1800-c7d7-11eb-8ab3-2ebb63b48452.PNG)

# 3.- Ejecutar los siguientes comandos dentro de la consola
### git clone https://github.com/jluisalvarez/k8s-vote-app
### cd k8s-vote-app
### nano vote-service.yaml (Cambiar NodePort por LoadBalancer)  
### nano result-service.yaml (Cambiar NodePort por LoadBalancer)
![21](https://user-images.githubusercontent.com/29304115/121077776-54881580-c7d8-11eb-9951-1fb14228fefd.PNG)
### kubectl apply -f . 
### kubectl get services (ip externas)
![21-2](https://user-images.githubusercontent.com/29304115/121077877-7bdee280-c7d8-11eb-8b23-ebc57498058a.PNG)


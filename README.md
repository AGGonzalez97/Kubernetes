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

# 4.- Comprobar que las ips funcionan
### Result -> Ip: 35.222.45.196:5001 
![21-2](https://user-images.githubusercontent.com/29304115/121078117-cfe9c700-c7d8-11eb-9b83-30f5c5a717d3.PNG)
### Vote -> Ip: 34.70.152.251:5000
![23](https://user-images.githubusercontent.com/29304115/121078183-e5f78780-c7d8-11eb-8a45-16f46e10cf60.PNG)
### Volvemos a Result para comprobar que se ha actualizado la votación
![24](https://user-images.githubusercontent.com/29304115/121078234-f60f6700-c7d8-11eb-864e-17479ab6d036.PNG)

# 5.- Cambiar el número de nodos de 3 (default) a 5
![25](https://user-images.githubusercontent.com/29304115/121078330-1c350700-c7d9-11eb-9f67-b141409ff5ad.PNG)

# 6.- Escalar cluster a 2 resplicas
![26](https://user-images.githubusercontent.com/29304115/121078401-353db800-c7d9-11eb-8982-cb430a8f5f97.PNG)

# 7.- Actualizar la imagen de postgres
![27](https://user-images.githubusercontent.com/29304115/121078473-4e466900-c7d9-11eb-9a13-979f450ad4fc.PNG)



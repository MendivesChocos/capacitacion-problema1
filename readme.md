# para construir imagen
docker build -t "mendives64/orbis-training-docker" .          
# para taggear imagen
docker tag 7db9c916bc4e mendives64/orbis-training-docker:0.1.0 

# comando subir la imagen al dockerhub
docker push mendives64/orbis-training-docker:0.1.0

# Comando para correr contenedor
docker run -it mendives64/orbis-training-docker:0.5.0 bash
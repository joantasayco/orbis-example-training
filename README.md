#Paso 3

1. Descargar el proyecto de bitbucket https://bitbucket.org/orbisunt/orbis-example-training/src/master/
2. Creamos repositorio GitHub con el mismo nombre del repositorio BitBucket
3. Enlazamos con el repositorio remoto con la instruccion git remote add origin git@github.com:joantasayco/orbis-example-training.git
4. Subir los cambios al repositorio remoto GitHub 
   git add .
   git commit -m "Feat....."
   git push origin master

5. Identificamos el archivo pesado
   git gc
   git verify-pack -v .git/objects/pack/pack-e6ff07a6e715cb01009ca282963174099f2b72ec.idx
   git rev-list --objects --all
   git rev-list --objects --all | grep 2ce5eca830c1f68c365b5323677e7c37212eccf6
   git rm 1_tSyuv3ZRCfsSD5aXB7v8DQ.png
   git status
   git add .
   git commit -m "Feat Eliminando archivo mas pesado"
   git push origin master

   



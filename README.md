# Prueba Modulo 4

Este repositorio contiene los archivos para completar el desafio del curso de DevOps de Desafio Latam

El desafio consistian en generar el deployment de un sitio web estaticos a un bucket S3 de aws, el cual debe estar gestionado globalmente con CloudFront, este deployment debe estar automatizado mediante Github acctions, el cual debe realizarse cada vez que se hace un pull request a la rama main

El desafio debe contar con los siguientes elementos

1. Crear un sitio web estatico
    - Minimo un index.html y un error.html  

2. Crear un repositorio de github
    - Configurar ramas para manejar los cambios

3. Configuracion de AWS S3
    - Configurar un bucket S3 para almacenar el sitio wwb
    - Configurar las politicas de acceso publico o usar OAI si es un bucket privado

4. Configuracion de Amazon CloudFront 
    - Configurar una distribucion de Cloudfront con el bucket s3 como origen

5. Automatizar con Github Actions
    - Crear un workflow de github action que:
        - Compile (si aplica)  y valide los archivos del sitio
        - Suba los archivos al bucket s3 cada vez que se haga una cambio en la rama main
        - invalide el Cache de CloudFront tras el despliege

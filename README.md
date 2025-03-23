Primera Fase del Proyecto de Catedra de Desarrollo de Aplicacion web con software interpretado en el Servidor.

Enunciado del problema:
La cooperativa “ACOEMPRENDEDORES” es una financiera que pretende trabajar con los emprendedores y
empresarios locales de nuestro país. Requieren de un Sistema de Información que le permita realizar las siguientes
funciones:Registro de empleados,Registro de clientes,Registro de productosfinancieros,Registro de transacciones de producto,Cartera virtual del cliente,Control de usuario.

----------------------------------------------------------------------------------------------------------------------

Tabla de Contenidos

-Integrantes

-Link a Notion

-Licinecia Creative Commons

-Proceso de Cierre

-------------------------------------------------------------------------------------------------

Integrantes

Nombres de los participantes con Usuarios de GitHub

Chavarria Velasquez, Manuel Alejandro - CV211229 GitHub (CV211229)

Aguilar Cruz, Joel Ernesto - AC223047 GitHub (AC223047)

Gudiel Magaña, Emerson Alexander – GM171814 GitHub (emersongudiel98)

Rodrigo Ernesto Escobar Rivas - ER222434 GitHub (XxRdorixX)

Ricardo Daniel Guevara Avelar - GA242652 GuitHub (RDGuevaraA)

---------------------------------------------------------------------------------------------------

Link de Notion

https://www.notion.so/1bd66c5b5b1f8032bf1acfb81285599a?v=1bd66c5b5b1f8050b642000ce46872a3&pvs=4

-----------------------------------------------------------------------------------------------------------

Licinecia Creative Commons

Se utilizó una licencia como una 
Creative Commons Reconocimiento-NoComercial-CompartirIgual 4.0 Internacional.

Link de la licencia:
https://creativecommons.org/licenses/by-nc-sa/4.0/

-----------------------------------------------------------------------------------------------------------------------

Proceso de Cierre

Paso 1: Iniciar Minikube

(minikube start) Inicia Minikube y crea un clúster Kubernetes local.

------------------------------------------------------------------------------------------------------------------------

Paso 2: Verificar el Estado de Minikube

(minikube status) Verifica el estado de Minikube y su configuración.

----------------------------------------------------------------------------------------------------------------------------

Paso 3: Configurar Docker

(minikube docker-env | Invoke-Expression (Windows PowerShell)) Configura Docker para usar el demonio Docker interno de Minikube en lugar del sistema anfitrión.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Paso 4: Construir la Imagen Docker

(docker build -t docker-php-entrypoi:latest .) Construye una imagen Docker a partir del Dockerfile en el directorio actual y la etiqueta como (docker-php-entrypoi:latest.)

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Paso 5: Listar Imágenes Docker

(docker images) Lista las imágenes Docker disponibles en el sistema.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Paso 6: Aplicar Manifiestos Kubernetes

(kubectl apply -f k8s/) Aplica los manifiestos Kubernetes contenidos en la carpeta (k8s/) para desplegar la aplicación.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Verificación del Despliegue

(kubectl get deployments) Lista los deployments en el clúster.

(kubectl get pods) Muestra los pods en ejecución en Kubernetes.

(kubectl get svc) Lista los servicios en el clúster Kubernetes.

(kubectl get hpa) Muestra las configuraciones de escalado automático horizontal de pods (HPA, Horizontal Pod Autoscaler).

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Acceso al Servicio

(minikube service docker-web-service --url) Obtiene la URL para acceder al servicio (docker-web-service) expuesto por Minikube.






# Plataforma Web IMCUFIDE: Implementación con Arquitectura de Contenedores

**Universidad Autónoma del Estado de México | Facultad de Ingeniería**
**Asignatura:** Tecnologías Computacionales I (2025-B)

Este proyecto consiste en el diseño y desarrollo de una plataforma web integral para el **Instituto Municipal de Cultura Física y Deporte (IMCUFIDE)** de Tenango del Valle. El sistema centraliza la gestión de ligas deportivas, automatiza la consulta de calendarios y resultados, y provee un canal de comunicación oficial para la ciudadanía.

---

## 🌐 1. Acceso a la Plataforma en Producción
El proyecto se encuentra desplegado y totalmente operativo. Puedes acceder a la versión pública a través del siguiente enlace:

### 🔗 **[https://imcufide-proyecto.vercel.app/](https://imcufide-proyecto.vercel.app/)**

> **Nota:** El Frontend está alojado en Vercel y el Backend en Render. Debido a las limitaciones de la capa gratuita de Render, es posible que la primera petición tarde unos segundos en responder (*cold start*).

---

## 🚀 2. Instrucciones de Despliegue Local (Docker)
Para replicar el entorno de producción en tu máquina local asegurando la paridad de entornos, utilizamos **Docker** y **Docker Compose**.

Sigue estos pasos en tu terminal para levantar el Frontend, Backend y Base de Datos automáticamente:

### Prerrequisitos
* Tener instalado [Docker Desktop](https://www.docker.com/products/docker-desktop) y Git.

### Pasos de Ejecución

**1. Clonar el repositorio:**
```bash
git clone [https://github.com/WiliEsquivel/imcufide-proyecto-main.git](https://github.com/WiliEsquivel/imcufide-proyecto-main.git)
````

**2. Acceder al directorio del proyecto:**

```bash
cd imcufide-proyecto
```

**3. Iniciar los servicios:**
Ejecuta el siguiente comando para construir las imágenes y levantar los contenedores:

```bash
docker-compose up --build
```

Una vez finalizado el proceso, podrás acceder localmente a los servicios (usualmente en `http://localhost:5173` para el frontend y `http://localhost:8000` para la API, dependiendo de tu configuración en el `docker-compose.yml`).

-----

## 🛠️ Arquitectura y Tecnologías

El sistema utiliza una arquitectura de software moderna y desacoplada en tres capas, containerizada para garantizar portabilidad y escalabilidad.

### **Frontend (Cliente)**

  * **Tecnologías:** Vue.js + Vite.
  * **Función:** Interfaz de usuario reactiva, SPA (Single Page Application) y diseño responsivo.

### **Backend (API)**

  * **Tecnologías:** Python + FastAPI.
  * **Función:** API RESTful de alto rendimiento, validación de datos con Pydantic y documentación automática (Swagger/ReDoc).

### **Base de Datos (Persistencia)**

  * **Tecnologías:** PostgreSQL + Supabase.
  * **Función:** Modelo relacional normalizado para gestionar deportes, categorías, equipos, partidos y resultados.

### **Infraestructura**

  * **Docker:** Containerización de servicios.
  * **Docker Compose:** Orquestación de contenedores para desarrollo local.

-----

## 🎯 Objetivo del Proyecto

Resolver la fragmentación de información y la ineficiencia operativa del IMCUFIDE mediante la digitalización de sus procesos.

  * **Gestión:** Administración centralizada de torneos (Fútbol, Básquetbol, Voleibol).
  * **Automatización:** Generación dinámica de tablas de posiciones y calendarios.
  * **Transparencia:** Información accesible en tiempo real para atletas y ciudadanos.

-----

## 👥 Autores

Proyecto elaborado por:

  * **Luis Antonio Ceballos Arriaga**
  * **Wilibaldo Esquivel Diaz**
  * **Edgar Germain Gonzalez Suarez**

**Docente:** Dr. Jose Antonio Hernández Servin

```
```

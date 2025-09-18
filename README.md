# 🚗🏍️🔧 MotorPoint - Aplicativo web de Repuestos y Accesorios para Autos y Motos

## 📖 Descripción del Proyecto
**Descripción General**  
MotorPoint es una aplicación web diseñada para facilitar el acceso a repuestos y accesorios de **autos y motos**.  
El objetivo principal es ofrecer un catálogo digital de productos, organizado y accesible, que permita a los usuarios encontrar de manera rápida lo que necesitan y a los administradores mantener la información actualizada.  

El sistema considera dos roles principales:  

**Usuario:**  
- Navegar el catálogo de productos.  
- Buscar productos por nombre o categoría.  
- Visualizar información detallada (nombre, descripción, precio e imagen).  
- Agregar o quitar productos de un carrito de compras.  
- Confirmar el pedido a través de una solicitud de cotización.  

**Administrador:**  
- Gestión de productos (crear, editar, eliminar y listar).  
- Gestión de categorías de productos.  
- Administración de usuarios registrados.  
- Revisión de solicitudes de cotización generadas por los clientes.  
- Generación de reportes básicos sobre el uso del sistema.

---
## 💻Tecnologías Utilizadas
- **Backend:**
  * Spring Boot
  * Maven:
     * Spring Web → Para construir APIs REST
     * Spring Security → Para autenticación y autorización
     * Spring Data JPA → Para acceso a base de datos con Hibernate
     * MySQL Driver → Para conectarse a la base de datos MySQL
     * Validation → Para validar datos de entrada
     * Spring Boot DevTools → Para recarga automática en desarrollo
     * Lombok → Para evitar escribir código repetitivo
- **Frontend:**
   * React
   * Bootstrap 
- **Base de datos:** MySQL  
- **Seguridad:** Spring Security + JWT (roles y autenticación)   
- **Control de versiones:** Git + GitHub

---
## 🔌Instalación y Ejecución
A continuación se muestran los pasos para instalar y ejecutar el proyecto de forma local, con las mismas acciones realizadas durante las pruebas. .  

### **1. Requisitos Previos**
Antes de iniciar, asegúrate de tener instalado:
- Git → para clonar el repositorio.
- Java 17+ y Maven → para el backend (Spring Boot).
- Node.js 16+ y npm → para el frontend (React).
- MySQL Server funcionando en tu máquina.
- Opcional el Postman para probar APIs.
  
### **2. Inicializar Git en el equipo**
En la carpeta destinada al proyecto, se preparó el entorno de Git ejecutando:
```bash
git init
```
<img width="597" height="95" alt="image" src="https://github.com/user-attachments/assets/bbb82e4a-d228-401a-afb7-0d6acb79a8fd" />

### **3. Clonar el repositorio**
Luego, se descargó el proyecto desde GitHub dentro de la carpeta inicializada:
```bash
git clone https://github.com/usuario/motorpoint.git
cd motorpoint
```
<img width="771" height="260" alt="image" src="https://github.com/user-attachments/assets/90d4a4a3-17e0-4a28-98e3-d54818361464" />

### **4. Configuración del Backend**
- Crear una base de datos en MySQL, por ejemplo:
```bash
CREATE DATABASE motorpoint_db;
```

- Editar el archivo `backend/src/main/resources/application.properties` con tus credenciales:
```bash
spring.datasource.url=jdbc:mysql://localhost:8080/motorpoint_db
spring.datasource.username=tu_usuario
spring.datasource.password=tu_password
```

- Iniciar el backend: 
```bash
   cd backend
   mvn spring-boot:run
 ```

### **5. Configuración del Frontend**
- Instalar dependencias:
```bash
cd frontend
npm install
```

- Iniciar el frontend:
```bash
npm start
```

---
## 📋 Roles
| Nombre           | Rol          | Funciones                                              |  
|------------------|--------------|--------------------------------------------------------|  
| Ashlee Maldonado | Full Stack   | - Creación de pantallas y componentes reutilizables.<br>- Apoyo en la lógica interna del sistema.<br>- Elaboración de la documentación del proyecto.              | 
| Angely Corahua   | Full Stack   | - Diseño visual y organización de interfaces.<br>- Manejo de datos mostrados al usuario.<br>- Revisión y validación de formularios.                               |  
| Bruno Guerra     | Full Stack   | - Desarrollo de reglas y procesos internos del sistema.<br>- Configuración de seguridad y accesos.<br>- Administración del repositorio y despliegue del proyecto. |  

---
## 🌱 Flujo de trabajo con Git

### **1. Ramas utilizadas**
- **main** → Rama estable, lista para producción.  
- **develop-nombre** → Rama de desarrollo.  
- **feature/nombre** → Nuevas funcionalidades.  
- **fix/nombre** → Correcciones de errores.  

#### Ejemplo
```bash
git checkout -b feature/catalogo-productos
```
<img width="955" height="222" alt="image" src="https://github.com/user-attachments/assets/b3b1e97e-16f9-467f-be56-d70f5e9a3124" />

#### Ejemplo 
```bash
git checkout -b fix/readme-conflict
```
<img width="600" height="58" alt="image" src="https://github.com/user-attachments/assets/c36a26de-89e0-4f0a-a172-1e07fecf60df" />


### **2. Commits**
- Commits atómicos y descriptivos.
```bash
git commit -m "feat: crear componente Login en React"
git commit -m "fix: resolver conflicto en README.md"
```

### **3. Uso de comandos Git**

Durante el desarrollo del **login** se documentaron los siguientes comandos:

---

🔄 **Restaurar archivos**
```bash
git restore src/components/Login.jsx
```
📌 Por qué: Cuando se modificó accidentalmente el componente Login.jsx y fue necesario volver al estado previo sin perder el resto de los cambios.

⏪ **Resetear cambios**
```bash
git reset --soft HEAD~1
```
🔀 **Cambiar de ramas**
```bash
git switch develop
```
📌 Por qué: Al pasar del desarrollo de la nueva feature login hacia la rama de integración develop.

### **4. Pull Request (PR) / Merge Request (MR)**

- Se generó una Pull Request desde **fix/readme-conflict** hacia **main**.

- Descripción clara del cambio.

- Checklist de revisión.

- Revisión y aprobación antes de hacer merge.

<img width="1600" height="688" alt="image" src="https://github.com/user-attachments/assets/fbe2a743-d9b7-48b5-88f4-7ac95d34de71" />

<img width="1286" height="741" alt="image" src="https://github.com/user-attachments/assets/0431419e-71aa-444d-9cae-c37e5433bc51" />

### **5. Resolución de Conflictos Ejemplo:**

Al intentar actualizar la rama **main** con los cambios remotos, se generó un conflicto en el archivo:

`README.md`

```diff
<<<<<<< HEAD
# MotorPoint - Sistema de Repuestos y Accesorios para Autos y Motos 
=======
# 🚗🏍️🔧 MotorPoint - Aplicativo web de Repuestos y Accesorios para Autos y Motos
>>>>>>> origin/main
```
✅ Solución: Se unificaron los cambios y se mantuvo la versión más completa y descriptiva:
```diff
# 🚗🏍️🔧 MotorPoint - Aplicativo web de Repuestos y Accesorios para Autos y Motos  

## 📖 Descripción del Proyecto
**Descripción General**  
MotorPoint es una aplicación web diseñada para facilitar el acceso a repuestos y accesorios de **autos y motos**.  
El objetivo principal es ofrecer un catálogo digital de productos, organizado y accesible, que permita a los usuarios encontrar de manera rápida lo que necesitan y a los administradores mantener la información actualizada.  

El sistema considera dos roles principales: **Usuario** y **Administrador** 🚀
```
### **6. Historial de commits (puntos de control)**
### Ejemplo de salida:
```bash
git log
```
### Muestra:
<img width="1278" height="1013" alt="image" src="https://github.com/user-attachments/assets/37bda904-30ba-4d1e-9e5d-9c09ec98c747" />

<img width="1304" height="953" alt="image" src="https://github.com/user-attachments/assets/e57c23d2-9f6e-44e4-8c8d-eecafdb33e61" />

### **7. Historial de cabeceras**
```bash
git reflog
```
<img width="1570" height="547" alt="image" src="https://github.com/user-attachments/assets/fed76798-5ddb-403a-b6cd-a28ea3dcadc8" />

### 🧩 Estructura de backend
### 🧩 Estructura del Frontend


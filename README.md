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
- **Estilos:** Bootstrap 
- **Control de versiones:** Git + GitHub

---
## 🔌Instalación y Ejecución
A continuación se muestran los pasos para instalar y ejecutar el proyecto de forma local, con las mismas acciones realizadas durante las pruebas. .  

### **1. Requisitos Previos**
- Git (clonar el repositorio).
- Java 17+.
- Maven (o usar el wrapper ./mvnw incluido).
- Node.js 16+ y npm.
- MySQL funcionando localmente.
- (Opcional) Postman o curl para probar APIs.
  
### **2. Inicializar Git en el equipo**
Lo primero es preparar la carpeta para trabajar con Git, usando:
```bash
git init
```
<img width="597" height="95" alt="image" src="https://github.com/user-attachments/assets/bbb82e4a-d228-401a-afb7-0d6acb79a8fd" />

### **3. Clonar el repositorio**
Luego descargamos el proyecto desde GitHub dentro de la carpeta inicializada, usando:
```bash
git clone https://github.com/usuario/motorpoint.git
cd motorpoint
```
<img width="771" height="260" alt="image" src="https://github.com/user-attachments/assets/90d4a4a3-17e0-4a28-98e3-d54818361464" />

### **4. Crear y moverse a la rama de trabajo**
Cada integrante trabajó en su propia rama de desarrollo, ejemplo:
```bash
git checkout -b develop-Angely
```
<img width="801" height="139" alt="image" src="https://github.com/user-attachments/assets/e74c92c4-254e-4443-8fb4-d1799cdcb8ba" />

### **5. Hacer cambios y guardar (commit)**
Una vez que cada integrante avanzaba en sus tareas, los cambios se guardaban con:
```bash
git add .
git commit -m "Descripción breve de los cambios realizados"
```
<img width="1280" height="667" alt="image" src="https://github.com/user-attachments/assets/7e59ef9b-ff8f-4946-b16a-1400c795c0b4" />

### **6. Creación de ramas adicionales para correcciones**
En algunos casos fue necesario crear ramas específicas para solucionar errores puntuales, por ejemplo:
```bash
git checkout -b fix/frontend-login
```
<img width="1175" height="158" alt="image" src="https://github.com/user-attachments/assets/e3d681c4-9d71-484b-ba30-32befcca37eb" />

### **7. Subir los cambios a GitHub**
Una vez confirmados los cambios en la rama, se subieron al repositorio remoto con:
```bash
git push origin develop-Angely
```
<img width="541" height="128" alt="image" src="https://github.com/user-attachments/assets/1ee73570-a514-4d77-a06a-8b7823b03dcf" />


---
## 📋 Roles
| Nombre           | Rol          | Funciones                                              |  
|------------------|--------------|--------------------------------------------------------|  
| Ashlee Maldonado | Full Stack   | - Creación de pantallas y componentes reutilizables.<br>- Apoyo en la lógica interna del sistema.<br>- Elaboración de la documentación del proyecto.              | 
| Angely Corahua   | Full Stack   | - Diseño visual y organización de interfaces.<br>- Manejo de datos mostrados al usuario.<br>- Revisión y validación de formularios.                               |  
| Bruno Guerra     | Full Stack   | - Desarrollo de reglas y procesos internos del sistema.<br>- Configuración de seguridad y accesos.<br>- Administración del repositorio y despliegue del proyecto. |  

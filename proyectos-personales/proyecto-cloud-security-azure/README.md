# 🔐 Seguridad básica en Azure Storage: de expuesto a seguro  
Proyecto orientado hacia Cloud Security Engineer

Este proyecto muestra cómo una configuración insegura en **Azure Blob Storage** puede exponer datos públicamente y cómo aplicar buenas prácticas de seguridad para protegerlos.  
Se trata de mi primer proyecto práctico orientado a **Cloud Security**, realizado como parte de mi proceso formativo en el Grado de Ciencia e Ingeniería de Datos.

---

## 🧭 Objetivo del proyecto

- Comprender cómo funciona el almacenamiento en Azure.  
- Detectar configuraciones inseguras (Blob Container público).  
- Aplicar principios básicos de seguridad: **acceso mínimo, IAM y auditoría**.  
- Validar que los datos quedan protegidos correctamente.  
- Documentar y estructurar el proceso como haría un Cloud Security Engineer junior.

---

## 🟦 1. Preparación del entorno

Antes de iniciar el proyecto:

- Activé **Azure for Students** con mi correo universitario.  
- Habilité **autenticación de dos factores (2FA)**.  
- Accedí al **Azure Portal** y me familiaricé con los servicios.  

---

## 🟦 2. Creación del Storage Account

1. Azure Portal → *Create a resource* → *Storage Account*.  
2. Nombre: `lorenavillastorage`  
3. Región: *West Europe*.  
4. Resto de configuraciones por defecto.  
5. Validación de la creación del recurso.

---

## 🟦 3. Creación del Blob Container

1. Entré en el Storage Account.  
2. Abrí la sección **Containers**.  
3. Creé un contenedor llamado `imagenes`.  
4. Le di **acceso público (Public)** para observar el impacto.

---

## 🟦 4. Subida de archivos y comprobación pública

- Subí una imagen de prueba.  
- Comprobé que el enlace público funcionaba sin login.  
- Validación: cualquier persona podía ver el contenido.  
> ❗ Esto demuestra una configuración insegura frecuente en entornos cloud.

---

## 🟦 5. Aplicación de seguridad: cerrar acceso público

Para asegurar el contenedor:

1. Cambié el **Public access level** → `Private`.  
2. Guardé cambios y probé el enlace anterior.  
3. El resultado fue **Access Denied** → ✔ Seguridad aplicada correctamente.

---

## 🟦 6. Control de acceso con IAM

Apliqué permisos mínimos:

- Añadí un usuario con rol **Storage Blob Data Reader**.  
- Verifiqué que solo podía **leer** y no modificar.  
- Eliminé accesos innecesarios.

> ✔ Buenas prácticas: principio de mínimo privilegio.

---

## 🟦 7. Auditoría y logging

Activé:

- **Storage Analytics Logging**  
- **Monitoring** desde Azure Monitor  
- Revisión de logs (timestamp, tipo de acceso, IP…)

Esto permite detectar accesos indebidos o comportamientos anómalos.

---

## 🟦 8. Validación final

- El contenedor ya no es accesible sin autenticación.  
- La identidad está correctamente gestionada.  
- La actividad queda registrada.  
- El acceso es seguro y controlado.

---

## 🟦 9. Capturas del proyecto

(Aquí deberías añadir tus imágenes cuando las subas a GitHub)



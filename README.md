# Central CCTV - Consola de Seguridad de Red

Sistema web para gestión centralizada de cámaras IP, planificación de tareas técnicas y monitoreo de infraestructura de seguridad.

## 🚀 Características

- 📷 **Inventario de Cámaras IP**: Registro y gestión de cámaras en múltiples ubicaciones
- 🔐 **Control de Acceso**: Sistema de autenticación con roles (Admin/Operador)
- 📊 **Estadísticas**: Panel de métricas en tiempo real
- 🔍 **Búsqueda Avanzada**: Filtrado por ubicación, IP, cámara y grupo
- 📥 **Exportación**: Descarga de inventario en formato CSV
- 💾 **Almacenamiento Local**: Datos persistentes en el navegador
- 🎨 **Interfaz Moderna**: Diseño oscuro optimizado para TI

## 📱 Acceso Rápido

**URL Pública**: https://jgonzalez-iss.github.io/central-cctv/

### Credenciales por Defecto

| Usuario | Contraseña | Rol |
|---------|-----------|-----|
| `admin` | `BellaCCTV2026` | Administrador (Lectura/Escritura) |
| `operador` | `CCTV123` | Operador (Solo Lectura) |

⚠️ **IMPORTANTE**: Cambiar credenciales en producción

## 🛠️ Tecnología

- **Frontend**: HTML5 + CSS3 + JavaScript Vanilla
- **Estilos**: Tailwind CSS
- **Almacenamiento**: LocalStorage del navegador
- **Compatibilidad**: Chrome, Firefox, Edge, Safari

## 📊 Funcionalidades

### Inventario de Cámaras
- Agregar/Editar/Eliminar cámaras
- Asignación de IP, ubicación y grupo
- Fecha de instalación automática

### Filtrado
- Búsqueda por IP, nombre de cámara, ubicación o grupo
- Filtrado por ubicación específica
- Contador de cámaras por ubicación

### Exportación
- Descargar inventario completo en CSV
- Compatible con Excel y Google Sheets

## 🔒 Seguridad

- Autenticación local en el navegador
- Datos almacenados en LocalStorage (no se envían a servidores)
- Sesiones seguras con validación de credenciales
- Sistema de roles para control de acceso

## 🚀 Despliegue

Esta aplicación se despliega automáticamente en GitHub Pages:

```
https://jgonzalez-iss.github.io/central-cctv/
```

Cualquier cambio en la rama `main` se actualiza automáticamente.

## 👥 Compartir con Compañeros

1. Comparte el enlace: `https://jgonzalez-iss.github.io/central-cctv/`
2. Tus compañeros ingresan con las credenciales proporcionadas
3. Cada uno tiene su propia sesión
4. Los datos se almacenan localmente en cada navegador

## 📝 Base de Datos

La aplicación incluye datos de ejemplo de:
- **Planet Honda 65** (4 cámaras)
- **Honda San Juan** (3 cámaras)
- **Honda Taller** (2 cámaras)
- **Parque de la Vista** (2 cámaras)

Los datos se guardan en LocalStorage del navegador.

## 🔄 Sincronización entre Dispositivos

Para sincronizar datos entre múltiples computadores:
1. Exportar CSV desde un dispositivo
2. Compartir el archivo
3. Importar desde otro dispositivo (próximamente)

## 📞 Soporte

Para reportar bugs o sugerencias, abre un issue en el repositorio:
https://github.com/jgonzalez-iss/central-cctv/issues

## 📄 Licencia

ISC © 2026

---

**Última actualización**: 2026-07-15

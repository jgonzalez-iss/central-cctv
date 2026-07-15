# 🚀 Guía de Instalación Local - Central CCTV

## Opción 1: Acceso Directo (Recomendado para usuarios)

Simplemente abre este enlace en tu navegador:

### 🌐 **URL Pública**
```
https://jgonzalez-iss.github.io/central-cctv/
```

**Ventajas:**
- ✅ No requiere instalación
- ✅ Funciona desde cualquier dispositivo
- ✅ Datos sincronizados automáticamente
- ✅ Acceso desde red interna o internet

---

## Opción 2: Ejecutar Localmente (Para Desarrolladores)

### Requisitos
- Git
- Node.js v14+ 
- npm

### Pasos

#### 1. Clonar el repositorio
```bash
git clone https://github.com/jgonzalez-iss/central-cctv.git
cd central-cctv
```

#### 2. Instalar dependencias (Opcional, solo si tienes package.json)
```bash
npm install
```

#### 3. Servir la aplicación

**Opción A: Con Python**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Luego abre: `http://localhost:8000/public/`

**Opción B: Con Node.js (si tienes package.json)**
```bash
npm start
```

Luego abre: `http://localhost:3000`

**Opción C: Con Live Server (VS Code)**
1. Instala la extensión "Live Server"
2. Click derecho en `public/index.html`
3. Selecciona "Open with Live Server"

---

## Opción 3: Red Interna (Compartir con compañeros)

Si ejecutas localmente, tus compañeros pueden acceder así:

### 1. Obtén tu IP local

**Windows:**
```bash
ipconfig
```

**Mac/Linux:**
```bash
ifconfig
```

Busca algo como `192.168.X.X`

### 2. Comparte el enlace

```
http://192.168.X.X:8000/public/
```
o
```
http://192.168.X.X:3000
```

### 3. Tus compañeros ingresan con

| Usuario | Contraseña |
|---------|-----------|
| `admin` | `BellaCCTV2026` |
| `operador` | `CCTV123` |

---

## 🔧 Solución de Problemas

### "Puerto ya está en uso"
```bash
# Cambiar puerto
python -m http.server 8001  # o cualquier número disponible
```

### "No se abre la página"
- Verifica que estés en la carpeta correcta
- Usa `http://` (no `file://`)
- Intenta con otro puerto

### "No puedo acceder desde otra PC"
- Verifica que ambas estén en la misma red WiFi
- Usa la IP que te muestra el comando `ipconfig`
- Desactiva firewall temporalmente para probar

---

## 📊 Estructura de Archivos

```
central-cctv/
├── public/
│   └── index.html          ← Abre esto en el navegador
├── README.md
├── config.md
├── INSTALL.md              ← Este archivo
└── .gitignore
```

---

## ✅ Verificación

Una vez abierto, deberías ver:

1. Pantalla de login
2. Ingresa: `admin` / `BellaCCTV2026`
3. Panel con cámaras y ubicaciones
4. Opción de exportar a CSV

**¡Listo! 🎉**

---

**Última actualización**: 2026-07-15

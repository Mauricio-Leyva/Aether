# Aether 🌌

**Aether** es una plataforma de comunidades diseñada para fomentar la colaboración y el intercambio de conocimientos, libre del ruido y la presión de las métricas de vanidad tradicionales. Un espacio digital tranquilo para compartir ideas, reflexiones, arte y tecnología.

![Aether Banner](https://via.placeholder.com/1200x400?text=Aether+Preview) 
*(Puedes reemplazar esta imagen con una captura de pantalla real de tu proyecto)*

## ✨ Características

*   **Diseño Minimalista & Premium**: Interfaz limpia inspirada en el "Glassmorphism" y tipografía profesional (Inter).
*   **Espacios Temáticos**: Comunidades dedicadas a Tecnología, Reflexión, Arte, Ciencia y Música.
*   **Sin Métricas de Vanidad**: Enfocado en el contenido, no en los likes (aunque los tenemos, no son el centro).
*   **Autenticación Segura**: Sistema de registro e inicio de sesión protegido con JWT y encriptación PBKDF2.
*   **Arquitectura Monorepo**: Gestión eficiente de Frontend y Backend en un solo repositorio.

## 🛠️ Tecnologías

### Frontend
*   **Framework**: [Astro](https://astro.build/) (Rendimiento y simplicidad)
*   **Estilos**: [Tailwind CSS v4](https://tailwindcss.com/) (Diseño moderno y responsivo)
*   **Tipografía**: Inter (Google Fonts)

### Backend
*   **API**: [FastAPI](https://fastapi.tiangolo.com/) (Alto rendimiento, fácil de usar)
*   **Base de Datos**: SQLite (Ligera y portable)
*   **ORM**: SQLModel (Interacción intuitiva con la base de datos)
*   **Seguridad**: Python-Jose (JWT) & Passlib (Hashing)

## 🚀 Instalación y Ejecución Local

Sigue estos pasos para correr Aether en tu máquina local.

### Prerrequisitos
*   **Node.js** (v18 o superior)
*   **Python** (v3.8 o superior)
*   **Git**

### 1. Clonar el Repositorio

```bash
git clone https://github.com/Mauricio-Leyva/Aether.git
cd Aether
```

### 2. Configurar el Backend (API)

Abre una terminal y navega a la carpeta del backend:

```bash
cd backend
```

Crea un entorno virtual e instala las dependencias:

```bash
# Windows
python -m venv venv
.\venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

Instala las librerías necesarias:

```bash
pip install -r requirements.txt
```

Inicia el servidor:

```bash
uvicorn main:app --reload
```
*El backend estará corriendo en `http://127.0.0.1:8000`*

### 3. Configurar el Frontend (Cliente)

Abre **otra** terminal (mantén la del backend abierta) y navega a la carpeta del frontend:

```bash
cd frontend
```

Instala las dependencias de Node:

```bash
npm install
```

Inicia el servidor de desarrollo:

```bash
npm run dev
```
*El frontend estará disponible en `http://localhost:4321`*

## 📂 Estructura del Proyecto

```
Aether/
├── backend/            # API FastAPI y Base de Datos
│   ├── main.py         # Endpoints y lógica de Auth
│   ├── models.py       # Modelos de Base de Datos (User, Post)
│   ├── database.py     # Conexión SQLite
│   └── requirements.txt
│
├── frontend/           # Aplicación Astro
│   ├── src/
│   │   ├── components/ # Componentes reutilizables (Header, PostCard)
│   │   ├── layouts/    # Plantilla base
│   │   └── pages/      # Rutas (Inicio, Login, Crear)
│   └── astro.config.mjs
│
└── README.md           # Documentación
```

## 🤝 Contribución

¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar Aether, siéntete libre de abrir un issue o enviar un pull request.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - siéntete libre de usarlo y modificarlo.

---
Hecho con ❤️ por [Mauricio Leyva](https://github.com/Mauricio-Leyva)

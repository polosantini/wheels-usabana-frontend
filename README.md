# Wheels UniSabana - Frontend

Aplicación web frontend para la plataforma de carpooling universitario Wheels UniSabana.

## 🚀 Tecnologías

- **React** - Biblioteca de UI
- **Vite** - Build tool y dev server
- **React Router** - Enrutamiento
- **Zustand** - Estado global
- **Axios** - Cliente HTTP
- **React Hook Form** - Manejo de formularios

## 📋 Requisitos Previos

- Node.js (v16 o superior)
- npm o yarn

## ⚙️ Instalación

1. Clonar el repositorio:
```bash
git clone <tu-repo-url>
cd frontend
```

2. Instalar dependencias:
```bash
npm install
```

3. Configurar variables de entorno:
Crear un archivo `.env` en la raíz con:
```env
VITE_API_URL=http://localhost:3000
```

4. Iniciar el servidor de desarrollo:
```bash
npm run dev
```

5. Construir para producción:
```bash
npm run build
```

## 📁 Estructura del Proyecto

```
frontend/
├── public/
│   └── vite.svg
├── src/
│   ├── api/              # Servicios de API
│   ├── assets/           # Recursos estáticos
│   │   └── images/       # Imágenes (logo, etc.)
│   ├── components/       # Componentes reutilizables
│   │   └── common/       # Componentes comunes (Toast, etc.)
│   ├── pages/            # Páginas/Vistas
│   │   ├── auth/         # Login, Registro
│   │   ├── driver/       # Vistas de conductor
│   │   └── passenger/    # Vistas de pasajero
│   ├── store/            # Estado global (Zustand)
│   ├── App.jsx           # Componente principal
│   ├── main.jsx          # Punto de entrada
│   └── index.css         # Estilos globales
├── .env.example
├── .gitignore
├── index.html
├── package.json
└── vite.config.js
```

## 🎨 Sistema de Diseño

### Paleta de Colores
- **Azul Principal**: `#032567` - Botones, CTAs
- **Azul Hover**: `#1A6EFF` - Hover de botones principales
- **Azul Claro**: `#e0f2fe` - Fondos de badges activos
- **Gris Oscuro**: `#57534e` - Texto secundario
- **Gris Claro**: `#f5f5f4` - Badges inactivos
- **Blanco**: `#ffffff` - Fondo principal

### Tipografía
- **Fuente**: Inter (Google Fonts)
- **Peso**: Normal (400) - Sin bold excesivo
- **Tamaños**: Relativos (rem)

### Componentes
- **Botones**: Border radius 25px, padding 12px, sombras sutiles
- **Inputs**: Border radius 25px, background `#d9d9d9`
- **Cards**: Border radius 12px, sombras ligeras
- **Badges**: Border radius 20px (estados), 12px (otros)

## 🔐 Rutas Protegidas

### Públicas
- `/` - Landing page
- `/login` - Iniciar sesión
- `/register` - Registro

### Autenticadas
- `/dashboard` - Dashboard principal
- `/profile` - Perfil de usuario

### Pasajero
- `/search` - Buscar viajes
- `/my-trips` - Mis viajes

### Conductor
- `/driver/become-driver` - Registrarse como conductor
- `/driver/create-trip` - Crear oferta de viaje
- `/driver/my-trips` - Mis viajes (conductor)
- `/driver/trips/:id` - Detalles de viaje
- `/driver/my-vehicle` - Mi vehículo

## 🛠️ Scripts Disponibles

```bash
# Desarrollo
npm run dev

# Build
npm run build

# Preview de build
npm run preview

# Linting
npm run lint
```

## 📱 Características

### Pasajero
- ✅ Búsqueda de viajes disponibles
- ✅ Solicitud de reservas
- ✅ Gestión de mis viajes (en progreso, reservados, completados, cancelados)
- ✅ Cancelación de reservas pendientes
- ✅ Cambio a rol conductor

### Conductor
- ✅ Registro de vehículo
- ✅ Publicación de viajes
- ✅ Gestión de solicitudes de reserva (aceptar/rechazar)
- ✅ Vista de detalles de viajes
- ✅ Actualización de información de vehículo
- ✅ Cambio a rol pasajero

### General
- ✅ Autenticación JWT
- ✅ Edición de perfil
- ✅ Cambio de contraseña
- ✅ Cambio de foto de perfil
- ✅ Sistema de notificaciones (Toasts)
- ✅ Diseño responsive
- ✅ Validación de formularios

## 🌐 Despliegue

### Vercel (Recomendado)
1. Instalar Vercel CLI: `npm i -g vercel`
2. Ejecutar: `vercel`
3. Configurar variables de entorno en Vercel dashboard

### Netlify
1. Build command: `npm run build`
2. Publish directory: `dist`
3. Configurar variables de entorno

## 📝 Licencia

Este proyecto es parte de un proyecto académico de la Universidad de La Sabana.

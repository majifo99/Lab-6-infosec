# Auth0 Express App

Una aplicación Express.js con autenticación Auth0 usando OpenID Connect.

## Características

- Autenticación con Auth0
- Rutas protegidas
- Dashboard de usuario
- Variables de entorno para configuración

## Instalación

1. Clona el repositorio:
```bash
git clone <url-del-repositorio>
cd Copiar-Contenido-A-Su-Folter
```

2. Instala las dependencias:
```bash
npm install
```

3. Configura las variables de entorno:
   - Copia `.env.example` a `.env`
   - Actualiza las variables con tu configuración de Auth0

4. Inicia la aplicación:
```bash
npm start
```

## Variables de Entorno

Crea un archivo `.env` con las siguientes variables:

```
ISSUER_BASE_URL=https://tu-tenant.auth0.com
CLIENT_ID=tu-client-id
CLIENT_SECRET=tu-client-secret
BASE_URL=http://localhost:3000
REDIRECT_URI=http://localhost:3000/dashboard
SECRET=tu-secret-key
PORT=3000
AUTH_REQUIRED=false
AUTH0_LOGOUT=true
```

## Rutas

- `/` - Página principal (muestra estado de autenticación)
- `/login` - Iniciar sesión con Auth0
- `/logout` - Cerrar sesión
- `/dashboard` - Dashboard protegido (requiere autenticación)

## Tecnologías

- Express.js
- Auth0 / express-openid-connect
- Swig (motor de plantillas)
- Express Sessions

## Licencia

MIT
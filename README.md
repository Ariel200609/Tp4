# Gestor de Personas - Full Stack Application

Esta es una aplicación full-stack que incluye un backend API con Express y un frontend con React + Vite.

## Estructura del Proyecto

```
tp4progra2/
├── Backend/                 # API Express con estructura MVC
│   ├── models/
│   │   └── Persona.js       # Modelo de datos
│   ├── controllers/
│   │   └── personasController.js  # Controlador
│   ├── routes/
│   │   └── personasRoutes.js      # Rutas
│   ├── package.json
│   └── server.js            # Servidor principal
└── Frontend/                # Aplicación React + Vite
    ├── src/
    │   ├── components/
    │   │   ├── TraerPersonas.jsx
    │   │   ├── ListaTarjetas.jsx
    │   │   └── TarjetaPersona.jsx
    │   ├── App.jsx
    │   └── main.jsx
    ├── package.json
    └── index.html
```

## Características

### Backend
- ✅ API REST con Express
- ✅ Estructura MVC (Modelo-Vista-Controlador)
- ✅ Ruta GET `/personas` que devuelve lista de personas
- ✅ Cada persona tiene: id, nombre, apellido, edad, email
- ✅ Al menos 5 personas de ejemplo
- ✅ CORS habilitado para comunicación con frontend

### Frontend
- ✅ React con Vite
- ✅ Componente `TraerPersonas` que hace petición HTTP
- ✅ Componente `ListaTarjetas` que recibe array de personas
- ✅ Componente `TarjetaPersona` con diseño atractivo
- ✅ Diseño responsive y moderno
- ✅ Estados de carga y error

## Instalación y Ejecución

### 1. Backend

```bash
# Navegar al directorio del backend
cd Backend

# Instalar dependencias
npm install

# Ejecutar en modo desarrollo
npm run dev

# O ejecutar en modo producción
npm start
```

El backend estará disponible en: `http://localhost:3000`

### 2. Frontend

```bash
# Navegar al directorio del frontend
cd Frontend

# Instalar dependencias
npm install

# Ejecutar en modo desarrollo
npm run dev
```

El frontend estará disponible en: `http://localhost:5173`

## Endpoints de la API

- `GET /` - Información de la API
- `GET /personas` - Obtener todas las personas

### Ejemplo de respuesta de `/personas`:

```json
{
  "success": true,
  "data": [
    {
      "id": 1,
      "nombre": "Juan",
      "apellido": "García",
      "edad": 28,
      "email": "juan.garcia@email.com"
    }
  ],
  "message": "Personas obtenidas exitosamente"
}
```

## Tecnologías Utilizadas

### Backend
- Node.js
- Express.js
- CORS

### Frontend
- React 18
- Vite
- Axios
- CSS3 con efectos modernos

## Componentes React

1. **TraerPersonas**: Maneja la petición HTTP y estados de carga/error
2. **ListaTarjetas**: Renderiza la lista de tarjetas de personas
3. **TarjetaPersona**: Muestra los datos de una persona individual

## Características del Diseño

- Diseño glassmorphism con efectos de blur
- Gradientes modernos
- Animaciones suaves
- Diseño responsive
- Estados interactivos (hover, loading, error)
- Iconos y avatares generados dinámicamente

## Notas Importantes

- Asegúrate de que el backend esté ejecutándose antes de usar el frontend
- El frontend hace peticiones a `http://localhost:3000/personas`
- La aplicación es completamente funcional y lista para usar #   T p 4  
 
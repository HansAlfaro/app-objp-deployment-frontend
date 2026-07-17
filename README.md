# Frontend — Objetos Perdidos del Campus

Sistema web de gestión de objetos perdidos y reclamaciones para el campus universitario, desarrollado con **React** y **Vite**.

## Descripción General

El Frontend proporciona una interfaz completa para que estudiantes y administradores gestionen objetos perdidos, realicen reclamaciones y administren el sistema.

### Funcionalidades Principales

#### Para Estudiantes
- **Autenticación**: Sistema de login y registro de usuarios
- **Visualización de Objetos**: Catálogo de objetos perdidos disponibles con detalles completos
- **Búsqueda y Filtrado**: Localización de objetos por categoría, ubicación y descripción
- **Reclamaciones**: Posibilidad de reclamar objetos perdidos
- **Historial de Reclamaciones**: Seguimiento de reclamaciones personales realizadas

#### Para Administradores
- **Panel de Control**: Dashboard administrativo para gestión del sistema
- **Gestión de Usuarios**: Crear, editar y eliminar usuarios del sistema
- **Gestión de Objetos**: Agregar, editar y eliminar objetos del catálogo
- **Gestión de Reclamaciones**: Revisar, validar y resolver reclamaciones de usuarios
- **Registro de Usuarios**: Interface para registrar nuevos administradores

## Estructura del Proyecto

```
src/
├── components/      # Componentes React reutilizables
├── pages/          # Páginas principales (Login, Register, StudentPage, AdminPage)
├── context/        # Context API para gestión de autenticación
├── services/       # Servicios para comunicación con la API
├── data/          # Datos estáticos (emojis, ubicaciones)
└── assets/        # Recursos estáticos
```

## Tecnologías Utilizadas

- **React 18**: Framework para construir la interfaz de usuario
- **Vite**: Herramienta de construcción y desarrollo rápido
- **Axios**: Cliente HTTP para comunicación con la API
- **Context API**: Gestión de estado global (autenticación)
- **CSS**: Estilos personalizados por componente

## Cómo Ejecutar

```bash
# Instalar dependencias
npm install

# Ejecutar en modo desarrollo
npm run dev

# Construir para producción
npm run build
```

## Conexión con el Backend

El Frontend se conecta a una API REST proporcionada por el backend. Los endpoints se consumen a través de servicios ubicados en `src/services/`.

### Servicios Disponibles
- **auth.service.js**: Autenticación y gestión de tokens JWT
- **objeto.service.js**: CRUD de objetos perdidos
- **reclamo.service.js**: CRUD de reclamaciones
- **categoria.service.js**: Gestión de categorías

## Características de Diseño

- **Interfaz Responsive**: Adaptable a diferentes tamaños de pantalla
- **Modal Management**: Interfaces modales para edición y visualización de detalles
- **Validación de Formularios**: Validación en cliente antes de enviar datos
- **Manejo de Errores**: Mensajes de error claros para el usuario

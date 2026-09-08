# 🎯 FOCUS+ - PWA para Gestionar Entregas

Tu tiempo, tus reglas, tu progreso.

FOCUS+ es una aplicación web progresiva (PWA) diseñada para ayudar a estudiantes a dejar de procrastinar y gestionar mejor su tiempo antes de las entregas académicas.

## ✨ Características

### 🧠 Test de Procrastinación Personalizado
La app comienza conociendo cómo procrastinas:
- **4 preguntas** para determinar tu tipo de procrastinador
- Identifica qué te tranquiliza
- Descubre qué usas como recompensa
- Conoce cómo te gusta sentirte

### 📊 Dashboard Inteligente
- **Próximas entregas** con indicadores visuales de urgencia
- **Misión del día** - pequeñas tareas de 20 minutos
- **Perfil personalizado** con tu estrategia recomendada
- **Progreso en tiempo real** de tus proyectos

### ⏱️ Modo Enfoque
- Temporizador de 20 minutos
- Interfaz sin distracciones
- Registro automático de avances
- Sistema de XP y racha

### 🔐 Modo Compromiso
Establece tus propias reglas voluntariamente:
- Bloquear redes sociales si te atrasas
- Activar modo concentración automático
- Notificaciones a tu acudiente
- Alertas de retraso personalizables

### 👨‍👩‍👧 Conexión con Acudientes
- Comparte solo lo que quieres
- Privacidad configurable
- Dashboard para padres/tutores
- Seguimiento sin invasión

## 🚀 Cómo Usar

### En tu Computadora
1. Abre `index.html` en tu navegador
2. O usa un servidor local: `python -m http.server 8000`
3. Accede a `http://localhost:8000`

### En iPhone
1. Abre Safari
2. Ve a la URL de la app
3. Toca **Compartir**
4. Selecciona **Añadir a pantalla de inicio**
5. Abre como app nativa

### En Android
1. Abre Chrome
2. Ve a la URL de la app
3. Toca el menú (⋮)
4. Selecciona **Instalar app**

## 🎨 Diseño Visual

- **Color principal:** Morado (#6C63FF)
- **Fondo:** Muy claro (#F6F7FB)
- **Tipografía:** System fonts Apple
- **Estilo:** Moderno, juvenil, amigable
- **Optimizado:** Para iPhone principalmente

## 📁 Estructura de Archivos

```
focus-plus-pwa/
├── index.html           # HTML principal
├── styles.css           # Estilos CSS
├── app.js              # Lógica de la aplicación
├── sw.js               # Service Worker
├── manifest.webmanifest # PWA manifest
└── README.md           # Este archivo
```

## 🔧 Tecnologías

- **HTML5** - Estructura
- **CSS3** - Estilos modernos con variables
- **JavaScript Vanilla** - Sin dependencias
- **PWA** - Funciona offline
- **LocalStorage** - Datos persistentes

## 📱 Pantallas Principales

### 1. Bienvenida
Introduce al usuario a la app y comienza el test.

### 2. Test de Procrastinación
4 preguntas interactivas para conocer al usuario.

### 3. Perfil Resultado
Muestra el perfil personalizado y la estrategia recomendada.

### 4. Dashboard
Pantalla principal con misión, entregas y perfil.

### 5. Modo Enfoque
Temporizador de 20 minutos sin distracciones.

### 6. Registro de Avance
Documenta qué completaste en tu misión.

### 7. Modo Compromiso
Configura tus propias reglas de bloqueo.

### 8. Guardián
Conecta a un acudiente y controla privacidad.

### 9. Ajustes
Información de la app y gestión de perfil.

## 💾 Datos Almacenados

Todos los datos se guardan localmente en `localStorage`:
- Perfil del usuario
- Entregas y progreso
- Misiones completadas
- XP y racha
- Configuración de compromiso
- Preferencias de privacidad

**No se envía información a servidores externos en esta versión.**

## 🎯 Tipos de Procrastinadores

La app identifica 5 tipos:

1. **El que empieza rápido** - Comienza inmediatamente
2. **El que piensa que todavía hay tiempo** - Pospone por lejana la fecha
3. **El abrumado** - No sabe por dónde empezar
4. **El distractor** - Se distrae con redes sociales
5. **El que trabaja bajo presión** - Necesita urgencia

## 🌟 Conceptos Principales

### "Tu tiempo, tus reglas, tu progreso"
La app respeta las decisiones del usuario y es un acompañante, no un juez.

### "Primero haz lo que necesitas. Después disfruta lo que quieres."
Recompensas personalizadas basadas en las preferencias del usuario.

### Misiones de 20 minutos
Pequeños bloques de tiempo manejables, no abrumadores.

## 🔮 Futuras Integraciones

- **Microsoft Teams** - Importar entregas automáticamente
- **Google Calendar** - Sincronizar fechas
- **Email** - Notificaciones
- **Real App Blocking** - Bloqueo real de aplicaciones
- **Analytics** - Análisis de productividad

## 🛠️ Desarrollo

### Agregar una nueva pantalla

1. Añade un caso en `switch(appState.currentScreen)`
2. Crea función `renderNewScreen()`
3. Actualiza navegación si es necesario

### Modificar preguntas del test

Edita el array `questions` en `app.js`:

```javascript
const questions = [
  {
    text: 'Tu pregunta',
    options: ['Opción 1', 'Opción 2', ...]
  }
];
```

### Cambiar colores

Modifica las variables de color en `styles.css`:
- `#6C63FF` - Morado principal
- `#F6F7FB` - Fondo claro
- `#1B2230` - Texto oscuro

## 📄 Licencia

MIT - Libre para usar y modificar

## 🤝 Contacto

Creado para estudiantes que luchan contra la procrastinación.

---

**FOCUS+** - Porque procrastinar es normal, pero abandonar nunca. 🚀
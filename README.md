# 🏋️ Coach Admin - Sistema de Gestión de Coaches

Sistema completo de gestión para coaches deportivos con sincronización en la nube. Administra tus clientes, pagos, asistencias, medidas corporales y rutinas de ejercicios desde cualquier dispositivo.

## ✨ Características Principales

### 📊 Gestión de Coaches
- ✅ Registro completo de información de clientes
- ✅ Gestión de periodos de pago
- ✅ Control de asistencias con calendario
- ✅ Estados visuales (activo, pendiente, vencido)
- ✅ Búsqueda y filtrado de coaches

### 💰 Control de Pagos
- ✅ Registro de pagos por periodo
- ✅ Cálculo automático de fechas de vencimiento
- ✅ Alertas visuales de pagos pendientes
- ✅ Historial completo de pagos

### 📅 Calendario de Asistencias
- ✅ Vista mensual, semanal y lista
- ✅ Registro rápido de asistencias
- ✅ Visualización de historial
- ✅ Optimizado para móvil y desktop

### 📏 Medidas Corporales
- ✅ Registro de peso, altura, edad
- ✅ Cálculo automático de IMC
- ✅ Historial por periodo
- ✅ Seguimiento de progreso

### 💪 Biblioteca de Ejercicios
- ✅ Gestión personalizada de ejercicios
- ✅ Agregar, editar y eliminar ejercicios
- ✅ Búsqueda rápida

### ☁️ Sincronización en la Nube
- ✅ **Sincronización automática** entre dispositivos
- ✅ Respaldo en tiempo real con JSONBin.io
- ✅ Acceso desde móvil, tablet y desktop
- ✅ Sin instalación de servidor
- ✅ **Mismo dato en todos tus dispositivos**

### 🎨 Interfaz Moderna
- ✅ Diseño responsive (móvil y desktop)
- ✅ Modo oscuro/claro
- ✅ Animaciones fluidas
- ✅ Optimizado para touch

### 🤖 Asistente IA (Coach Virtual)
- ✅ Generación de rutinas personalizadas
- ✅ Consejos de entrenamiento
- ✅ Integración con DeepSeek AI

## 🚀 Instalación

### Opción 1: Uso Local (Más Simple)
1. Descarga el archivo `index.html`
2. Ábrelo en tu navegador
3. ¡Listo! La aplicación funciona sin servidor

### Opción 2: Con Servidor Web
```bash
# Usando Python
python -m http.server 8000

# O usando Node.js
npx serve

# Luego abre: http://localhost:8000
```

## 🧪 Datos de Prueba

Para probar la aplicación con datos de ejemplo completos:

### 📥 Importar Datos de Prueba

1. Descarga el archivo `datos-prueba.json`
2. Abre la aplicación
3. Ve a **Configuración** (⚙️)
4. Haz clic en **"Importar datos"**
5. Selecciona el archivo `datos-prueba.json`
6. ¡Listo! Verás 6 coaches con datos completos

### 📊 ¿Qué incluyen los datos de prueba?

- **6 Coaches** con perfiles diversos:
  - María González (Tonificación, 3 días/semana)
  - Carlos Martínez (Atleta, preparación maratón)
  - Ana Rodríguez (Principiante, pérdida de peso)
  - Juan Pérez (Hipertrofia, 5 días/semana)
  - Laura Sánchez (CrossFit, nivel avanzado)
  - Diego Torres (Plan ejecutivo, 2 días/semana)

- **Pagos registrados** para cada coach
- **Historial de asistencias** con rutinas completas
- **Medidas corporales** con seguimiento
- **28 ejercicios** en la biblioteca
- **Rutinas detalladas** con:
  - Calentamientos
  - Ejercicios con series, reps y pesos
  - Notas y observaciones
  - Diferentes tipos: máquinas y calistenia

### 💡 Casos de Uso de los Datos de Prueba

Los datos de prueba te permiten explorar:
- ✅ Diferentes tipos de clientes y objetivos
- ✅ Historial de asistencias y faltas
- ✅ Rutinas variadas (fuerza, resistencia, principiante)
- ✅ Seguimiento de medidas corporales
- ✅ Estados de pago (activos, vencidos)

## ⚙️ Configuración de Sincronización en la Nube

### 📋 Requisitos
- Cuenta gratuita en [JSONBin.io](https://jsonbin.io)
- Plan gratuito incluye 10,000 requests/mes (más que suficiente)

### 🔧 Configuración Inicial

#### 1. Crear Cuenta en JSONBin.io
1. Visita https://jsonbin.io
2. Crea una cuenta gratuita
3. Ve a la sección "API Keys"
4. Copia tu **Master Key** y **Access Key**

#### 2. Configurar las Keys en la Aplicación
Abre `index.html` y busca estas líneas (alrededor de la línea 1839):

```javascript
const JSONBIN_MASTER_KEY = 'TU_MASTER_KEY_AQUI';
const JSONBIN_ACCESS_KEY = 'TU_ACCESS_KEY_AQUI';
```

Reemplaza con tus keys:
```javascript
const JSONBIN_MASTER_KEY = '$2a$10$4d8nGl4vV/rjeR1UUMlR7OA32Vpph.pvceoEokv3OzaIiejifVgPm';
const JSONBIN_ACCESS_KEY = '$2a$10$lxvV9USetswKtFK3wxaMqOTjKlNs.SiZbv3X9NZcOJWpYZQqEjG.m';
```

## 🔄 Cómo Sincronizar Entre Dispositivos

### 📱 Primer Dispositivo (Ej: Tu Teléfono)
1. Abre la aplicación
2. Agrega tus coaches y datos
3. Haz clic en el botón de **Configuración** (⚙️)
4. En la sección **"☁️ Sincronización en la Nube"**
5. Copia el **"ID de tu Nube"** (📋 botón copiar)
6. Guarda ese ID (envíatelo por WhatsApp, email, etc.)

### 💻 Segundo Dispositivo (Ej: Tu Computadora)
1. Abre la aplicación
2. Haz clic en **Configuración** (⚙️)
3. En **"☁️ Sincronización en la Nube"**
4. Pega el ID en el campo **"¿Tienes un ID de otro dispositivo?"**
5. Haz clic en **"Aplicar"**
6. ¡Automáticamente descargará todos tus datos! 🎉

### 🔄 Sincronización Continua
- **Automática**: Los cambios se suben automáticamente al guardar
- **Manual**: Haz clic en el botón ☁️ en el header para sincronizar
- **Bidireccional**: Primero descarga, luego sube cambios

## 📱 Uso de la Aplicación

### Agregar un Coach
1. Haz clic en el botón **"+ Agregar Coach"**
2. Completa el formulario (nombre, email, teléfono)
3. Haz clic en **"Guardar Coach"**
4. ✅ Se sincroniza automáticamente con la nube

### Registrar un Pago
1. Selecciona un coach de la lista
2. Haz clic en **"💰 Registrar Pago"**
3. Ingresa monto, fecha inicio y duración del periodo
4. Haz clic en **"Registrar Pago"**

### Marcar Asistencias
1. En la vista del coach, ve a la pestaña **"Calendario"**
2. Selecciona el periodo activo
3. Haz clic en los días para marcar/desmarcar asistencia

### Registrar Medidas Corporales
1. En la vista del coach, ve a **"Medidas"**
2. Haz clic en **"+ Agregar Medida"**
3. Ingresa peso, altura, edad, etc.
4. El IMC se calcula automáticamente

### Gestionar Ejercicios
1. Ve a **Configuración** (⚙️)
2. Haz clic en **"Biblioteca de Ejercicios"**
3. Agrega, edita o elimina ejercicios

### Usar el Coach IA
1. Haz clic en el botón flotante 🤖 (esquina inferior derecha)
2. Configura tu API Key de DeepSeek (primera vez)
3. Conversa con el asistente para generar rutinas

## 💾 Backup y Restauración

### Exportar Datos
1. Ve a **Configuración** (⚙️)
2. Haz clic en **"Exportar datos"**
3. Se descargará un archivo JSON con todos tus datos

### Importar Datos
1. Ve a **Configuración** (⚙️)
2. Haz clic en **"Importar datos"**
3. Selecciona tu archivo JSON de backup
4. Confirma la importación
5. ✅ Los datos se sincronizan automáticamente con la nube

## 🎨 Personalización

### Modo Oscuro
- Haz clic en el botón 🌙/☀️ en el header
- Se guarda automáticamente tu preferencia

### Modo de Pruebas
- Útil para testing y demos
- Actívalo en **Configuración** (⚙️)
- Te permite simular fechas

## 🛠️ Tecnologías Utilizadas

- **HTML5** - Estructura
- **Tailwind CSS** - Estilos y diseño responsive
- **JavaScript Vanilla** - Lógica de la aplicación
- **LocalStorage** - Almacenamiento local
- **JSONBin.io API** - Sincronización en la nube
- **SweetAlert2** - Modales y notificaciones
- **DeepSeek AI** - Asistente virtual (opcional)

## 📊 Estructura de Datos

### Coaches
```javascript
{
  "coaches": [
    {
      "id": "1234567890",
      "nombre": "Juan Pérez",
      "email": "juan@example.com",
      "telefono": "+57 300 1234567",
      "notas": "Cliente desde 2024"
    }
  ]
}
```

### Pagos
```javascript
{
  "pagos": {
    "coach_id": [
      {
        "id": "pago123",
        "monto": 150000,
        "periodoInicio": "2024-01-01",
        "periodoFin": "2024-01-31",
        "fechaPago": "2024-01-01"
      }
    ]
  }
}
```

### Asistencias
```javascript
{
  "asistencias": {
    "coach_id": {
      "pago_id": {
        "2024-01-15": true,
        "2024-01-16": true
      }
    }
  }
}
```

## 🔐 Seguridad y Privacidad

- ✅ Todos los datos se almacenan localmente en tu navegador
- ✅ La sincronización usa tu cuenta privada de JSONBin.io
- ✅ Solo tú tienes acceso a tus API Keys
- ✅ Sin servidor propio = sin vulnerabilidades de servidor
- ✅ Compatible con HTTPS para máxima seguridad

## 🐛 Solución de Problemas

### "No sincroniza entre dispositivos"
✅ **Solución**: Asegúrate de usar el **mismo Bin ID** en todos los dispositivos
1. Copia el ID del primer dispositivo (Configuración → Sincronización)
2. Pégalo en los demás dispositivos

### "Error al sincronizar"
✅ **Solución**: Verifica tus API Keys en el código
- Asegúrate de tener la Master Key correcta
- Verifica que tu cuenta de JSONBin.io esté activa

### "Los datos no se muestran"
✅ **Solución**: Haz clic en el botón ☁️ para forzar sincronización
- Abre la consola (F12) para ver logs detallados

### "IMC no se calcula"
✅ **Solución**: Verifica que peso y altura tengan valores válidos
- Peso en kg (ej: 70.5)
- Altura en metros (ej: 1.75)

## 📝 Roadmap / Futuras Mejoras

- [ ] Gráficas de progreso de medidas
- [ ] Notificaciones push de pagos pendientes
- [ ] Exportar reportes en PDF
- [ ] Múltiples coaches para un solo usuario admin
- [ ] Integración con calendarios (Google Calendar)
- [ ] App móvil nativa (PWA)

## 🤝 Contribuciones

¿Tienes ideas o mejoras? Las contribuciones son bienvenidas:
1. Fork del proyecto
2. Crea una rama con tu feature
3. Haz commit de tus cambios
4. Push a la rama
5. Abre un Pull Request

## 📄 Licencia

Este proyecto es de código abierto y está disponible bajo la licencia MIT.

## 👨‍💻 Autor

Desarrollado con ❤️ para coaches y entrenadores personales.

## 📞 Soporte

¿Tienes preguntas o necesitas ayuda?
- 📧 Abre un issue en GitHub
- 💬 Revisa la documentación en este README
- 🔍 Consulta la consola del navegador (F12) para logs detallados

---

## 🎯 Quick Start

### Opción A: Empezar desde Cero
```bash
# 1. Descarga el proyecto
git clone [URL_DEL_REPO]
cd coach-admin

# 2. Abre index.html en tu navegador
open index.html

# 3. Agrega tu primer coach manualmente
# Haz clic en "+ Agregar Coach"

# 4. (Opcional) Configura sincronización en la nube
# Edita index.html y agrega tus API Keys de JSONBin.io
```

### Opción B: Probar con Datos de Ejemplo (Recomendado)
```bash
# 1. Descarga el proyecto
git clone [URL_DEL_REPO]
cd coach-admin

# 2. Abre index.html en tu navegador
open index.html

# 3. Importa los datos de prueba
# - Ve a Configuración (⚙️)
# - Haz clic en "Importar datos"
# - Selecciona el archivo "datos-prueba.json"
# - ¡Verás 6 coaches con datos completos!

# 4. Explora todas las funcionalidades
# - Calendario de asistencias
# - Rutinas de ejercicios
# - Medidas corporales
# - Pagos y periodos
```

### 🎬 Demo Rápida (2 minutos)

1. **Abre `index.html`** en tu navegador
2. **Importa `datos-prueba.json`** desde Configuración
3. **Explora**:
   - Haz clic en "María González"
   - Ve la pestaña "Calendario"
   - Mira las rutinas del 3, 5 y 8 de enero
   - Revisa sus medidas corporales
4. **Prueba agregar**:
   - Una nueva rutina en un día futuro
   - Una medida corporal
   - Un nuevo pago

---

**¡Disfruta gestionando tus coaches!** 🏋️💪🎉


# 💈 BarberPro — SaaS de Gestión para Barberías

> Plataforma SaaS completa para la gestión integral de barberías. Desarrollada con React, Supabase y Tailwind CSS, con 12 módulos funcionales y cliente piloto real en operación.

---

## 🌐 Demo en vivo

👉 **[barberproo0.netlify.app](https://barberproo0.netlify.app)**

---

## ✨ Módulos incluidos

| # | Módulo | Descripción |
|---|--------|-------------|
| 1 | 📊 Dashboard | Vista general del negocio en tiempo real |
| 2 | 📅 Citas | Agendamiento y gestión de turnos |
| 3 | 👥 Clientes | Base de datos de clientes con historial |
| 4 | ✂️ Servicios | Catálogo de servicios y precios |
| 5 | 📱 Recordatorios WhatsApp | Notificaciones automáticas a clientes |
| 6 | 🏆 Programa de lealtad | Puntos y recompensas para clientes frecuentes |
| 7 | 📦 Inventario | Control de productos e insumos |
| 8 | 💰 Caja registradora | Registro de ingresos y egresos |
| 9 | 👨‍💼 Empleados | Gestión del equipo de trabajo |
| 10 | 🎁 Referidos | Sistema de referidos con beneficios |
| 11 | 📋 Bitácora | Registro de actividad y eventos |
| 12 | 🔐 PIN de seguridad | Control de acceso por roles |

---

## 🛠️ Tech Stack

| Capa | Tecnología |
|------|-----------|
| Frontend | React, Vite |
| Estilos | Tailwind CSS |
| Backend / DB | Supabase (PostgreSQL) |
| Autenticación | Supabase Auth |
| Seguridad | Row Level Security (RLS) |
| Despliegue | Netlify |

---

## 📁 Estructura del proyecto

```
barberpro/
├── src/
│   ├── components/         # Componentes reutilizables
│   ├── pages/              # Páginas por módulo
│   ├── hooks/              # Custom hooks
│   ├── lib/                # Configuración de Supabase
│   └── main.jsx            # Entry point
├── public/
├── index.html
├── vite.config.js
├── tailwind.config.js
└── package.json
```

---

## ⚙️ Instalación y configuración

### 1. Clona el repositorio

```bash
git clone https://github.com/Alvar069/barberpro.git
cd barberpro
```

### 2. Instala las dependencias

```bash
npm install
```

### 3. Configura las variables de entorno

Crea un archivo `.env` en la raíz del proyecto:

```env
VITE_SUPABASE_URL=tu_supabase_url
VITE_SUPABASE_ANON_KEY=tu_supabase_anon_key
```

### 4. Ejecuta en modo desarrollo

```bash
npm run dev
```

Abre tu navegador en `http://localhost:5173`

### 5. Build para producción

```bash
npm run build
```

---

## 🚀 Despliegue en Netlify

1. Conecta tu repo de GitHub con Netlify
2. Build command: `npm run build`
3. Publish directory: `dist`
4. Agrega las variables de entorno en el panel de Netlify
5. ¡Listo!

---

## 🔐 Arquitectura de seguridad

- **Row Level Security (RLS)** en Supabase — cada barbería solo accede a sus propios datos
- **Control de acceso por roles** — dueño, administrador, barbero
- **Flujo de aprobación manual** — nuevos registros quedan en estado `active: false` hasta ser aprobados
- **PIN de seguridad** — bloqueo de pantalla para proteger el sistema en caja

---

## 💼 Modelo de negocio

BarberPro está diseñado como un producto SaaS con precios validados para el mercado colombiano. Cada barbería que se registra pasa por un flujo de aprobación controlado por el administrador de la plataforma.

---

## 📋 Requisitos

- Node.js 18+
- Cuenta en [Supabase](https://supabase.com) (gratuita)
- Cuenta en [Netlify](https://netlify.com) para despliegue (gratuita)

---

## 👨‍💻 Autor

**Alvaro Daniel Reyes Blanco**  
Ingeniero de Software — Universidad de Cartagena  
📧 alvarodanielyt22@gmail.com  
🐙 [github.com/Alvar069](https://github.com/Alvar069)  
🌐 [barberproo0.netlify.app](https://barberproo0.netlify.app)

---

## 📄 Licencia

Este proyecto está bajo uso personal y educativo. Contactar al autor para uso comercial.

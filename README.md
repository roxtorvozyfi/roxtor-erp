
# 🦖 ROXTOR Intelligent ERP v1.5

Sistema de gestión operativa de alto rendimiento para la industria textil. Incluye inteligencia artificial para ventas y sincronización en la nube.

## 🚀 Guía de Activación Profesional

### PASO 1: Base de Datos (Supabase)
1. Crea un proyecto en [Supabase](https://supabase.com).
2. En el **SQL Editor**, ejecuta este comando:
   ```sql
   create table roxtor_sync (
     store_id text primary key,
     last_sync timestamp with time zone default now(),
     payload jsonb
   );
   ```
3. Copia la `Project URL` y la `anon key` desde **Settings > API**.

### PASO 2: Despliegue (Vercel)
1. Sube tu código a GitHub.
2. Conecta el repositorio en [Vercel](https://vercel.com).
3. Añade la Variable de Entorno obligatoria:
   - `API_KEY`: Tu clave de Google Gemini ([Obtenla aquí](https://aistudio.google.com)).
4. Haz clic en **Deploy**.

### PASO 3: Configuración en App
1. Abre tu URL de Vercel.
2. Ve a **Gerencia > Ajustes de Marca > Conexión Nube**.
3. Pega las credenciales de Supabase y activa la sincronización.

---

## 🔒 Credenciales Maestras
- **PIN Acceso App:** `0000`
- **PIN Gerencia:** `1234`
*(Cámbialos en el panel de Ajustes tras el primer inicio)*

## 🛠️ Funciones Principales
- **Radar AI:** Procesa textos de WhatsApp y genera órdenes automáticas.
- **Vozify:** Entrena a tu equipo con audios de respuesta con el tono de tu marca.
- **Flujo de Taller:** Control de tareas, transferencias y espera de confección externa.
- **Cierre Consolidado:** Métricas financieras por sede en tiempo real.

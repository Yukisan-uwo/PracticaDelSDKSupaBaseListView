# 📱 Student Management System - Android & Supabase

¡Bienvenido! Este es un proyecto de gestión de estudiantes desarrollado en **Android Nativo (Kotlin)**, integrado con **Supabase** como Backend-as-a-Service (BaaS). La aplicación permite visualizar y filtrar listas de estudiantes de forma dinámica según su semestre y materia asignada.

---

## 🚀 Características Principales

- **Integración con Supabase:** Uso del SDK oficial de Supabase para consultas en tiempo real y filtrado de datos desde PostgreSQL.
- **Filtrado Dinámico:** Selección de niveles (semestres) que cargan automáticamente las materias correspondientes.
- **UI Moderna:** Implementación de componentes de **Material Design 3**, incluyendo `TextInputLayout` con menús desplegables y un diseño de lista limpio.
- **Gestión de Imágenes:** Uso de la librería **Glide** para la carga asíncrona de fotografías de perfil con transformaciones circulares.
- **Eficiencia:** Manejo de procesos asíncronos mediante **Kotlin Coroutines** para garantizar una interfaz fluida.

---

## 📸 Resultados (Screenshots)

<img width="406" height="899" alt="image" src="https://github.com/user-attachments/assets/461193f8-e46c-4c0c-9849-a6de792a0986" />

---

<img width="406" height="899" alt="image" src="https://github.com/user-attachments/assets/6962038a-e766-4440-8318-4b6ee66f4d5d" />

---

<img width="946" height="535" alt="image" src="https://github.com/user-attachments/assets/99be12d0-1633-4013-b325-e4100df228cc" />

---

## 🛠️ Stack Tecnológico

- **Lenguaje:** [Kotlin](https://kotlinlang.org/)
- **Backend:** [Supabase](https://supabase.com/) (PostgreSQL + Postgrest)
- **Imagen:** [Glide](https://github.com/bumptech/glide)
- **Arquitectura:** Patrón basado en Modelos, Adaptadores y Servicios.
- **Red:** Ktor Client (consumido por Supabase SDK).

---

## ⚙️ Configuración del Proyecto

Para replicar este proyecto, sigue estos pasos:

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/tu-usuario/tu-repositorio.git
   ```

2. **Configurar Supabase:**
   - Crea las tablas `alumnos` y `materias` (puedes usar los archivos CSV proporcionados en el historial del proyecto).
   - Desactiva las RLS o configura políticas de lectura pública.

3. **Variables de Entorno:**
   En tu archivo `local.properties`, añade tus credenciales:
   ```properties
   SUPABASE_URL=https://tu-proyecto.supabase.co
   SUPABASE_KEY=tu-anon-key-aqui
   ```

4. **Ejecutar:**
   Sincroniza con Gradle y presiona **Run** en Android Studio.

---

## 📁 Estructura del Código

- `Models/`: Clases de datos (`Alumno`, `Materia`) preparadas para serialización JSON.
- `Adapters/`: `AlumnoAdapter` para el manejo personalizado de la vista de lista.
- `Services/`: `SupabaseManager` para centralizar la conexión con el cliente.
- `Utils/`: Manejo de errores global y diálogos de alerta.

---
**Desarrollado con ❤️ para la gestión académica eficiente.**

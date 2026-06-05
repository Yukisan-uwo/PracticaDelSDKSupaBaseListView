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

| Lista de Estudiantes (A-C) | Lista de Estudiantes (J-K) | Entorno de Desarrollo |
| :---: | :---: | :---: |
| <img src="https://raw.githubusercontent.com/TuUsuario/TuRepositorio/main/screenshots/resultado1.png" width="250" alt="Resultados 1"> | <img src="https://raw.githubusercontent.com/TuUsuario/TuRepositorio/main/screenshots/resultado2.png" width="250" alt="Resultados 2"> | <img src="https://raw.githubusercontent.com/TuUsuario/TuRepositorio/main/screenshots/ide_view.png" width="250" alt="Android Studio"> |

> *Nota: Asegúrate de guardar tus capturas en una carpeta llamada `/screenshots` en la raíz del repo para que se vean correctamente.*

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

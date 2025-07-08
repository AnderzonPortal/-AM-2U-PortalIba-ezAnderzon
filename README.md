# 💻 **SharedPreferences - Proyecto Semana 9**

## **Descripción del Proyecto**

**SharedPreferences** es una aplicación móvil que permite gestionar datos de usuario y preferencias a través de almacenamiento local. En este proyecto, se incluyen funcionalidades como la creación de un perfil de usuario, el contador de visitas, y la opción de cambiar entre el modo claro y oscuro para mejorar la experiencia de usuario.

**Finalidad del Proyecto:**
- **Contador de Visitas:** Llevar un registro de las veces que se abre la app.
- **Perfil de Usuario:** Crear un perfil para cada usuario que guarde su nombre, edad y correo electrónico.
- **Modo Oscuro/Claro:** Permitir al usuario alternar entre los dos modos para una mejor interacción visual dependiendo de su preferencia.

---

## **Semana 9:**

### **1. Contador de Visitas**

   - **Objetivo:** Contabilizar cuántas veces se ha abierto la aplicación.
   - **Características:**
     - Un botón para resetear el contador de visitas.

   **Vista previa:**

   <p align="center">
     <img src="S9_SharedPreferences/app/src/imagenes/contador-visitas1.png" alt="Contador de visitas 1" width="40%">
     <img src="S9_SharedPreferences/app/src/imagenes/contador-visitas2.png" alt="Contador de visitas 2" width="40%">
   </p>

---

### **2. Creación de Perfil de Usuario**

   - **Objetivo:** Crear una nueva actividad para que el usuario pueda ingresar su perfil.
   - **Campos a ingresar:**
     - Nombre
     - Edad
     - Email
   - **Acciones:**
     - Botón para guardar y cargar el perfil.
     - Los datos se deben guardar en **SharedPreferences**.

   **Vista previa:**

   <p align="center">
     <img src="S9_SharedPreferences/app/src/imagenes/perfil-usuario1.png" alt="Perfil de usuario 1" width="40%">
     <img src="S9_SharedPreferences/app/src/imagenes/perfil-usuario2.png" alt="Perfil de usuario 2" width="40%">
     <img src="S9_SharedPreferences/app/src/imagenes/perfil-usuario3.png" alt="Perfil de usuario 3" width="40%">
   </p>

---

### **3. Modo Oscuro / Claro**

   - **Objetivo:** Implementar un interruptor (Switch) que permita al usuario cambiar entre el modo claro y el modo oscuro.
   - **Características:**
     - El switch tendrá el texto **"Modo Oscuro"**.
     - Al cambiar el estado del switch, la preferencia se debe guardar inmediatamente y aplicar en tiempo real.
     - **Modo Claro:** Fondo blanco con texto negro.
     - **Modo Oscuro:** Fondo gris con texto blanco.

   **Vista previa:**

   <p align="center">
     <img src="S9_SharedPreferences/app/src/imagenes/modo-oscuro-claro1.png" alt="Modo Oscuro/Claro 1" width="40%">
     <img src="S9_SharedPreferences/app/src/imagenes/modo-oscuro-claro2.png" alt="Modo Oscuro/Claro 2" width="40%">
   </p>

---

## **Tecnologías Utilizadas - Semana 9**

- 🧩 Kotlin
- 🔐 SharedPreferences
- 🌙 Modo Oscuro / Claro
- 📱 Android Studio

---

# 🎮 **GameVault - Proyecto Semana 10**

## **Descripción del Proyecto**

**GameVault** es una aplicación móvil diseñada para gestionar tu biblioteca personal de videojuegos. El proyecto incluye integración con Firebase para la autenticación de usuarios y el almacenamiento de datos en tiempo real mediante Firebase Realtime Database. 

**Finalidad del Proyecto:**
- **Configuración Firebase Database:** Configurar Firebase Realtime Database para almacenar información de los juegos.
- **Registro de Juegos:** Crear un formulario para agregar juegos a la biblioteca y guardarlos en Firebase.
- **Lista de Juegos:** Visualizar los juegos registrados con una lista dinámica usando `RecyclerView`.

---

## **Semana 10:**

### **🔥 Configuración Firebase Database**

1. **Habilitar Realtime Database en Firebase Console**  
   ![Realtime Database](S10_GameVault/app/src/imagenes/firebase-enable-db.jpg)

2. **Configurar reglas de seguridad**  
   ![Reglas de seguridad](S10_GameVault/app/src/imagenes/firebase-rules.jpg)

3. **Agregar dependencia en `build.gradle`**  
   ![Gradle Firebase](S10_GameVault/app/src/imagenes/gradle-dependency.jpg)

---

### **💾 Registro de Juegos**

Todo comienza con un formulario intuitivo para agregar juegos a tu biblioteca personal.

- 🧩 **Crear modelo `Game.kt`**  
  ![Game Model](S10_GameVault/app/src/imagenes/modelo-game.jpg)

- 🛠️ **Implementar `AddGameActivity.kt`**  
  ![AddGameActivity](S10_GameVault/app/src/imagenes/add-game-activity.jpg)

- ✅ **Crear formulario con validaciones**  
  <img src="S10_GameVault/app/src/imagenes/formulario-validado.jpg" width="40%">

---

### **📋 Lista de Juegos**

Visualiza tus juegos registrados en una lista dinámica con datos en tiempo real.

- 🧱 **RecyclerView con `GameAdapter`**  
  ![RecyclerView](S10_GameVault/app/src/imagenes/game-adapter.jpg)

- 🙋‍♂️ **Mostrar datos del usuario autenticado**  
  <img src="S10_GameVault/app/src/imagenes/datos-usuario.jpg" width="40%">

| Funcionalidad              | Imagen                                                                 |
|---------------------------|------------------------------------------------------------------------|
| ✏️ Editar juegos           | <img src="S10_GameVault/app/src/imagenes/editar-juego1.jpg" width="35%"> &nbsp; <img src="S10_GameVault/app/src/imagenes/editar-juego2.jpg" width="35%"> &nbsp; <img src="S10_GameVault/app/src/imagenes/editar-juego3.jpg" width="35%"> |
| 🗑️ Eliminar juegos         | <img src="S10_GameVault/app/src/imagenes/eliminar-juego1.jpg" width="35%"> &nbsp;&nbsp; <img src="S10_GameVault/app/src/imagenes/eliminar-juego2.jpg" width="35%"> |
| 🎯 Filtro por género       | <img src="S10_GameVault/app/src/imagenes/filtro-genero1.jpg" width="35%"> &nbsp;&nbsp; <img src="S10_GameVault/app/src/imagenes/filtro-genero2.jpg" width="35%"> |
| 🔍 Búsqueda por título     | <img src="S10_GameVault/app/src/imagenes/busqueda-titulo.jpg" width="35%"> |

---

## **Tecnologías Utilizadas - Semana 10**

- 🧩 Kotlin
- 🔐 Firebase Authentication
- 🌐 Firebase Realtime Database
- 📱 Android Studio
- 📦 RecyclerView

---

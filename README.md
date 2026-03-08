# 🎥 CineApp: Arquitectura Backend con Flask

Este repositorio funciona como un **Case Study** sobre el desarrollo de una plataforma de gestión de contenidos utilizando Python y Flask. El foco principal del proyecto es la implementación de un backend sólido y la aplicación del patrón arquitectónico MVC.

> **Refactorización en curso:** El código fuente se encuentra en un repositorio privado mientras se migra la integración de servicios hacia APIs oficiales (YouTube SDK) y se optimiza la capa de modelos.

---

## 🛠️ Stack Tecnológico

* **Backend:** Python & Flask.
* **Arquitectura:** MVC (Model-View-Controller).
* **Frontend:** CSS personalizado.
* **API Integration:** Consumo de TMDb API desde el servidor (Python requests).

---

## 💡 Desafíos de Ingeniería Backend

### 1. Patrón MVC y Modularidad
A diferencia de aplicaciones monolíticas simples, CineApp separa la lógica de las rutas (Controller), el renderizado de plantillas (View) y la gestión de datos (Model). Esto facilita el mantenimiento y la escalabilidad del sistema.

### 2. Abstracción de Endpoints Externos
Desarrollé una capa de servicios en Python para centralizar las llamadas a la API de TMDb. Esto permite que, si la API externa cambia, solo sea necesario modificar un archivo en el servidor, sin afectar al resto de la aplicación.

### 3. Gestión de Seguridad y Entorno
Implementación de `python-dotenv` para proteger las API Keys y configuraciones del servidor, garantizando que ninguna credencial sensible sea expuesta en el historial de versiones.

---

## 📸 Análisis de Interfaz (Desktop & Web)

*(Espacio para capturas de pantalla)*

---

## 🚀 Roadmap de Mejora
* **Migración a SQLAlchemy:** Implementación de un ORM para persistencia de datos de usuario.
* **Caché de Servidor:** Implementación de Redis o caché simple para reducir las llamadas repetitivas a la API externa.
* **Integración Legal:** Conexión final con YouTube Player API para trailers.

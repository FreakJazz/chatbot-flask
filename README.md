# 🤖 Chatbot Web con Flask + Gemini AI

Este proyecto es una aplicación web desarrollada con **Python Flask** que permite a los usuarios chatear con una **Inteligencia Artificial (IA)** de Google Gemini. Utiliza la API de Google Generative AI y guarda las conversaciones en una base de datos SQLite. Incluye una interfaz con Bootstrap y la opción de borrar el historial.

---

## 🧠 ¿Qué es Gemini?

[Gemini](https://deepmind.google/technologies/gemini/) es el modelo de lenguaje de Google para generación de contenido, competencia de GPT, capaz de mantener conversaciones contextuales, responder preguntas, resumir textos y mucho más.

---

## 🚀 Características del proyecto

- Conexión a Gemini AI mediante API
- Interfaz con Bootstrap 5
- Simulación de chat en tiempo real
- Almacenamiento de mensajes en SQLite
- Funcionalidad para borrar historial
- Uso de variables de entorno con `.env`

---

## 📁 Estructura del Proyecto

chatbot-flask/
│
├── app.py
├── templates/
│ └── index.html
├── chat.db
├── .env
└── README.md

---

## ⚙️ Requisitos

- Python 3.8 o superior
- Cuenta en Google AI Studio para obtener una API Key:
  👉 https://aistudio.google.com/app/apikey

---

## 📦 Instalación

1. Clona el repositorio:

```bash
  git clone https://github.com/FreakJazz/chatbot-flask.git
  cd chat_gemini
```

## 📁 Estructura del Proyecto


├── app.py
├── requirements.txt
├── Procfile
├── database.db # opcional: si deseas subir la BD directamente
├── templates/

## 📦 Instalación local

1. Clona el repositorio:

  ```bash
    git clone https://github.com/tu-usuario/tu-repo.git
    cd tu-repo
    python -m venv venv
    venv\Scripts\activate
    pip install -r requirements.txt
    gunicorn app:app
  ```

## ▶️ Ejecuta la aplicación localmente

1. Asegúrate de haber instalado las dependencias con:

  ```bash
    pip install -r requirements.txt
    python app.py
  ```

## 📄 Archivo requirements.txt

Flask
gunicorn

##  ⚙️ Archivo Procfile

## ☁️ 2. Crear Web Service en Render

1. Accede a [https://render.com](https://render.com) y crea una cuenta o inicia sesión.
2. Haz clic en **"New" > "Web Service"** desde el panel de control.
3. Conecta tu cuenta de GitHub si es la primera vez.
4. Selecciona el repositorio donde está tu proyecto Flask.
5. En la configuración del servicio, completa lo siguiente:

   - **Name:** Nombre que desees para el servicio.
   - **Environment:** Python
   - **Region:** Selecciona la más cercana (ej. US Central, Latin America si está disponible).
   - **Branch:** `main` (o la rama donde está tu código).
   - **Build Command:**  

     ```bash
     pip install -r requirements.txt
     ```

     (puede dejarse vacío si ya está configurado correctamente).
   - **Start Command:**  
     ```bash
     gunicorn app:app
     ```
     
     > Asegúrate de que `app.py` sea tu archivo principal y que el objeto de Flask se llame `app`.

6. Haz clic en **"Create Web Service"**.
7. Render instalará automáticamente tus dependencias, ejecutará el proyecto y mostrará la URL pública cuando esté listo.

---

## 🧠 Consideraciones sobre SQLite

- Render no guarda archivos modificados en el disco después del reinicio (su sistema de archivos es **efímero**).
- Si tu app **solo lee** el archivo `.db`, puedes incluirlo en tu repositorio.
- Si necesitas **escribir** en la base de datos y mantener la persistencia entre reinicios, se recomienda usar un servicio de base de datos como **Render PostgreSQL** (tienen un plan gratuito).

---

## ✅ Buenas prácticas

- Asegúrate de poner `debug=False` en producción.
- Usa `.env` o variables de entorno para proteger claves y configuraciones sensibles.
- No subas datos privados en la base de datos SQLite si está dentro del repo.
- Usa control de versiones y documentación para facilitar mantenimiento y colaboración.

---

## 🧑‍💻 Autor

**Tu Nombre**  
🔗 [GitHub](https://github.com/FreakJazz)

---

## 📝 Licencia

Este proyecto se distribuye bajo la licencia GNU GENERAL PUBLIC LICENSE.

---

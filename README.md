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
  git clone https://github.com/tu_usuario/chat_gemini.git
  cd chat_gemini
```

# 🔥 Firebase Local Emulator Suite (FLES) - Lab

Este repositorio es un laboratorio de aprendizaje para el desarrollo local con Firebase en entornos modernos (**WSL2 + VS Code**). El objetivo es probar servicios de forma aislada y end-to-end sin tocar la nube ni generar costes.

## 🚀 Requisitos Rápidos (WSL / Ubuntu)
- **Node.js**: v20+ (Detectado: v24.x)
- **Java**: JRE 11+ (Necesario para los emuladores)
- **Firebase CLI**: `npm install -g firebase-tools`

## 🛠️ Configuración Inicial
1. Clonar el repo: `git clone <tu-repo>`
2. Instalar dependencias: `npm install`
3. Iniciar emuladores:

   ```bash
   firebase emulators:start --import=./seed --export-on-exit

## ⚙ Servicios de Firebase

| Servicio | Función en el Emulador |
| :--- | :--- |
| **Authentication** | Simula creación de usuarios, logins y tokens (sin enviar emails reales). |
| **Firestore** | Base de datos NoSQL con soporte completo para Security Rules. |
| **Realtime Database** | La base de datos original de Firebase en tiempo real. |
| **Cloud Functions** | Ejecuta tus funciones en Node.js ante eventos de otros emuladores. |
| **Cloud Storage** | Almacenamiento de archivos (imágenes, PDFs) local. |
| **Pub/Sub** | Emula mensajería asíncrona para arquitecturas dirigidas por eventos. |
| **Hosting** | Sirve tu contenido estático localmente. |
| **Eventarc** | Para capturar eventos de GCP (en fase beta en el emulador). |

## ⌨️ Comandos Útiles

| Acción | Comando |
| :--- | :--- |
| **Iniciar Emuladores** | `firebase emulators:start` |
| **Iniciar con Datos** | `firebase emulators:start --import=./data` |
| **Exportar Datos Manual** | `firebase emulators:export ./data` |
| **Limpiar Estado** | `rm -rf ./data` |

## Recursos de Aprendizaje de Google
Recursos oficiales:

* **Codelab Oficial:** [Local Development with the Firebase Emulator Suite](https://firebase.google.com/codelabs/firebase-emulator) - Es la base perfecta.
* **Arquitecturas de Referencia:** [Firebase for Web](https://firebase.google.com/docs/web/setup) - Para entender cómo conectar tu app al emulador mediante `connectFirestoreEmulator`.
* **Documentación:** [Introduction to Local Emulator Suite](https://firebase.google.com/docs/emulator-suite).


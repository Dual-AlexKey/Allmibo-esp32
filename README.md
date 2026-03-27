# 📱 ESP32 EasyCon - Amiibo Emulator - Android App (Bluetooth Mod)

Esta es la aplicación complementaria para el proyecto de emulación de Amiibos con ESP32 (EasyCon Mod). Permite gestionar e inyectar archivos `.bin` de Amiibos hacia tu consola Nintendo Switch de forma completamente inalámbrica, utilizando una conexión Bluetooth.

## ✨ Características Principales
* **Gestión Inalámbrica:** Olvídate de los cables. Envía tus Amiibos desde tu celular al ESP32.
* **Inyección Rápida:** Carga archivos `.bin` desde el almacenamiento de tu teléfono en segundos.
* **Portabilidad Total:** Al usar Bluetooth, puedes alimentar tu ESP32 con una simple Power Bank o cargador de celular y llevar tus Amiibos a donde quieras.

## 🛠️ Requisitos Previos
* Un dispositivo Android.
* Una placa ESP32 previamente flasheada con el firmware de EasyCon.
* Un módulo Bluetooth HC-06 conectado al ESP32 (TX a RX0, y RX a TX0) y configurado a **115200 baudios**.

## 📥 Instalación de la Aplicación (APK)

1. Ve y descarga el archivo `AmiiDrop.apk` en tu dispotivo android.
2. Instala el APK y concédele los permisos necesarios (Bluetooth y acceso a archivos).

## 🚀 Guía de Uso Rápido

1. **Sincronización Inicial:** * Enciende tu placa ESP32.
   * Ve a los ajustes de Bluetooth de tu teléfono, busca el dispositivo (usualmente llamado `HC-06`) y vincúlalo. El PIN por defecto suele ser `1234` o `0000`.
2. **Conexión en la App:** * Abre la aplicación **AmiiDrop**.
   * Presiona el botón verde de **Conectar** y automaticamente selecionara tu HC-06 si es que lo has vinculado antes.
     
     <img width="441" height="78" alt="image" src="https://github.com/user-attachments/assets/e7017e0a-c431-472d-89d1-3ade8280eb40" />
3. **Cargar el Amiibo:** * Selecciona una ranura (slot) disponible en la app.
   * Busca y selecciona el archivo `.bin` de tu Amiibo en el almacenamiento de tu teléfono.
     <img width="417" height="192" alt="image" src="https://github.com/user-attachments/assets/3f474d14-14cb-44a3-ab45-e6e780a6a40c" />
4. **Sincronizar con la Switch:**
   * En tu Nintendo Switch, ve a **Controles > Cambiar modo de sujeción u orden**.
   * Desde la app o mediante el ESP32, activa el mando virtual. La consola lo detectará como un control Pro.
     <img width="408" height="244" alt="image" src="https://github.com/user-attachments/assets/e1adf791-db41-417d-9045-182aaab958b6" />
5. **¡A jugar!:** Cuando el juego te pida colocar el Amiibo, utiliza la aplicación para inyectar el archivo y la consola lo leerá instantáneamente.

---
**Autor:** Dual-AlexKey

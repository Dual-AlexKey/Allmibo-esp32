# 🎮 ESP32 EasyCon - Amiibo Emulator (Web Serial)

Este proyecto convierte un microcontrolador ESP32 en un control Pro emulado para Nintendo Switch, con la capacidad especial de inyectar Amiibos (NFC) mediante archivos `.bin`. Además, cuenta con una interfaz web que funciona como un mando virtual (D-pad y botones X, Y, A y B) para controlar la consola directamente desde el navegador.

## 🛠️ Requisitos de Hardware
* 1x Placa ESP32 (NodeMCU / DevKit).
* Consola Nintendo Switch.
* Cable USB para conexión de datos al PC.

## ⚙️ Pasos de Instalación (Flasheo)

1. **Descargar el Firmware Base:** Primero, debes descargar el sistema EasyCon desde su repositorio oficial:
   [Repositorio EasyMCU_ESP32](https://github.com/EasyConNS/EasyMCU_ESP32?tab=readme-ov-file)

2. **Flashear el ESP32:**
   Utilizando la aplicación oficial **Flash Download Tool** de Espressif, sube el archivo `.bin` principal utilizando exactamente la siguiente configuración:

   <img width="430" height="688" alt="Configuración de Flash Download Tool" src="https://github.com/user-attachments/assets/eb277aed-90d9-473d-8f53-fb822341f73e" />

## 🚀 Guía de Uso (Interfaz Web HTML)

Una vez que el ESP32 tenga el firmware instalado, sigue estos pasos para inyectar tus Amiibos:

1. **Conectar la placa:** Conecta el ESP32 a tu PC mediante el cable USB.
2. **Abrir el Gestor:** Abre el archivo `.html` de la interfaz en tu navegador basado en Chromium (Chrome, Edge, etc.).
3. **Enlazar:** Presiona el botón **"🔌 Conectar ESP32 (USB)"** y selecciona el puerto de tu placa.
4. **Cargar el Amiibo:** Haz clic en **"📥 Quemar nuevo .bin"** y selecciona el archivo de tu Amiibo. Al hacerlo, se desbloquearán 3 nuevas opciones en la interfaz:
   * **⚡ Activar y Usar Mando** (Para iniciar la emulación).
   * **🔄 Reemplazar Amiibo** (Para cargar un archivo `.bin` diferente).
   * **❌ Desvincular** (Elimina el Amiibo de la interfaz visual).
5. **Sincronizar con la Switch:** * Haz clic en **"⚡ Activar y Usar Mando"**.
   * En tu Nintendo Switch, dirígete a **Controles > Cambiar modo de sujeción u orden**.
   * El ESP32 se sincronizará y aparecerá en la pantalla como un control Pro.
6. **¡A jugar!:** Utiliza el mando virtual de la página HTML para seleccionar el juego donde deseas usar el Amiibo. La consola lo detectará automáticamente.

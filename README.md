# Open Colorimeter - Guía de Instalación

Este repositorio contiene los pasos y archivos necesarios para instalar y ejecutar el **Open Colorimeter de IO Rodeo** usando una placa Adafruit PyBadge.

---

## 📦 Requisitos

- Arduino IDE instalado (opcional, si vas a cargar otro firmware)
- Cable USB que permita transferencia de datos
- Archivos del firmware (.zip)
- Bootloader v3.14
- CircuitPython 7.3.2
- Librerías de Adafruit necesarias

---

## ⬇️ Descarga y actualización del firmware

### Instrucciones:

1. Descargue el archivo `.zip` con la **última versión del firmware** (disponible en la carpeta `firmware/` de este repositorio o desde el sitio oficial).
2. Extraiga el contenido del `.zip` en su computadora.
3. Conecte el PyBadge a su PC y asegúrese de que aparece como unidad `CIRCUITPY`.
4. **Elimine cualquier firmware anterior** de la unidad `CIRCUITPY`.
5. Copie los nuevos archivos del firmware a la unidad `CIRCUITPY`.

---

## 🧰 Instalación del Bootloader y CircuitPython

> Antes de instalar el firmware del colorímetro, asegúrese de que su PyBadge tiene la versión correcta del bootloader y CircuitPython.

### 🛠️ Paso 1: Cambiar al modo de arranque (bootloader mode)

1. 🔌 Conecte su PyBadge a la computadora con un cable USB **de datos** (no solo de carga).
2. 🔁 Presione **dos veces rápidamente** el botón `RESET` (el botón blanco pequeño en la parte posterior o lateral del PyBadge).
3. La pantalla debería cambiar a color verde o azul.
4. En su PC aparecerá una nueva unidad llamada `BADGEBOOT` o `ARCADE`.

---

### 🧱 Paso 2: Instalar el Bootloader v3.14

1. Descargue el archivo del bootloader desde este enlace:
   - 🔗 [`update-bootloader-arcade_pybadge-v3.14.0.uf2`](bootloader/update-bootloader-arcade_pybadge-v3.14.0.uf2)
2. Arrastre ese archivo `.uf2` a la unidad `BADGEBOOT`.
3. El PyBadge se reiniciará automáticamente después de copiar el archivo.

---

### 🐍 Paso 3: Instalar CircuitPython 7.3.2

1. Presione dos veces nuevamente el botón `RESET` para volver al modo `BADGEBOOT`.
2. Descargue CircuitPython desde este enlace:
   - 🔗 [`adafruit-circuitpython-pybadge-en_US-7.3.2.uf2`](circuitpython/adafruit-circuitpython-pybadge-en_US-7.3.2.uf2)
3. Arrastre ese archivo `.uf2` a la unidad `BADGEBOOT`.
4. El PyBadge se reiniciará y aparecerá una nueva unidad llamada `CIRCUITPY`.

---

### ✅ Paso 4: Verificar instalación

- Si todo está correcto, su computadora mostrará una unidad llamada `CIRCUITPY`.
- El PyBadge estará listo para recibir el firmware del colorímetro.

---

## 📂 Estructura del repositorio


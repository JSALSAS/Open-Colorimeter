# 🎨 Open Colorimeter - Guía de Instalación y Configuración

Bienvenido/a al repositorio oficial de instalación del **Open Colorimeter de IO Rodeo**, un dispositivo portátil para análisis colorimétrico basado en hardware abierto. Este proyecto está diseñado para facilitar su uso en aplicaciones educativas, científicas y de investigación.

---

## 📸 Modelo del dispositivo

![Modelo del Open Colorimeter](images/open_colorimeter_modelo.jpg)

---

## 📦 Requisitos del sistema

### 🔧 Componentes del Open Colorimeter

- Adafruit PyBadge (versión original o LC)
- Sensor de luz **TSL2591**
- Pantalla TFT incorporada en el PyBadge
- Fuente de alimentación por USB o batería LiPo
- Impresora 3D para la carcasa (opcional pero recomendada)
- Cable USB **con transferencia de datos**

### 🖥️ Software y archivos necesarios

- [Arduino IDE](https://www.arduino.cc/en/software) (opcional, si se desea cargar firmware personalizado)
- Bootloader actualizado: `v3.14`
- CircuitPython versión: `7.3.2`
- Firmware del colorímetro (`.zip`)
- Librerías de Adafruit requeridas

---

## 📁 Archivos disponibles en este repositorio

- [`firmware/`](firmware/) → Última versión del firmware del colorímetro (`.zip`)
- [`bootloader/`](bootloader/) → Archivo `.uf2` para actualizar el bootloader
- [`circuitpython/`](circuitpython/) → Archivo `.uf2` de CircuitPython v7.3.2
- [`libraries/`](libraries/) → Librerías necesarias para CircuitPython
- [`images/`](images/) → Imágenes de referencia del dispositivo y su configuración

---

## 🔄 Instalación del firmware

### 📥 Paso 1: Descargar y copiar el firmware

1. Descargue el archivo `.zip` desde [`firmware/`](firmware/).
2. Extraiga el contenido del `.zip` en su computadora.
3. Conecte el PyBadge a la computadora: debe aparecer como unidad `CIRCUITPY`.
4. Elimine cualquier firmware anterior.
5. Copie los archivos nuevos del firmware extraído a la unidad `CIRCUITPY`.

---

## 🔃 Actualización del bootloader y CircuitPython

> ⚠️ **Importante:** Para el funcionamiento correcto del colorímetro, es necesario que el PyBadge utilice el bootloader v3.14 y CircuitPython 7.3.2.

### 🛠️ Paso 2: Entrar en modo bootloader

1. Conecte el PyBadge a su PC con un cable USB **de datos**.
2. Presione dos veces rápidamente el botón `RESET`.
3. El dispositivo mostrará una pantalla azul o verde.
4. Aparecerá una unidad nueva llamada `BADGEBOOT` o `ARCADE`.

---

### 🧱 Paso 3: Instalar Bootloader v3.14

1. Descargue el archivo `.uf2` desde [`bootloader/`](bootloader/).
2. Arrastre el archivo `update-bootloader-arcade_pybadge-v3.14.0.uf2` a la unidad `BADGEBOOT`.
3. El PyBadge se reiniciará automáticamente.

---

### 🐍 Paso 4: Instalar CircuitPython 7.3.2

1. Presione dos veces el botón `RESET` para entrar nuevamente a `BADGEBOOT`.
2. Descargue el archivo `.uf2` desde [`circuitpython/`](circuitpython/).
3. Arrastre `adafruit-circuitpython-pybadge-en_US-7.3.2.uf2` a `BADGEBOOT`.
4. El PyBadge se reiniciará y se mostrará una nueva unidad llamada `CIRCUITPY`.

---

## ✅ Paso 5: Verificación

- Si todo ha salido bien, debe ver una unidad `CIRCUITPY` en su PC.
- El colorímetro está ahora listo para usarse con el nuevo firmware.

---

## 📚 Créditos

Proyecto basado en el diseño de código abierto de [IO Rodeo](https://iorodeo.com)  
Repositorio oficial de código original: [https://github.com/iorodeo/colorimeter](https://github.com/iorodeo/colorimeter)

---

## 🧪 Contacto y soporte

Para reportar errores, sugerencias o contribuir, puedes crear un **Issue** o enviar un **Pull Request** a este repositorio.

---



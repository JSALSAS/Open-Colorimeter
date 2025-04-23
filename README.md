# Open Colorimeter - Guía de Instalación y Configuración

Este repositorio contiene todos los archivos necesarios y una guía detallada para instalar y configurar el **Open Colorimeter de IO Rodeo**, un dispositivo portátil de código abierto diseñado para realizar análisis colorimétricos con precisión. Es ideal para uso educativo, científico y experimental.

---

## Modelo del dispositivo

<img src="image_1.png" alt="Open Colorimeter" width="500"/>

---

## 📦 Requisitos

### Componentes de hardware

Asegúrate de contar con los siguientes elementos físicos:

- ✅ Adafruit PyBadge (modelo original o LC)
- ✅ Sensor TSL2591 (sensor de luz digital)
- ✅ Pantalla TFT incorporada (en el PyBadge)
- ✅ Cable USB **de datos** (no solo carga)
- ✅ Carcasa impresa en 3D (opcional pero recomendada)

### Archivos incluidos en este repositorio

Todos los archivos requeridos se encuentran organizados en las siguientes carpetas:

| Carpeta                       | Contenido                                           |
|------------------------------|----------------------------------------------------|
| `open_colorimeter_firmware_v0.1.1/` | Archivos del firmware principal del colorímetro |
| `bootloader v3.14/`          | Archivo `.uf2` para actualizar el bootloader       |
| `circuitpython 7.3.2/`       | Archivo `.uf2` para instalar CircuitPython 7.3.2   |

---

## Instrucciones de instalación

###  Paso 1: Instalar el firmware del colorímetro

1. Ve a la carpeta `open_colorimeter_firmware_v0.1.1/` y copia todos los archivos a tu computadora.
2. Conecta el PyBadge a tu PC: debe aparecer como unidad `CIRCUITPY`.
3. Elimina cualquier archivo antiguo dentro de `CIRCUITPY`.
4. Copia los nuevos archivos del firmware dentro de la unidad `CIRCUITPY`.

---

##  Actualización del sistema del PyBadge

> ⚠️ Este proceso es **necesario si tu PyBadge no tiene el bootloader o CircuitPython correctos**.

### Paso 2: Activar el modo bootloader

1. Conecta el PyBadge a tu PC usando un cable USB **de datos**.
2. Presiona dos veces rápidamente el botón `RESET` en la parte posterior o lateral.
3. Verás que la pantalla cambia (color azul o verde) y aparecerá una unidad nueva llamada `BADGEBOOT` o `ARCADE`.

---

### Paso 3: Instalar bootloader v3.14

1. Ve a la carpeta `bootloader v3.14/`.
2. Copia el archivo `.uf2` que está ahí a la unidad `BADGEBOOT`.
3. El PyBadge se reiniciará automáticamente una vez copiado.

---

### Paso 4: Instalar CircuitPython 7.3.2

1. Vuelve a poner el PyBadge en modo bootloader si es necesario (presionando `RESET` dos veces).
2. Ve a la carpeta `circuitpython 7.3.2/`.
3. Copia el archivo `.uf2` dentro de `BADGEBOOT`.
4. El dispositivo se reiniciará y mostrará la unidad `CIRCUITPY`.

---

## Paso 5: Verificar

- La unidad `CIRCUITPY` debe estar visible en tu PC.
- El PyBadge debe mostrar la interfaz del colorímetro en su pantalla.
- El sistema está listo para ser utilizado.

---

## Créditos

Este proyecto se basa en el diseño de código abierto desarrollado por [IO Rodeo](https://iorodeo.com).  
Repositorio oficial del firmware original:  
🔗 [https://github.com/iorodeo/open_colorimeter_firmware/releases](https://github.com/iorodeo/open_colorimeter_firmware/releases)

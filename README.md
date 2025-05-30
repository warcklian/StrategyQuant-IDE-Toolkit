# StrategyQuant-IDE-Toolkit

**Versión:** 0.9.4-beta1  
**Autor:** Jorge Octavio Gómez González  
**Telegram:** [Grupo de soporte y discusión](https://t.me/g69I5IygZJNlZTJh)  
**Licencia:** MIT

---

## ¿Qué es StrategyQuant-IDE-Toolkit?

Es un entorno de desarrollo profesional, multiplataforma (versión inicial para Windows) orientado a traders algorítmicos, quants y programadores que trabajan con **StrategyQuant X**. Permite crear, editar, compilar, organizar y exportar estrategias, indicadores y plantillas, con un enfoque moderno tipo Visual Studio Code. 

El editor soporta múltiples pestañas, resaltado de sintaxis avanzado, temas personalizados, integración con carpetas y paquetes `.zip`, `.sxp`, `.spx` y exportación directa a tu instalación de StrategyQuant.

---

## Características principales

- **Edición y creación profesional** de archivos `.sqx`, `.java`, `.mq4`, `.mq5`, `.js`, `.html`, `.tpl`, `.csv`, `.txt`, `.py`, `.c`, `.cpp`, `.json`, entre otros.
- **Apertura de paquetes comprimidos** (.zip, .sxp, .spx): los descomprime en carpetas temporales y permite navegar y editar cualquier archivo del paquete (sin sobrescribir el original).
- **Árbol lateral estilo VSCode:** muestra toda la estructura de archivos/carpetas, permite doble click para abrir cualquier recurso.
- **Detección y guardado inteligente:** identifica si es indicador o estrategia, y lo guarda en la carpeta correspondiente (`custom_indicators` o `strategies`).
- **Exportación a StrategyQuant** en un solo clic.
- **Reempaquetado de archivos:** Empaqueta cambios a .zip, .sxp o la extensión original del paquete.
- **Soporte multitema** (oscuro, claro, azul, cyan, sepia, Nord, Gruvbox, etc).
- **Resaltado de sintaxis** contextual y adaptable al tema.
- **Soporte para atajos estándar:** Ctrl+N (Nuevo), Ctrl+O (Abrir), Ctrl+S (Guardar), Ctrl+Shift+S (Guardar como...), Ctrl+E (Exportar a StrategyQuant), F7 (Compilar), F1 (Ayuda).

---

#######################################################################################################################

## Instalación y dependencias

### Descarga para usuarios finales

**No es necesario instalar Python ni dependencias!**  
Solo descarga el `.exe` desde la sección Releases.

> **IMPORTANTE:**  
> El programa requiere tener instalado Java 8 (OpenJDK 8).  
> Descarga el instalador oficial aquí:  
> [OpenJDK8U-jdk_x64_windows_hotspot_8u452b09.msi](https://github.com/adoptium/temurin8-binaries/releases)

### Versión fuente para desarrolladores

Requiere Python 3.10+ y PyQt5, chardet, etc.  
Ejecuta:

```bash
pip install pyqt5 chardet
python main.py
Cómo se usa
Ejecuta StrategyQuant-IDE-Toolkit.exe o python main.py

#######################################################################################################################


### Tema Personalizado (Custom)

Puedes definir tu propio esquema de colores para todo el editor mediante un archivo externo llamado `custom_theme.json`. Si seleccionas el tema **Custom** desde el menú de temas, el programa leerá y aplicará automáticamente tus preferencias de color.

**¿Cómo personalizar tu tema?**

1. Crea un archivo llamado `custom_theme.json` en la misma carpeta donde está el `.exe` (o `main.py` si usas la versión fuente).
2. Ejemplo de estructura de `custom_theme.json`:

```json
{
    "name": "Custom",
    "background": "#222034",
    "foreground": "#e6e6e6",
    "highlight": "#39c5bb",
    "selection": "#234060",
    "menubar_bg": "#232537",
    "menubar_fg": "#b9e6ff",
    "menubar_active": "#39c5bb",
    "editor_bg": "#222034",
    "editor_fg": "#e6e6e6",
    "border": "#446688"
}
Cambia cualquier color hexadecimal a tu gusto. Los nombres de clave deben coincidir con los usados en el ejemplo.

Abre el programa y selecciona “Custom” en el menú Tema. Si ya estaba seleccionado, vuelve a elegirlo para recargar los cambios.

Nota:
Si editas el archivo mientras el programa está abierto, deberás volver a seleccionar el tema "Custom" en el menú para refrescarlo.


#######################################################################################################################


Usa el menú Archivo para crear, abrir o importar archivos/paquetes

Edita y navega usando el árbol lateral y las pestañas

Usa Guardar o Guardar como para persistir tus cambios. El programa detecta automáticamente la carpeta de destino para estrategias o indicadores.

Exporta el archivo actual a tu instalación de StrategyQuant para convertir a otros formatos (MQL4, MQL5, NinjaTrader, etc)

Nota. NO convierte automaticamente indicadores, estrategias etc.

Usa el menú Reempaquetar para guardar paquetes .zip, .sxp, etc.

Soporte de archivos y extensiones
El editor puede abrir y editar archivos de los siguientes tipos:

.sqx, .java (StrategyQuant nativos)

.mq4, .mq5 (MetaTrader 4/5)

.js, .py, .json, .csv, .tpl, .txt, .html, .css, .c, .cpp, .h, .ts, .ini, .md, .xml, .tpl, .mql, .mqh

.zip, .sxp, .spx (paquetes comprimidos con archivos de código o plantillas)

Navega y edita cualquier archivo texto plano (soporta autodetección de encoding con chardet)

Temas y personalización
Incluye temas:

Claro (VSCode)

Oscuro (VSCode)

Cyan Contrast

Azul Rey

Sepia Gray

Nord

Gruvbox Dark

Cambia de tema desde el menú Tema.

Atajos rápidos
Ctrl+N: Nuevo archivo

Ctrl+O: Abrir archivo

Ctrl+S: Guardar

Ctrl+Shift+S: Guardar como...

Ctrl+E: Exportar a StrategyQuant

Ctrl+Shift+O: Abrir paquete .sxp

Ctrl+Alt+Shift+O: Abrir ZIP

Ctrl+Alt+Shift+E: Reempaquetar paquete

F7: Compilar (No implementado)

F1: Ayuda

Ctrl+F1: Acerca de


#######################################################################################################################

Comunidad y soporte
¿Tienes dudas, sugerencias o errores?
Únete al grupo de Telegram: https://t.me/g69I5IygZJNlZTJh

Licencia y estado del proyecto
MIT License.

Este software es BETA. No es oficial de StrategyQuant ni tiene garantía de funcionamiento para usos críticos en producción.

Usa bajo tu propio riesgo.

Créditos
Desarrollado por Jorge Octavio Gómez González
Repositorio: github.com/warcklian


# Control Facial - Instrucciones rápidas

Requisitos mínimos:
- Python 3.8+ instalado (en Windows suele instalarse con el lanzador `py`).

Pasos recomendados (PowerShell):

1) Actualizar pip (ya lo hiciste):
```powershell
py -m pip install --upgrade pip
```

2) (Opcional pero recomendado) Crear y activar un entorno virtual:
```powershell
py -m venv .venv
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
.\.venv\Scripts\Activate.ps1
```

3) Instalar dependencias desde `requirements.txt`:
```powershell
py -m pip install -r requirements.txt
```

4) Probar importaciones rápidas:
```powershell
py test_imports.py
# o
python test_imports.py
```

5) Ejecutar el script principal:
```powershell
py control_facial.py
```

Notas útiles:
- Si `py` no existe, instala Python desde https://www.python.org/ y marca "Add Python to PATH".
- Si la cámara no funciona con índice `0`, edita `control_facial.py` y prueba `cv2.VideoCapture(1)`.
- Si `pyautogui` no puede mover o clickear, prueba ejecutar PowerShell como administrador o instalar `pywin32`.
- Asegúrate de que `haarcascade_frontalface_default.xml` esté en la misma carpeta del script.

Si quieres, puedo ejecutar los comandos de instalación por ti (los generaré para PowerShell) o probar `test_imports.py` aquí y ayudarte a interpretar la salida si pegas los mensajes.

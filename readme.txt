CUE: CONSULTAS PERSONALIZADAS 
DRILLING: PROFUNDIZANDO EN EL USO DE MANAGER.RAW()


evaluacion 
m7_s8

Para clonar:

Thelma Delgado








		
pasos para instalar DEPENDENCIAS
------------------------------------------

    1-instalar entorno virtual:
        py.exe -m venv venv
    2- activar entorno virtual
        .\venv\scripts\activate
    3- restaurar DEPENDENCIAS
        pip install -r .\requirements.txt



superuser

nombre: admin
email: admin@admin.com
clave: 123456


LOGICA 
----------------------------
logica en vista inventario/views.py -> listado_productos_view


RESPUESTAS EN TERMINAL
----------------------------
Partiendo del modelo creado en el Rebound Exercise de este CUE: 
1. Obtenga los campos de nombre, precio, y fecha de vencimiento de los productos



System check identified no issues (0 silenced).
November 24, 2024 - 21:43:35
Django version 4.2.16, using settings 'config.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.

El producto: Ariel suavizante se vence en: 2025-06-20, con un precio de : $ 1800
El producto: Champú se vence en: 2024-12-31, con un precio de : $ 2500
El producto: Colgate se vence en: 2025-06-27, con un precio de : $ 1450
El producto: Colgate 360 se vence en: 2024-12-27, con un precio de : $ 1850
El producto: Crema colgate se vence en: 2026-02-12, con un precio de : $ 1500
El producto: Crest Premiun se vence en: 2025-04-09, con un precio de : $ 2500
El producto: Downy Aroma Floral se vence en: 2025-12-19, con un precio de : $ 3500
El producto: Jabon en polvo se vence en: 2025-07-17, con un precio de : $ 3500
El producto: Protex Aloe se vence en: 2025-09-30, con un precio de : $ 1250
El producto: Speed Stick 24/7 se vence en: 2025-07-27, con un precio de : $ 4500
[24/Nov/2024 21:43:43] "GET /inventario/productos HTTP/1.1" 200 713




2. Obtenga los productos donde el precio sea menor o igual a 2500, y muestre solo los campos de nombre y precio, respectivamente.  

System check identified no issues (0 silenced).
November 24, 2024 - 23:03:05
Django version 4.2.16, using settings 'config.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.

El producto: Ariel suavizante tiene un precio de : $ 1800
El producto: Champú tiene un precio de : $ 2500
El producto: Colgate tiene un precio de : $ 1450
El producto: Colgate 360 tiene un precio de : $ 1850
El producto: Crema colgate tiene un precio de : $ 1500
El producto: Crest Premiun tiene un precio de : $ 2500
El producto: Protex Aloe tiene un precio de : $ 1250
[24/Nov/2024 23:03:33] "GET /inventario/productos HTTP/1.1" 200 7138




3. Modifique haciendo uso de SQL personalizado y cursores, la fábrica con nombre P&G
 en el país que se encuentra asignada a EEUU, o a Canadá

System check identified no issues (0 silenced).
November 25, 2024 - 09:25:31
Django version 4.2.16, using settings 'config.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.

[('Canada',)]
[25/Nov/2024 09:26:16] "GET /inventario/productos HTTP/1.1" 200 7138
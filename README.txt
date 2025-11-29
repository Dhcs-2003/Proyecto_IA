
Proyecto 2:  Problema del Coloreo del Mapa
Inteligencia Artificial I - Universidad Politécnica de San Luis Potosí
Profesor: Dr. Omar Montano Rivas
-----------------------------------------------------------------------------
Matrícula: 178378
Autor: Daniel Humberto Cano Sánchez
Fecha de entrega: 28 de Noviembre de 2025

1. Descripción
-----------------------------------------------------------------------------
Este programa resuelve el problema de satisfacción de restricciones para
el coloreo de mapas de México. Implementa:
- Algoritmo de Vuelta Atrás (Backtracking).
- Heurísticas: Mínimos Valores Restantes (MRV) y Grado Heurístico.


2. Requerimientos
-----------------------------------------------------------------------------
- .NET SDK (Versión 8.0, 9.0 o 10.0).
- Compatible con Windows, Linux y macOS.

3. Instrucciones para generar ejecutable
-----------------------------------------------------------------------------
Para compilar el código fuente y generar un ejecutable optimizado (Release),
abra una terminal en la carpeta del proyecto y ejecute:

    dotnet publish -c Release

Esto creará el archivo 'ColoreoMapa.exe' en la carpeta:
    /bin/Release/net10.0/publish/

**NOTA: El comando dotnet "publish -c Release" se debe ejecutar en la carpeta donde se encuentra
        el proyecto, en este caso ../ColoreoMapa/

**NOTA 2: Este paso solo es necesario si no se encuentra el
        archivo en la ruta /bin/Release/net10.0/publish/

4. Ejecución del programa
-----------------------------------------------------------------------------
Existen dos formas de ejecutar el programa:

OPCIÓN A (Recomendada para desarrollo - Compila y ejecuta):
    dotnet run -- <archivo.txt> <modo>

OPCIÓN B (Ejecutar el .exe generado en el paso 3):
    1. Navegue a la carpeta del ejecutable:
       cd bin/Release/net10.0/publish
    2. Copie el archivo de texto (ej. mexico_4_colores.txt) a esta carpeta.
    3. Ejecute:
       ColoreoMapa.exe <archivo.txt> <modo>

**NOTA: Este paso solo es necesario si no se encuentra el/los
        archivo(s) en la ruta /bin/Release/net10.0/publish/

5. Parámetros
-----------------------------------------------------------------------------
El <modo> puede ser:
    - simple        (Para Backtracking estándar)
    - heuristicas   (Para Backtracking con MRV y Grado)

Ejemplo:
    dotnet run -- mexico_4_colores.txt heuristicas

Archivos necesarios
-----------------------------------------------------------------------------
- Código fuente (Program.fs)
- Archivo de proyecto (ColoreoMapa.fsproj)
- Archivos de prueba (mexico_2_colores.txt, mexico_3_colores.txt, etc.)

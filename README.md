# Cuentita

Calculadora compacta para Windows 11: el resultado aparece mientras escribís la cuenta.

Este repositorio tiene solo los instaladores y las actualizaciones de Cuentita.

## Instalación

En Windows, abrí PowerShell, pegá esta línea y apretá Enter:

```powershell
iwr -UseBasicParsing https://github.com/jotapece/cuentita-releases/releases/latest/download/Cuentita-win-Setup.exe -OutFile $env:TEMP\Cuentita-win-Setup.exe; & $env:TEMP\Cuentita-win-Setup.exe
```

El comando baja el instalador a una carpeta temporal y lo ejecuta. Cuentita queda instalada solo para tu usuario, sin permisos de administrador, con un acceso en el menú Inicio.

Instalada así, Windows no muestra el aviso de SmartScreen («Windows protegió tu PC»). Ese aviso aparece con lo que se baja desde el navegador, y Cuentita no está firmada.

## Actualizaciones

Son automáticas. Unos segundos después de abrirse, Cuentita se fija si hay una versión nueva y la baja en segundo plano, sin avisar. La próxima vez que la abrís, ya arranca actualizada.

## Desinstalar

Configuración → Aplicaciones → Aplicaciones instaladas → Cuentita → Desinstalar.

El historial y la posición de la ventana quedan en `%APPDATA%\Cuentita`. Si querés borrarlos, borrá esa carpeta.

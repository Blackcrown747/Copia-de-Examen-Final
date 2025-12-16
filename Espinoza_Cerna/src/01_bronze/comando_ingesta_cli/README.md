# 1. Crear el contenedor 'bronce' dentro de tu cuenta 'bronze1'
```
az storage fs create -n bronce --account-name bronze1 --auth-mode login
```
# 2. Crear la carpeta 'raw' donde aterrizarán los datos
```
az storage fs directory create -n raw -f bronce --account-name bronze1 --auth-mode login
```
# 3. SUBIR EL ARCHIVO 
```
az storage fs file upload \
    --account-name bronze1 \
    --file-system bronce \
    --path raw/flights.csv \
    --source "C:\Ruta\A\Tu\Archivo\flights.csv" \
    --auth-mode login
```

# BodegaConvApp

Este Software ha sido desarrollado por Ignacio Gaona Vargas.

La finalidad del mismo es la conversión de ficheros excel ha un formato de campos de tamaño fijo, la converison se basa en una plantilla Json.

Ejemplos campos Json:
* Campo string:
```sh
{
    "nombrecolumna": "XX",   Aqui debemos de introducir el nombre de la columna a buscar en el excel.
    "tamano": "15",  el tamaño es obligatorio y debe de marcar el numero de caracteres que tendra dicho campo en el formato fijo
    "formato": "0X", el formato representa la visualizacion del dato, donde X es el valor leido del excel y por ejemplo '0' representa que se rellenara con 0 hasta                             completar el tamaño. Podría usarse otro tipos de caracteres como ' '.
    "orden": "0" representa el orden dentro del formato fijo de salida
  }
```

  * Campo numerico:
```sh
  {
    "nombrecolumna": "c",
    "orden": "2",
    "formato": "000,000" Aqui se hace referencia a la representación del formato numerico ejemplo : valor excel -> 10 ; valor resultante-> 010,000
}
```
*Campo Fecha:
```sh
{
    "nombrecolumna": "Fecha",
    "orden": "3",
    "formato": "ddMMyyyy"  Aqui representaremos la fecha en los formatos que deseemos (es el formato de fecha resultante)
  }
```

# Bienvenido! 
 > aqui te adjunto alguno de las herramientas que he generado o adaptado para solventar rapidamente los formatos chilenos
 > - Desarrollado en **typescript** para **npm**

## npm i andinotools
Herramienta generada para solucionar problemas con formatos chilenos
actualmente la herramienta cuenta con

 - Generar un formato de moneda chilena
 - Verificar formato de rut

### Funciones

#### rutValidator(valor: any):string 
> Verifica el formato de un *string* y retorna un *string* en blanco si la consulta fue satisfactoria, caso contrario *string* del problema.

    
|Input| Output | Descripcion |
|--|----| -- |
| 12312312X | '' | Correcto
| 123123122 | 'El rut no coincide con el cv' | Error
| 12.312.3122 | 'El formato del rut es invalido' | Error



#### moneyFormat(cantidad: number):string
> Transforma un valor numérico en un string con formato en pesos chilenos 


| Input | Output |
|--|--|
| 20140 | '$20.140' |

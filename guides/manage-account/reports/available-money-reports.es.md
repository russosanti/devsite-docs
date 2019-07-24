# ¿Qué es el Reporte de Dinero Disponible? (h1)

En esta página

    Introducción 
    Casos de uso
    Cómo usar el reporte
    Ejemplos


## Introducción

El Reporte de Dinero Disponible es un **informe descargable** en formato .csv o .xlsx que te permite conocer la liquidez de tu negocio, es decir, cuánto dinero tienes para usar. Contiene el **detalle de los pagos liberados** que están listos para retirar a una cuenta bancaria o invertir en Mercado Pago. 

Accede a tus reportes desde la sección de Informes en tu cuenta en Mercado Pago siguiendo estos pasos:
1. [Inicia sesión](https://www.mercadolibre.com/jms/mla/lgz/msl/login/H4sIAAAAAAAEAy2OQQ7DIAwE_-JzlNw59iPIIoagQo2MI1pF_XtN1OOux2NfUDjll9dPI3BA71ZyyAoLtIIaWarPuw1qs6pnpX8sOBEUrKQkHdw1RYn2B9nSVKmcZAyeevhYeFh1n7IusYVDtXW3bWOMtZIE3Llh4jVwXVE2w4RS7man-cCt-y4QsatXwfAEF7F0-v4AxU1qhMMAAAA/user) en Mercado Pago
1. Ve a [Informes](https://www.mercadopago.com/mla/account/movements) y de ahí accede a tus [Reportes](https://www.mercadopago.com.ar/balance/reports)
1. En Reportes, elige Dinero Disponible, allí encontrarás un listado de los reportes generados.

Ten en cuenta que la generación del reporte lleva un tiempo, es decir, que no siempre estará listo al instante y verás el estado “En preparación”. Una vez disponible, estará en tu bandeja de reportes y siempre lo podrás descargar de dos formas: 
* Desde un link de descarga que te enviaremos por mail
* Desde tu cuenta de Mercado Pago, en <span style="color:blue">Reportes de Dinero Disponible.</span> 

Es importante aclarar que el valor total del reporte no siempre coincide con los valores del reporte de Dinero en Cuenta o los reportes de facturación. Dependiendo de [los plazos y tasas que elijas](https://www.mercadopago.com.ar/settings/release-options), el dinero que ganes por una venta se liberará un tiempo después de acreditado el cobro. Para saber la fecha exacta en que estará disponible el dinero de una operación, revisa el detalle de tus [cobros acreditados](https://www.mercadopago.com.ar/activities/balance). 
 
Esos plazos tienen que ver con los tiempos de los bancos o por los flujos de intermediación cuando las operaciones se realizan en Mercado Libre. Otras operaciones que pueden afectar la liberación de tu dinero son los Contracargos y Reclamos que puedas recibir por una venta. 

## Casos de uso

Por lo general, **este reporte se usa para conciliar los retiros de dinero** e incluye las transacciones que lo componen. 

Generamos un Reporte de Dinero Disponible en estas tres situaciones: 
1. Cada vez que lo generas manualmente. 
1. De forma programada, según tus ajustes.
1. Con cada retiro de dinero a una cuenta bancaria. 

Usa el Reporte de Dinero Disponible en estos casos: 
* Cuando quieras tener un informe de liquidez de la cuenta,
* Para conciliar cómo están compuestas las operaciones que impactan en tu dinero disponible en un nivel transaccional,
* Conciliación mensual o periódica con el detalle de los movimientos que generan saldo disponible para retirar.
* Para conocer:
    + El historial de dinero disponible entre dos fechas o dos retiros. 
    + El detalle de los eventos que componen un retiro automático o manual, total o parcial. 
    + El detalle de disputas, reembolsos, shipping, contracargos, impuestos y otras operaciones que afecten el dinero disponible.
    + El detalle de las cuotas liberadas y de las operaciones “En cuotas”


## Cómo usar el reporte

Para leer el reporte te recomendamos usar un archivo .csv y que revises la configuración de los caracteres. Debe estar en formato UTF-8. Compruébalo en los ajustes de tu planilla de cálculo (Excel, LibreOffice Calc, etc): 

![excel](/images/manage-account/reports/excel.png)
<p style="text-align:center;">Ejemplo en Excel</p>

![open-office](/images/manage-account/reports/open-office.png)
<p style="text-align:center;">Ejemplo en Open Office</p>

El reporte contiene 4 secciones:
1. Balance Inicial (Initial Available Balance)
1. Detalle de Liberaciones de dinero (Releases)
1. Bloqueos de dinero por disputas (Block)
1. Desbloqueos por la resolución de la disputa (Unblock)

Verás una sección de **subtotales** por cada bloque y, finalmente, el **resultado total**. A este total lo calculamos sobre los subtotales netos de cada sección, es la suma neta de: 

<p style="text-align:center;">Subtotal release - Subtotal block + Subtotal unblock = resultado total</p>

Revisa el [Glosario completo](https://www.mercadopago.com.ar/ayuda/_2118)

Reflejamos los conceptos contables universales del *debe* (dinero que tienes que pagar) y *haber* (dinero que tienes por cobrar) escribiendo el reporte en dos columnas, una por cada concepto:  

<p style="padding:0 0 0 50px;">Tu haber lo verás en la columna NET_CREDIT</p>
<p style="padding:0 0 0 50px;">Tu deber estará en la columna NET_DEBIT</p>

Verás el dinero disponible de las operaciones liberadas en las columnas NET_CREDIT (acreditado) y NET_DEBIT (debitado), dependiendo de si el monto es positivo o negativo. También verás ahí el monto bruto y los gastos de financiamiento, impuestos y costos de envío que descontamos para llegar al monto neto.

<!--
<table style="border: 1px solid black;">
  <tr style="border: 1px solid black;">
    <td style="border: 1px solid black;">

**¿Quieres agregar detalles a la vista de las operaciones?** Selecciona las columnas que quieras exportar e incluir en los Ajustes del reporte, según lo que quieras analizar y conciliar. 
     </td>
  </tr>
</table>
-->

**¿Qué pasa si un retiro falla?**

Si esto pasa, el reporte sigue siendo válido. El dinero vuelve a tu cuenta y la operación aparecerá en el reporte como una nueva línea en la columna NET_CREDIT.

### Ejemplos

Observa cómo está compuesto el reporte de dinero disponible en este ejemplo para identificar las secciones y leer tus propios reportes:

![examples](/images/manage-account/reports/examples.png =200x)

La versión por defecto mostrará una vista extendida de las columnas. El informe final tendrá la mayor cantidad de detalle posible. Si quieres menos detalle o hay columnas que no te sirven para la conciliación, puedes modificar cuáles incluir y cuáles no en Ajustes.  

<table>
  <tr>
    <td style="border: 1px solid black;width:50%">

**Importante: diferencias entre retiro parcial y retiro total.**

Cuando retires todo tu dinero disponible, el total del reporte va a coincidir con ese monto. En cambio, cuando hagas un retiro parcial, que no incluya la totalidad de tu dinero en cuenta liberado, el total de dinero disponible y el total del reporte no van a coincidir. 

Por ejemplo, imagina que tienes $ 3.000 disponibles para retirar a una cuenta bancaria pero solo retiras $ 2.000. El retiro es parcial pero el valor total del reporte seguirá mostrándote el monto del balance inicial que había al momento del retiro, es decir, los $ 3.000 que tenías disponibles. En cambio, si retiras los $ 3.000, el valor total del reporte va a coincidir con el valor de ese retiro. 
     </td>
     <td ></td>
  </tr>
</table>

# >Próximos pasos Cards

# Cómo generar tus reportes

## Vía web

Desde tu panel de Mercado Pago, solo podrás programar los reportes por retiro. Seguí estos pasos para hacerlo:

1. Iniciá sesión en Mercado Pago
1. Ve a Informes y de ahí accede a tus Reportes
1. En Reportes, elige Dinero Disponible.
1. Una vez dentro de Dinero Disponible, clickea en **‘Generar reporte’**
1. Selecciona el **período de tiempo** que quieras incluir en el reporte

¡Y listo! Vas a ver que el reporte está **en preparación.** 

Gana tiempo programando la **frecuencia de generación** de reportes. Guarda los ajustes para automatizar cada preparación, ya sea manual o de forma programada.

## Vía API

### De forma manual

1. Generación

Haz el POST a la API especificando las fechas de inicio y fin de la siguiente manera:

[[[
```curl
curl -X POST \
    -H 'accept: application/json' \
    -H 'content-type: application/json' \
    'https://api.mercadopago.com/v1/account/bank_report?access_token=ACCESS_TOKEN' \
    -d '{
            "begin_date": "2019-05-01T00:00:00Z",
            "end_date": "2019-06-01T00:00:00Z"
    }'
```
```Python
import requests

headers = {
    'accept': 'application/json',
    'content-type': 'application/json',
}
params = { 'access_token', 'ACCESS_TOKEN' }
data = '{ "begin_date": "2019-05-01T00:00:00Z", "end_date": "2019-06-01T00:00:00Z" }'

response = requests.post('https://api.mercadopago.com/v1/account/bank_report', headers=headers, params=params, data=data)

```
```node
var request = require('request');

var headers = { 'accept': 'application/json', 'content-type': 'application/json' };

var dataString = '{ "begin_date": "2019-05-01T00:00:00Z", "end_date": "2019-06-01T00:00:00Z" }';

var options = {
    url: 'https://api.mercadopago.com/v1/account/bank_report?access_token=ACCESS_TOKEN',
    method: 'POST',
    headers: headers,
    body: dataString
};
function callback(error, response, body) {
    if (!error && response.statusCode == 200) {
        console.log(body);
    }
}
request(options, callback);
```
]]]

Recibirás como respuesta un HTTP STATUS 202 (Accepted), y el reporte se generará de manera asincrónica.

2. Búsqueda

Consulta la API de esta forma para ver si la generación de reportes quedó lista:

[[[
```curl
curl -G \
    -H 'accept: application/json' \
    -d 'access_token=ACCESS_TOKEN' \
    'https://api.mercadopago.com/v1/account/bank_report/list'
```
```Python
import requests
headers = { 'accept': 'application/json' }
data = { 'access_token': 'ACCESS_TOKEN' }
response = requests.post('https://api.mercadopago.com/v1/account/bank_report/list', headers=headers, data=data)
```
```node
var request = require('request');
var headers = { 'accept': 'application/json'};
var dataString = 'access_token=ACCESS_TOKEN';
var options = {
    url: 'https://api.mercadopago.com/v1/account/bank_report/list',
    method: 'POST',
    headers: headers,
    body: dataString
};
function callback(error, response, body) {
    if (!error && response.statusCode == 200) {
        console.log(body);
    }
}
request(options, callback);

```
]]]

Recibirás como respuesta:
```json
[
    {
        "id": 1234,
        "user_id": 130379930,
        "begin_date": "2015-05-01T00:00:00Z",
        "end_date": "2015-06-01T00:00:00Z",
        "file_name": "BK-TEST-1234567890123.csv",
        "created_from": "manual",
        "date_created": "2016-01-20T10:07:53.000-04:00"
    },
    {
    	...
    }
]
```

3. Descarga

Utilizando el atributo file_name, puedes descargar el reporte desde la siguiente URL:

```curl
curl -X GET 'https://api.mercadopago.com/v1/account/bank_report/:file_name?access_token=ACCESS_TOKEN' 
```

Recibirás como respuesta:

```json
DATE,SOURCE_ID,EXTERNAL_REFERENCE,RECORD_TYPE,DESCRIPTION,NET_CREDIT_AMOUNT,NET_DEBIT_AMOUNT,GROSS_AMOUNT,MP_FEE_AMOUNT,FINANCING_FEE_AMOUNT,SHIPPING_FEE_AMOUNT,TAXES_AMOUNT,COUPON_AMOUNT,INSTALLMENTS,PAYMENT_METHOD
2018-04-17T15:07:53.000-04:00,,,initial_available_balance,,813439.19,0.00,813439.19,0.00,0.00,0.00,0.00,0.00,1,
2018-04-17T15:07:53.000-04:00,,,release,withdrawal,0.00,813363.45,-813360.45,-3.00,0.00,0.00,0.00,0.00,1,
2018-04-17T15:11:12.000-04:00,,,release,payment,225.96,0.00,269.00,-43.04,0.00,0.00,0.00,0.00,1,account_money
2018-04-17T15:18:16.000-04:00,,,release,payment,124.32,0.00,148.00,-23.68,0.00,0.00,0.00,0.00,1,visa
2018-04-17T15:38:40.000-04:00,,,release,payment,820.14,0.00,1099.00,-278.86,0.00,0.00,0.00,0.00,6,visa
2018-04-17T15:38:40.000-04:00,,,release,payment,850.00,0.00,850.00,0.00,0.00,0.00,0.00,0.00,1,account_money
```

**Response status code: 200 OK**


### De forma programada

1. Generación

Programa la generación automática del reporte utilizando la frecuencia en el recurso de configuración. Actualiza el atributo scheduled en la configuración a true ([Ver](#actualizar-configuración)):

```curl
curl -X POST \
    -H 'accept: application/json' \
    -H 'content-type: application/json' \
    'https://api.mercadopago.com/v1/account/bank_report/schedule?access_token=ACCESS_TOKEN' \
    -d '{
        "user_id": USER-ID
    }'
``` 

Recibirás como respuesta:

```json
{
    "id": 2541818,
    "user_id": USER-ID,
    "begin_date": "2019-07-01T06:00:00Z",
    "end_date": "2019-08-01T06:00:00Z",
    "created_from": "schedule",
    "is_test": false,
    "status": "pending",
    "report_type": "bank",
    "generation_date": "2019-08-01T06:00:00.000Z",
    "report_id": null,
    "last_modified": "2019-07-24T13:45:33.479-04:00",
    "retries": 0
}
```
**Response status code: 200 OK**


Detiene la generación automática del reporte. Actualiza el atributo scheduled en la configuración a false:

```curl
curl -X DELETE \
  -H 'accept: application/json' \
  -H 'content-type: application/json' \
  'https://api.mercadopago.com/v1/account/bank_report/schedule?access_token=ACCESS_TOKEN' \
  -d '{"user_id": USER-ID}'
```
Recibirás como respuesta:

```json
{
    "id": 2538023,
    "begin_date": "2019-07-24T06:00:00Z",
    "created_from": "schedule",
    "end_date": "2019-07-25T06:00:00Z",
    "generation_date": "2019-07-25T02:00:00.000-04:00",
    "is_test": false,
    "last_modified": "2019-07-24T13:50:10.719-04:00",
    "report_id": null,
    "report_type": "bank",
    "retries": 0,
    "status": "deleted",
    "user_id": USER-ID
}
```
**Response status code: 200 OK**


2. Descarga

Descarga el archivo con este comando: 

```curl
curl -X GET 'https://api.mercadopago.com/v1/account/bank_report/:file_name?access_token=ACCESS_TOKEN' 
```
Recibirás como respuesta:

```json
DATE,SOURCE_ID,EXTERNAL_REFERENCE,RECORD_TYPE,DESCRIPTION,NET_CREDIT_AMOUNT,NET_DEBIT_AMOUNT,GROSS_AMOUNT,MP_FEE_AMOUNT,FINANCING_FEE_AMOUNT,SHIPPING_FEE_AMOUNT,TAXES_AMOUNT,COUPON_AMOUNT,INSTALLMENTS,PAYMENT_METHOD
2018-04-17T15:07:53.000-04:00,,,initial_available_balance,,813439.19,0.00,813439.19,0.00,0.00,0.00,0.00,0.00,1,
2018-04-17T15:07:53.000-04:00,,,release,withdrawal,0.00,813363.45,-813360.45,-3.00,0.00,0.00,0.00,0.00,1,
2018-04-17T15:11:12.000-04:00,,,release,payment,225.96,0.00,269.00,-43.04,0.00,0.00,0.00,0.00,1,account_money
2018-04-17T15:18:16.000-04:00,,,release,payment,124.32,0.00,148.00,-23.68,0.00,0.00,0.00,0.00,1,visa
2018-04-17T15:38:40.000-04:00,,,release,payment,820.14,0.00,1099.00,-278.86,0.00,0.00,0.00,0.00,6,visa
2018-04-17T15:38:40.000-04:00,,,release,payment,850.00,0.00,850.00,0.00,0.00,0.00,0.00,0.00,1,account_money
```
**Response status code: 200 OK**


### También puedes ajustar la configuración del reporte vía API, usa los siguientes comandos para cada caso: 

### Consultar configuración 

[[[

```curl
curl -X GET \
    -H 'accept: application/json' \
    -H 'content-type: application/json' \
    'http://api.mercadopago.com/v1/account/bank_report/config?access_token=ACCESS_TOKEN' \
```

```Python
import requests
headers = {
    'accept': 'application/json',
    'content-type': 'application/json',
}
params = {'access_token', 'ACCESS_TOKEN'}

response = requests.get('http://api.mercadopago.com/v1/account/bank_report/config', headers=headers, params=params)
```

```node
var request = require('request');

var headers = {
    'accept': 'application/json',
    'content-type': 'application/json'
};

var options = {
    url: 'http://api.mercadopago.com/v1/account/bank_report/config?access_token=ACCESS_TOKEN',
    headers: headers
};
function callback(error, response, body) {
    if (!error && response.statusCode == 200) {
        console.log(body);
    }
}
request(options, callback);
```

]]]


### Crear configuración

[[[
    
```curl
curl -X POST \
    -H 'accept: application/json' \
    -H 'content-type: application/json' \
    'https://api.mercadopago.com/v1/account/bank_report/config?access_token=ACCESS_TOKEN' \
    -d '{
            "file_name_prefix": "bank-report-USER_ID",
            "include_withdrawal_at_end": false,
            "detailed": true,
            "execute_after_withdrawal": true,
            "extended": true,
            "frequency": {
                "hour": 0,
                "type": "monthly",
                "value": 1
            }
    }'
```

```Python
import requests

headers = {
    'accept': 'application/json',
    'content-type': 'application/json',
}

params = {'access_token', 'ACCESS_TOKEN'}

data = '{  
            "file_name_prefix": "bank-report-USER_ID",
            "include_withdrawal_at_end": false,
            "detailed": true,
            "execute_after_withdrawal": true,
            "extended": true,
            "frequency": {"hour": 0,"type": "monthly","value": 1}
        }'

response = requests.post('https://api.mercadopago.com/v1/account/bank_report/config', headers=headers, params=params, data=data)
```

```node
var request = require('request');

var headers = {
    'accept': 'application/json',
    'content-type': 'application/json'
};

var dataString = '{
            "file_name_prefix": "bank-report-USER_ID",
            "include_withdrawal_at_end": false,
            "detailed": true,
            "execute_after_withdrawal": true,
            "extended": true,
            "frequency": {
                "hour": 0,
                "type": "monthly",
                "value": 1
            }
    }';

var options = {
    url: 'https://api.mercadopago.com/v1/account/bank_report/config?access_token=ACCESS_TOKEN',
    method: 'POST',
    headers: headers,
    body: dataString
};

function callback(error, response, body) {
    if (!error && response.statusCode == 200) {
        console.log(body);
    }
}

request(options, callback);

```

]]]

### Actualizar configuración

[[[

```curl
curl -X PUT \
    -H 'accept: application/json' \
    -H 'content-type: application/json' \
    'https://api.mercadopago.com/v1/account/bank_report/config?access_token=ACCESS_TOKEN' \
    -d '{
        "file_name_prefix": "bank-report-USER_ID",
        "include_withdrawal_at_end": false,
        "detailed": true,
        "execute_after_withdrawal": true,
        "extended": true,
        "frequency": {
            "hour": 0,
            "type": "monthly",
            "value": 1
        }
    }'
```

```Python
import requests

headers = {
    'accept': 'application/json',
    'content-type': 'application/json',
}

params = (
    ('access_token', 'ACCESS_TOKEN'),
)

data = '{
            "file_name_prefix": "bank-report-USER_ID",
            "include_withdrawal_at_end": false,
            "detailed": true,
            "execute_after_withdrawal": true,
            "extended": true,
            "frequency": {"hour": 0,"type": "monthly","value": 1}
        }'

response = requests.put('https://api.mercadopago.com/v1/account/bank_report/config', headers=headers, params=params, data=data)
```

```node
var request = require('request');

var headers = {
    'accept': 'application/json',
    'content-type': 'application/json'
};

var dataString = '{
        "file_name_prefix": "bank-report-USER_ID",
        "include_withdrawal_at_end": false,
        "detailed": true,
        "execute_after_withdrawal": true,
        "extended": true,
        "frequency": {
            "hour": 0,
            "type": "monthly",
            "value": 1
        }
    }';

var options = {
    url: 'https://api.mercadopago.com/v1/account/bank_report/config?access_token=ACCESS_TOKEN',
    method: 'PUT',
    headers: headers,
    body: dataString
};

function callback(error, response, body) {
    if (!error && response.statusCode == 200) {
        console.log(body);
    }
}

request(options, callback);

```

]]]

### Iniciar generación programada

[[[

```curl
curl -X POST \
    -H 'accept: application/json' \
    -H 'content-type: application/json' \
    'https://api.mercadopago.com/v1/account/bank_report/schedule?access_token=ACCESS_TOKEN'
```

```Python
import requests

headers = {
    'accept': 'application/json',
    'content-type': 'application/json',
}

params = (
    ('access_token', 'ACCESS_TOKEN'),
)

response = requests.post('https://api.mercadopago.com/v1/account/bank_report/schedule', headers=headers, params=params)
```

```node
var request = require('request');

var headers = {
    'accept': 'application/json',
    'content-type': 'application/json'
};

var options = {
    url: 'https://api.mercadopago.com/v1/account/bank_report/schedule?access_token=ACCESS_TOKEN',
    method: 'POST',
    headers: headers
};

function callback(error, response, body) {
    if (!error && response.statusCode == 200) {
        console.log(body);
    }
}

request(options, callback);

```

]]]

### Cancelar generación programada

[[[

```curl
curl -X DELETE \
    -H 'accept: application/json' \
    -H 'content-type: application/json' \
    'https://api.mercadopago.com/v1/account/bank_report/schedule?access_token=ACCESS_TOKEN'
```

```Python
import requests

headers = {
    'accept': 'application/json',
    'content-type': 'application/json',
}
params = {'access_token', 'ACCESS_TOKEN'}

response = requests.delete('https://api.mercadopago.com/v1/account/bank_report/schedule', headers=headers, params=params)
```

```node
var request = require('request');

var headers = {
    'accept': 'application/json',
    'content-type': 'application/json'
};

var options = {
    url: 'https://api.mercadopago.com/v1/account/bank_report/schedule?access_token=ACCESS_TOKEN',
    method: 'DELETE',
    headers: headers
};

function callback(error, response, body) {
    if (!error && response.statusCode == 200) {
        console.log(body);
    }
}

request(options, callback);

```

]]]

# Ficha técnica

|              |                |
| ------------ |	--------    |
| `Programacion`| -  Diaria.<br/> -  Semanal.<br/>-  Mensual.|
| `Generación`  | -  Manual.<br/> -  Automática por retiro de dinero disponible, total o parcial <br/><br/> Las tres instancias de generación conviven. Es decir, aunque programes la generación de tus reportes automáticamente, cada vez que retires dinero se generará un reporte adicional. |
| `Detalla de tablas` | El detalle de las tablas comprende información generada en día 1 como mínimo. Excepto en los reportes generados por retiro de dinero. |
| `Formato del filename` | Cuando el reporte es programado o manual:<br/> “<prefijo-configurable>-<fecha-de-creación>.csv” <br/> Ejemplo:  mitienda-28-05-2019.csv <br/><br/> Cuando el reporte se genera por un retiro de dinero: “<prefijo-configurable>-<id-de-retiro>-<fecha-de-creación>.csv” Ejemplo: mitienda-ID23902138-28-05-2019.csv|
| `Formatos de descarga` | .csv, .xlsx <br/><br/>Tip: descarga el reporte en .csv para importar los datos y usarlos en otras aplicaciones. Descárgalo en .xlsx para leer la información en las tablas de la hoja de cálculo.|
| `Configuración disponible vía API` | -  Columnas a generar por reporte<br/> -  Prefijo del archivo para identificarlo fácilmente<br/> -  Carga por SFTP<br/> -  Separador de columnas (punto o punto y coma)<br/> -  Separador decimal (coma o punto)<br/> -  Notificación por e-mail<br/> -  Retiro al final del reporte (opcional) |
| `Orden de columnas` | Fijo |
| `Archivo` | Los reportes generados quedan guardados en tu cuenta de Mercado Pago |
| `Período máximo` | Reportes con datos de hasta 60 días |
| `Moneda` | Local (basada en el país donde esté registrada la cuenta de Mercado Pago) |
| `Zona horaria de las columnas con fechas:` | GMT-4 |
| `Selección de fechas vía API` | Formato del timezone: UTC / GMT-0 |
| `Selección de fechas vía web ` | <b>Debe basarse en el timezone de la cuenta del usuario.</b><br/>Por ejemplo, a la cuenta de usuario registrada en Brasil le corresponde el timezone de Sao Paulo.|


# Glosario

Lo sabemos, algunos términos son técnicos y puede que no estés familiarizado con todos ellos. ¡Usa este glosario para no perderte!

| `Nombre de la columna del reporte`  | `Qué significa` |
| ----------------------------------- |	--------------- |
| `DATE`| Fecha de liberación, bloqueo o desbloqueo, según corresponda.|
| `SOURCE_ID` | ID de operación en Mercado Pago (por ejemplo, el pago de una venta).|
| `EXTERNAL_REFERENCE` | ID que ayuda a identificar el origen de la operación. Por ejemplo, puede ser la venta a través del ID de la orden o el envío (si es una compra de carrito) o del ID propio provisto por el vendedor en caso de una integración externa.<br/><br/> Tené en cuenta que es posible que este campo esté vacío para algunos casos como el pago de facturas o un envío de dinero, entre otros.|
| `RECORD_TYPE` | initial_available_balance: Dinero disponible del período anterior.<br/><br/> block → Dinero bloqueado por un reclamo o contracargo.<br/><br/> unblock → Dinero liberado porque se resolvió un reclamo o contracargo.<br/><br/> release → Dinero de un cobro que fue liberado.<br/><br/> fullblock → Dinero bloqueado por restricción<br/><br/> subtotal → Suma de los montos de cada record type.<br/><br/> total → Monto neto total. |
| `DESCRIPTION` | <table style="border:none;" ><tr style="border:none;"><td style="border:none;"> Posibles valores que puede tomar el campo:<br/><ul><li> Para **block o unblock**: chargeback, dispute, shipping_return, credit_payment</li><li>Para **release**: payment, withdrawal, refund, tax_payment_ibcf, tax_payment_ibcf_cancel, tax_payment_ibex, tax_payment_iibb, tax_payment_iibb_cancel, shipping, shipping_cancel, tax_withdholding, tax_withdholding_cancel, mediation,mediation_cancel, chargeback, fee_release_in_advance, asset_management_gain, asset_management_loss</li><li>Para **fullblock**: restriction.</li><li>Para **subtotal**: block, unblock o release.</li></ul></td></tr><tr style="border:none;"><td style="border:none;">Definiciones a tener en cuenta:<br/><br/> **chargeback**: aparece cuando se inicia o resuelve un contracargo asociado al pago al que hace referencia.<br/><br/> **dispute**: aparece cuando se inicia o resuelve una mediación o reclamo sobre el pago al que hace referencia. Puede ocurrir antes o después de que el pago se haya liberado como dinero disponible e incluso retirado de la cuenta.<br/><br/>**shipping_return**: aparece cuando se bloquea o desbloquea un pago realizado por devolución express.<br/><br/>**payment**: pago que se libera en alguno de los canales en los que opera el cliente.<br/><br/>**withdrawal**: retiro que se ejecuta sobre el dinero disponible.<br/><br/>**refund**: devolución asociada al pago al que hace referencia.<br/><br/>**tax_payment_ibcf**: percepción de ingresos brutos en Capital Federal, se calcula una vez por mes de acuerdo a las operaciones transaccionadas. Para conciliar por operación, ver el detalle en los [Informes de Facturas en MyML](https://vendedores.mercadolibre.com.ar/blog/notas/todo-lo-que-tenes-que-saber-sobre-tu-facturacion/).<br/><br/>**tax_payment_ibcf_cancel**: cancelación del impuesto de percepción de ingresos brutos en Capital Federal.<br/><br/>**tax_payment_ibex**: percepción de ingresos brutos por sujeto excedido de régimen simplificado, se calcula una vez por mes de acuerdo a las operaciones transaccionadas. Para conciliar por operación, ver el detalle en los [Informes de Facturas en MyML](https://vendedores.mercadolibre.com.ar/blog/notas/todo-lo-que-tenes-que-saber-sobre-tu-facturacion/). <br/><br/> **tax_payment_iibb**: percepción de ingresos brutos en provincia de Buenos Aires, se calcula una vez por mes de acuerdo a las operaciones transaccionadas. Para conciliar por operación, ver el detalle en los [Informes de Facturas en MyML](https://vendedores.mercadolibre.com.ar/blog/notas/todo-lo-que-tenes-que-saber-sobre-tu-facturacion/).<br/><br/> **tax_payment_iibb_cancel**: cancelación del impuesto de percepción de ingresos brutos.<br/><br/> **tax_withdholding**: el cobro de retenciones que no se pudieron ejecutar transaccionales al pago asociado. En Argentina son únicamente retenciones de Ingresos Brutos (las percepciones se debitan como otra operación). En Uruguay son retenciones de IVA. En Colombia son retenciones de IVA, ICA y Fuente según aplique el caso.<br/><br/> **tax_withdholding_cancel**: la cancelación de la retención tax_withdholding.<br/><br/> **shipping**: comisión de shipping para las compras de carrito que no se incluye en cada uno de los pagos del carrito.<br/><br/> **shipping_cancel**: cancelación de la comisión de shipping para las compras de carrito que no se incluye en cada uno de los pagos del carrito.<br/><br/> **mediation**: resolución de una mediación a favor del comprador que termina restando del dinero disponible del vendedor.<br/><br/> **mediation_cancel**: cancelación de la mediación resuelta a favor del comprador.<br/><br/> **chargeback**: contracargo ya sea a favor o en contra de una operación.<br/><br/>**fee-release_in_advance**: comisión por adelanto.<br/><br/> **asset_management_gain**: rendimiento positivo generado por la variación del valor de cuotapartes suscritas en el fondo común de inversión.<br/><br/> **asset_management_loss**: rendimiento negativo generado por la variación del valor de cuotapartes suscritas en el fondo común de inversión.<br/><br/> **restriction**: ocurre cuando se te aplica una restricción por comportamiento fraudulento.<br/><br/> **credit_payment**: aparece cuando se cobra la cuota de un préstamo otorgado.</td></tr></table>|
| `NET_DEBIT_AMOUNT` | Acreditado al monto disponible. |
| `NET_CREDIT_AMOUNT` | Debitado al monto disponible. |
| `GROSS_AMOUNT` | Monto de la operación bruto. |
| `MP_FEE_AMOUNT` | Pago Comisión de Mercado Pago y/o Mercado Libre. Incluye IVA.|
| `FINANCING_FEE_AMOUNT` | Costo por ofrecer cuotas sin interés. |
| `SHIPPING_FEE_AMOUNT` | Costo de envío. |
| `TAXES_AMOUNT` | Impuestos cobrados por retenciones de Ingresos Brutos. |
| `COUPON_AMOUNT` | Monto del cupón de descuento. **Solo se descuenta del monto bruto (GROSS_AMOUNT) si está provisto por el vendedor**.|
| `INSTALLMENTS` | Cantidad de cuotas en las que se realizó la operación. |
| `PAYMENT METHOD` | Medio de pago. Puede ser: <br/>visamaster<br/> amex<br/> naranja<br/> nativa<br/> tarshop<br/> cencosud<br/> cabal<br/> argencard<br/> diners<br/> pagofacil<br/> rapipago<br/> redlink<br/> bapropago<br/> account_money (Pago con dinero en la cuenta de Mercado Pago).|
| `TAX_DETAIL` | Descripción del impuesto retenido por operación en el TAXES_AMOUNT. Puede tomar los siguientes valores según la jurisdicción: <br/>cordoba<br/>mendoza<br/>la_pampa<br/>santa_fe<br/>tucuman<br/>entre_rios<br/>catamarca<br/>neuquen<br/>santiago_del_estero<br/>rio_negro<br/>jujuy<br/> |
| `TAX_AMOUNT_TELCO` | Es el valor del impuesto a las empresas de telecomunicaciones que se descuenta del valor bruto. |
| `TRANSACTION_APPROVAL_DATE` | Fecha de aprobación de la operación. |
| `POS_ID` | ID de caja si el pago se realiza a través de un comercio físico. |
| `POS_NAME` | Nombre de caja para el pago realizado a través de un comercio físico. |
| `EXTERNAL_POS_ID` | ID de caja definido por el usuario para el pago realizado a través de un comercio físico. |
| `STORE_ID` | ID de sucursal si el pago se realiza a través de un comercio físico. |
| `STORE_NAME` | Nombre de sucursal para el pago realizado a través de un comercio físico. |
| `EXTERNAL_STORE_ID` | ID de sucursal definido por el usuario para el pago realizado a través de un comercio físico. |
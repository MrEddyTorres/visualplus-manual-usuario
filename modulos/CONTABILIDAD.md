
___________________________

# CONTABILIDAD

<img src="assets/img/modulos logo/contabilidad.png" alt="JuveR" width="135px"> 


_____________________________
| <font size="3"> Funciones principales:  </font>|
| :---------------------- |
| - **CONFIGURACIONES CONTABLES** |
| [Migrar plan de cuentas a un sistema nuevo](modulos/contabilidad?id=migrar-plan-de-cuentas-a-un-sistema-nuevo)|
| [Primera configuración contable](modulos/contabilidad?id=primera-configuraciÓn-contable) |
| [Configuración de cuentas](modulos/contabilidad?id=configuraciÓn-de-cuentas) |
| [Configurar grupos de items](contabilidad?id=configurar-grupos-de-items) |
| [Configurar tipos de cuenta](modulos/contabilidad?id=configurar-tipos-de-cuenta) |
| - **PROVEEDORES** |
| [Cancelar factura de Proveedor](modulos/contabilidad?id=cancelar-totalmente-una-factura-de-un-proveedor-comprobantes-de-pago) |
| [Crear y Devolver Anticipos a Proveedores](modulos/contabilidad?id=anticipos-a-proveedores-comprobantes-de-ingreso-y-egreso) |

_________________________

# CONFIGURACIONES CONTABLES

## MIGRAR PLAN DE CUENTAS A UN SISTEMA NUEVO

> El plan de cuentas debe ser preparado y aprobado por el contador o contadora de la empresa acorde a las necesidades de la misma.

- Si va a migrar el plan de cuentas debe tener listo un EXCEL con la **columna A y B vacías** (actualmente ya no se llena esa información). En la **columna C** debe estar el código contable y en la **columna D** el nombre de la cuenta.

- Verificar que esten correctos los nombres de las cuentas y que no tengan espacios en blanco entre ellas.

Ingresamos a opción **"PLAN DE CUENTAS"** y damos clic en el botón **"IMPORTAR"** de la parte inferior.

<img src="assets/img/contabilidad/importar.png" alt="JuveR" width=80px border="1">

- El sistema nos mostrará un mensaje con las indicaciones previamente mencionadas. Damos clic en **"SÍ"**.

- Buscamos y seleccionamos el archivo EXCEL en donde lo guardamos y damos clic en **"ACEPTAR"**

- Esperamos a que se migre el plan de cuentas. Al finalizar nos aparecerá el siguiente mensaje:

<img src="assets/img/contabilidad/asignar.png" alt="JuveR" width=195px border="1">

- Damos clic en **"Sí"** y listo.

## PRIMERA CONFIGURACIÓN CONTABLE

Una vez integrado el plan de cuentas la primera configuración contable se la realiza dentro del módulo de **AUDITORÍA**. 

_Es necesario tener migrado el plan de cuentas._

Enlazaremos las siguientes cuentas: 

- CUENTAS POR COBRAR DE CLIENTES
- ANTICIPO DE CLIENTES
- CUENTAS POR PAGAR A PROVEEDORES
- ANTICIPO A PROVEEDORES

__Esto lo haremos para que el sistema por defecto coloque estas cuentas al crear un cliente o proveedor nuevos.__ 

Ingresamos al módulo **AUDITORÍA**, clic en **AUDITORÍA, CONFIGURACIÓN** y clic en la opción **"CONFIGURACIÓN DEL SISTEMA"**

- Dentro, seleccionamos la pestaña de la parte superior llamada **"CONTABILIDAD"**

- Encontraremos los siguientes campos:

<img src="assets/img/contabilidad/cuentas.png" alt="JuveR" width=180px border="1">

- Para desbloquear, hacemos clic sobre la palabra de la parte superior de cada campo.

- En el recuadro de la izquierda podemos digitar el nombre de la cuenta contable, y la seleccionamos desde el listado de la derecha.

  - Con clic derecho sobre el listado podemos intercalar entre una búsqueda por **"nombre de la cuenta contable"** o por el **"nro del código contable"**

- Una vez finalizada la configuración damos clic en el botón de "GUARDAR" de la parte inferior.

## CONFIGURACIÓN DE CUENTAS
> Conforme se integren en el LIBRO DIARIO las compras, ventas, retenciones, recaudaciones, etc, se rellenará este listado automáticamente. 

- En el módulo CONTABILIDAD hacemos clic en la opción **"CONFIGURACIÓN DE CUENTAS"**

- Seleccionamos la cuenta que queremos que se integre, en este caso seleccionaremos **"EFECTIVO"** 

- En la parte superior del listado encontraremos los íconos de **“CREAR, EDITAR, ELIMINAR Y REGRESAR”**
 
<img src="assets/img/MED.PNG" alt="JuverR" width="110px" >

Clic en **"EDITAR"** para editar el registro:

Se abrirá una nueva ventana, 

<img src="assets/img/contabilidad/config.png" alt="JuveR" width=290px border="1">

En el recuadro de la izquierda de cada campo, podemos digitar el nombre de la cuenta contable, y nos aparecerá el listado en la derecha.

  - Con clic derecho sobre el listado podemos intercalar entre una búsqueda por **"nombre de la cuenta contable"** o por el **"nro del código contable"**

A modo de ejemplo colocaremos la siguiente información:

- **CÓDIGO DE CUENTA:** "Caja General | 1.01.01.01.01" 

- **CÓDIGO DEL DEBE:** "Caja General  | 1.01.01.01.01"

- **CÓDIGO DEL HABER:** De ser necesario colocamos un código distinto, pero en este caso lo podemos dejar vacío o colocarle nuevamente "Caja General".


***NOTA: Al comienzo muchos asientos del LIBRO DIARIO se irán a PENDIENTES. Haremos este proceso para enlazar manualmente las cuentas contables y así poco a poco iremos configurando todas las cuentas***

## CONFIGURAR GRUPOS DE ITEMS
> Aquí configuraremos las cuenta contables a la que se irán los GRUPOS que contienen nuestro items de inventario, dependiendo del tipo de proceso.

Ingresamos a opción **"PROCESOS CONTABLES"** y damos clic en el botón **"GRUPO"**

Se desplegará un listado con todos los GRUPOS que hayamos creado en el módulo **ITEM**. Cada columna corresponderá a los siguientes nombres:

<img src="assets/img/contabilidad/grupo.png" alt="JuveR" width=250px >

Se puede editar manualmente las cuentas contables de cada grupo seleccionándolo y dando clic en la opción **"EDITAR"** 

<img src="assets/img/MED.PNG" alt="JuverR" width="110px" >

- Para asignar la misma cuenta a todos los grupos utilizamos la pestaña de la parte superior.

<img src="assets/img/contabilidad/grupo2.png" alt="JuveR" width=250px border="1" >

- Primero seleccionamos el nombre en la primera pestaña. ***Ej: "Cod. de Inventario Gravado"***

- Segundo en el listado inferior seleccionamos el **código contable**  ***Ej: Inv. De Mercaderia 12% | 1.01.03.01.01*** (digitamos el nombre de la cuenta o el código contable luego de desplegar el listado)

  - Recuerda que con **clic derecho** podemos intercalar entre buscar por código o por nombre de la cuenta.

- Una vez estemos seguros, damos clic en el **"VISTO"**, de este modo se enlazará la cuenta contable con todos los GRUPOS. Repetimos el mismo procedimiento para el resto de cuentas.

NOTAS ADICIONALES: 
- En las cuentas que dicen **gravado 14%** las dejamos vacías o les colocamos las cuentas que correspondan al IVA vigente, en este caso el 12%.
- Si no nos aparece el código en nuestro plan de cuentas, procedemos a *buscarlo o crearlo* mediante el botón de los **tres puntitos**  <img src="assets/img/contabilidad/puntos.png" alt="JuveR" width=20px border="1"> una vez ubiquemos la cuenta la seleccionamos y damos clic en el botón **"REGRESAR"** ubicado al final de las opciones de **“CREAR, EDITAR, ELIMINAR Y REGRESAR”** 

<img src="assets/img/MED.PNG" alt="JuverR" width="110px" >

Esto cerrará la ventana y seleccionará el código automáticamente.
 

## CONFIGURAR TIPOS DE CUENTA 
> Aquí enlazaremos las cuentas referentes a las **modalidades de pagos** con sus respectivas cuentas contables.

Ingresamos a la opción **"TIPOS DE CUENTA"**

Seleccionamos entre las opciones la cuenta que deseamos configurar, como ejemplo configuraremos la cuenta **CHEQUE**

- La seleccionamos y editamos manualmente con la opción de **EDITAR** de la parte superior.

<img src="assets/img/contabilidad/med.png" width="100" border="1">

Se desplegará la siguiente ventana:

<img src="assets/img/contabilidad/cheque.png" width="400" border="1">

En el recuadro de la izquierda de cada campo, podemos digitar el nombre de la cuenta contable, y nos aparecerá el listado a la derecha.

  - Con clic derecho sobre el listado podemos intercalar entre una búsqueda por **"nombre de la cuenta contable"** o por el **"nro del código contable"**

- En **DEBE** colocamos la cuenta de "Cheques por Cobrar | 1.01.02.01.03"

- En **"HABER"** colocaremos la misma cuenta  "Cheques por Cobrar | 1.01.02.01.03"

***Notas Adicionales:*** 

 - ***Transferencias, depósitos y cheques trabajan con cuentas transitorias.*** 

  - ***Esta configuración puede variar de acuerdo a la forma de trabajar del contador/a o la empresa.***

_______________________________________

# PROVEEDORES

## CANCELAR TOTALMENTE UNA FACTURA DE UN PROVEEDOR (COMPROBANTES DE PAGO)
_______________________________________

- **CANCELAR FACTURAS DE COMPRA TUTORIAL:**

<button style="border:none"> <a href="https://www.youtube.com/embed/cbUeFXXBuSM" target="_blank"> <img src="assets/img/tutorial demo.png" alt="TEXTO" width="300" height="150" border="1" /></a> </button>

___________________________

## ANTICIPOS A PROVEEDORES (COMPROBANTES DE INGRESO Y EGRESO)
____________________________________

- **CREAR ANTICIPOS A PROVEEDORES TUTORIAL:**

<button style="border:none"> <a href="https://www.youtube.com/embed/Qmg-P5YW4ls" target="_blank"> <img src="assets/img/tutorial demo.png" alt="TEXTO" width="300" height="150" border="1" /></a> </button>

_____________________________________________

- **DEVOLUCIÓN DE ANTICIPOS A PROVEEDORES TUTORIAL:**

<button style="border:none"> <a href="https://www.youtube.com/embed/fF_QOGL7Aks" target="_blank"> <img src="assets/img/tutorial demo.png" alt="TEXTO" width="300" height="150" border="1" /></a> </button>
___________________________


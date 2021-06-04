# Página Combo

## ● **Cubos Uniswap V2**

### **No puedo encontrar el token / grupo que quiero**

Admitimos la función de importación de token en cubos Uniswap V2. Simplemente pegue la dirección del token / indica la dirección del token en la barra de búsqueda.

![](../.gitbook/assets/image%20%288%29.png)

### **¿Puedo intercambiar WETH directamente?**

Desafortunadamente, el uso de WETH como entrada o salida en los cubos Uniswap V2 no está disponible en Furucombo. una alternativa, puede usar el cubo WETH que está debajo para envolver o desenvolver.

### **¿Cuál es la configuración de deslizamiento en Uniswap?**

El deslizamiento predeterminado se establece en 3%.

## ● **Aave cubos**

### **Cómo usar flashloan**

Tenemos un tutorial completo que te guíara para crear un combo flashloan. [Leer aquí](https://medium.com/furucombo/create-flashloan-combo-on-furucombo-c7c3b23267f0)

### **¿Por qué dice "algo anda mal dentro de los cubos de flashloan"?**

Cuando presionas el botón de enviar, Furucombo ejecuta una estimación de tu combo en la secuencia de configuración de tus cubos. Cuando vea el mensaje de error "algo está mal dentro del flashloan", significa que la transacción fallará al ejecutar los cubos de flashloan.

El error más común es que el precio ha cambiado en los cubos de flashloan. En este caso pulsa el botón de actualizar precio.

También puede intentar eliminar los cubos flashloan y presionar enviar nuevamente para ver qué cubo tiene un error.

### **¿Por qué tengo que pagar una tarifa del 0,09%?**

La tarifa del 0.09% se paga directamente a Aave por usar flashloan. Furucombo no cobra ninguna tarifa de ninguna forma.

### **¿Por qué no puedo poner cubos de Aave dentro de flashloan?**

Esta es una configuración de limitación de Aave. Cuando usa flashloan, está tomando la liquidez de Aave. No tiene sentido utilizar los fondos prestados con el fondo común prestado, ¿verdad?

## ● Cubos Maker

### **¿Qué es una bóveda?**

Las bóvedas son un componente central del protocolo maker, que facilita la generación de DAI contra garantías bloqueadas. Todos los DAI en circulación son creados por las bóvedas. El uso de las bóvedas altera colectivamente el suministro total de DAI. Los usuarios crean DAI generándolo contra su garantía y, a su vez, destruyen DAI cuando pagan el saldo de DAI generado.

Las bóvedas no son de uso gratuito y conllevan riesgos inherentes. La generación de DAI requiere el pago de tarifas de estabilidad \(SF\). El SF es una tasa variable y está sujeta a cambios en función de las decisiones de los titulares de Token MKR mediante votación.

Para reclamar la garantía, los usuarios deben reembolsar el DAI generado previamente y el SF acumulado.

Las bóvedas deben tener una garantía excesiva y tener un índice de liquidación que los propietarios de las bóvedas deben mantener para evitar la liquidación de sus bóvedas. Cuando se liquida una bóveda, se aplica una multa por liquidación y se vende la garantía para pagar el saldo pendiente de DAI de la bóveda. Además, se impone un límite máximo de deuda globalmente en el Protocolo Maker, así como individualmente en cada tipo de bóveda.

### **¿Dónde consigo mi número de bóveda?**

Si ya tiene una bóveda, primero conecte su billetera y luego elija cualquier cubo Maker excepto "New Vault". Verá el número de su bóveda cuando haga clic en el espacio en blanco de Vault \#.

Si usa New Vault para crear una bóveda. Obtendrá el número de la bóveda después de que el combo se envíe correctamente. Luego regresa y elige cualquier cubo Maker excepto "New Vault" para ver su número de bóveda.

![](../.gitbook/assets/image%20%2832%29.png)

Alternativamente, puede visitar [oasis.app](https://oasis.app/) para ver su número de bóveda.

### **¿Qué es Oasis Trade?**

Maker lanza Oasis Trade. Es un grupo de liquidez en la cadena de bloques Ethereum. Los contratos inteligentes de Simple Market y Matching Market proporcionan el intercambio atómico de tokens ERC20 sin contrariesgos de terceros.

### **¿Cómo beneficiarse de la transferencia de CDP a Compound?**

Este es un combo para usuarios que ya tienen una bóveda en Maker para ayudarlos a mover fácilmente los tokens a Compound. No es necesariamente una combinación rentable. Es más como un combo de gestión de activos para Maker  


## ● Cubos Curve

### **¿Puedo elegir la piscina para intercambiar?**

No puedes elegir la piscina en Curve. Cuando usa el cubo Swap Token de Curve, Curve elige automáticamente el mejor grupo para usted.

### **¿Cuál es el deslizamiento configurado en Curve?**

El deslizamiento predeterminado se establece en 3%.

### **Mi combo Claim CRV no funciona**

Cuando usa Claim CRV, el token CRV reclamado va directamente a su billetera. Por lo tanto, si desea utilizar los tokens CRV en los siguientes cubos, debe insertar un cubo "Add Funds" como el siguiente cubo con CRV.

## ● C**ubo 1inch**

### No puedo encontrar el token que quiero, pero puedo encontrarlo en 1inch

Los token en Furucombo son seleccionadas por el equipo de Furucombo. Si no puede encontrar el token que desea, avísele al equipo en el canal de Discord \#feedback.

### **¿Cuál es el deslizamiento configurado en un cubo de 1inch?**

El deslizamiento predeterminado se establece en 3%.

### **Uso 1inch en mi combo pero sigue diciendo que fallará**

Hay un problema inconsistente conocido por usar 1inch. Aquí hay una solución alternativa para su referencia:

* Vaya a 1inch.exchange para ver qué servicio de intercambio utilizan en la ruta para su intercambio. Digamos que ve que pasa por Uniswap V2
* Vuelve a Furucombo y reemplaza el cubo de 1inch con Uniswap V2

## ● **Cubos Compound**

### **¿Cómo puedo pedir prestado de Compound?**

Desafortunadamente, la función de préstamo de Compound no es compatible con Furucombo. Pero es un trabajo en progreso. 

### **¿Cómo puedo auto liquidarme en Compound?**

Tenemos [un combo prediseñado](https://furucombo.app/combo/bt49ulfm1503gp5r5keg?refreshPrice=1) para usted, que también puede encontrar en nuestra [página Explorar](https://furucombo.app/explore/combo_compound_00004) para su futura revisión.

![use Compund tag to fast locate the combo](../.gitbook/assets/compound-self-liq.png)

## ● **Cubo de Kyberswap**

### No puedo encontrar el token que quiero, pero puedo encontrarlo en Kyberswap

Los token en Furucombo son seleccionadas por el equipo de Furucombo. Si no puede encontrar el token que desea, avísele al equipo en el canal de Discord \#feedback.

### **¿Cuál es la configuración de deslizamiento en Kyberswap?**

El deslizamiento predeterminado se establece en 3%.

## ● **Cubos Balancer**

### No puedo encontrar el token o grupo que quiero

Los token en Furucombo son seleccionadas por el equipo de Furucombo. Si no puede encontrar el token que desea, avísele al equipo en el canal de Discord \#feedback.

### **¿Cómo examinó un grupo en Balancer?**

1️⃣ Verifique los primeros seis dígitos de la dirección de la piscina.

![](../.gitbook/assets/image%20%2819%29.png)

2️⃣ Verifique el activo en el grupo

![](../.gitbook/assets/image%20%2827%29.png)

### **¿Qué son las opciones Single-Asset y All-Assets?**

Al agregar o eliminar liquidez desde Balancer, verá las opciones All-Assets y Single-Asset en la parte superior. Tomemos como ejemplo el grupo WETH 50% / WBTC 50%:

![](../.gitbook/assets/image.png)

* Agregar liquidez **All Assets**: usted proporciona todos los activos del grupo de manera proporcional a los porcentajes del grupo. 
  * 👉 Envía 1 WETH y 0.0285WBTC a Balancer y recibe el token 0.02283 BPT token.
* Agregar liquidez **Single Asset**: solo proporciona un tipo de token al grupo. Balancer intercambiará proporcionalmente el token que aportó para agregar liquidez al grupo. 
  * 👉 Envía 1 WETH a Balancer y recibe un token de 0.01105BPT.

## ● **Cubos de utilidad**

### **¿Qué es Enviar Token?**

Como dice, el cubo Send Token le permite enviar token a una dirección designada. Algunos casos de uso pueden ser

* Enviar token a varias direcciones
* Envía varios tokens a una dirección
* Mueva todas sus token a otra billetera

### **¿Qué es WETH?**

Cuando "envuelve" ETH, en realidad no está envolviendo sino negociando a través de un contrato inteligente por un token igual llamado WETH. Si desea recuperar su ETH simplemente, debe "desenvolverlo" o también puede cambiarlo por ETH.

Para obtener más información sobre WETH, visite [weth.io](http://weth.io/)

### **¿Qué es Agregar fondos?**

El cubo Add Funds se usa cuando necesitas enviar ETH o tokens a Furucombo **durante la ejecución** de un combo.

For example, when you wanna claim your CRV and sell them to DAI, you must use "Add Funds" to complete the combo. This is because when you claim CRV, the claimed CRV tokens go straight to your wallet but not Furucombo. In order to continue sending those CRV to Uniswap, you need to send the CRV to Furucombo first. See the correct setup below.

![](../.gitbook/assets/image%20%2811%29.png)

### **¿Qué son los fondos de devolución?**

El cubo de devolución de fondos se usa cuando desea enviar ETH o tokens a su billetera **durante la ejecución** del combo. Aunque Furucombo envía todos los fondos a los usuarios al completar la ejecución del combo, en algunos casos, se deben agregar fondos de devolución para ejecutar con éxito el combo.

Por ejemplo \(vea la imagen a continuación\), desea intercambiar sus garantías en Compound, diga cDAI a cETH. Cuando toma prestado ETH de flashloan y proporciona el ETH a Compound, el cETH que ve en el segundo cubo, en realidad se envía al proxy de Furucombo. Su cDAI está bloqueado hasta que tenga suficiente cETH para respaldar su deuda, por lo que aquí necesitamos el cubo "Devolver fondos" que transfiere cETH del proxy de Furucombo a su billetera. ¡Y en el siguiente cubo, mueves tu cDAI al proxy de Furucombo con el cubo "Agregar fondos"!

![Compound Collateral Swap](../.gitbook/assets/image%20%2821%29.png)

### **¿Qué es Gas Saver?**

El cubo Gas Saver se usa cuando tiene algunos token CHI o GST2 en su billetera. Cuando los quema \(especialmente a un alto precio de la gasolina\), obtiene un reembolso para hacer que la gasolina cueste mucho más barato de ejecutar que la misma transacción que no usa GasToken. Para obtener más información sobre el token de gas, consulte los enlaces a continuación:

* [GasToken.io](https://gastoken.io/#:~:text=GasToken%20is%20a%20new%2C%20cutting,gas%20when%20it%20is%20expensive.)
* [CHI token por 1inch ](https://medium.com/@1inch.exchange/everything-you-wanted-to-know-about-chi-gastoken-a1ba0ea55bf3)

## 🧠 **Estrategias de arbitraje**

### **¿Qué es el arbitraje?**

En muchos sentidos, el arbitraje criptográfico es como el arbitraje fiduciario o deportivo. La idea principal aquí es simple: intenta beneficiarse de las diferencias de precio para el mismo activo en diferentes mercados o bolsas. 

Investopedia describe el arbitraje como “la compra y venta simultánea de un activo para beneficiarse de un desequilibrio en el precio. Es un comercio que se beneficia al explotar las diferencias de precio de instrumentos financieros idénticos o similares en diferentes mercados o en diferentes formas ”.

En otras palabras, **¡compre barato y venda caro!**

Lecturas relacionadas: 

* [Arbitraje en DeFi por The Block](https://www.theblockcrypto.com/post/45750/exploring-defi-trading-strategies-arbitrage-in-defi)

### **¿Cómo se ve un combo rentable?**

![](../.gitbook/assets/profitable.png)

* **No** hay fondos iniciales

{% hint style="danger" %}
Si ve que aparece la sección de fondos iniciales, eso significa que no es una combinación rentable. El peor de los casos es que pierde los fondos iniciales y no obtiene nada a cambio.
{% endhint %}

* Usted recibirá
  * Los activos que se muestran en esta sección son ganancias del combo.

### **¿Cómo hacer un combo rentable?**

* En primer lugar, debe encontrar una oportunidad de arbitraje. 
* Teniendo en cuenta los costos del gas, los combos de arbitraje cuestan más que los combos promedio debido a la complejidad de las acciones. Este es un factor de costo principal que influye en la rentabilidad del comercio.
* Recuerde que hay muchas operaciones de bots que se ejecutan al frente en todo momento. Por lo tanto, existe la posibilidad de que su combo sea liderado por bots.
* Los combos de arbitraje tienen una mayor probabilidad de fallar ya que la configuración del combo generalmente tiene una alta dependencia de las salidas de cada cubos. Dicho esto, una vez que la oportunidad se desvanece, su combinación falla y pierde la tarifa de gasolina que acaba de pagar.

## 👛 **Billetera**

### No veo la billetera de Coinbase en el menú

Si no ve Coinbase Wallet, haga clic en Wallet Connect y escanee el código QR con su aplicación Coinbase Wallet.

### **¿Puedo usar MetaMask en Brave?**

Siga este [tutorial](https://www.loom.com/share/bee83b1e0d724779aa4d22c9d8a242c0) para permitir que Furucombo conecte su MetaMask en Brave.

La razón detrás de esto es que Brave acaba de actualizar su configuración sobre cómo conectarse al "proveedor Web3 para usar Dapps".  
​  
Seguiremos investigando este problema y nos aseguraremos de que esté actualizado.

### **No puedo conectarme a la plataforma**

* Asegúrese de seleccionar la red correcta \(Ethereum Mainnet\), normalmente en el proveedor de billetera puede cambiar la red en las opciones de configuración.
* En Ledger de forma nativa o sobre Metamask:
  * Asegúrese de desbloquear y seleccionar la aplicación Ethereum.
  * Asegúrese de que los datos del contrato estén permitidos en la configuración de la aplicación Ethereum.
* Coinbase
  * Utilice el código QR escaneado para conectarse.
* Conectar billetera
  * Utilice el código QR escaneado para conectarse.
* Fortmatic
  * Asegúrese de cambiar a Ethereum Mainnet.

## ⛽️ Gas

### **¿Por qué es tan alta la tarifa del gas?**

Depende de cuántos cubos uses y de qué tan ocupada esté la red Ethereum. Puede hacer clic en el botón "Enviar" para calcular el costo del gas. Su billetera \(por ejemplo, MetaMask\) aparecerá y le dirá cuánto costará la tarifa.

### **¿Puedo saber cuánto gas costará antes de enviarlo?**

Desafortunadamente, no puede obtener la estimación del gas antes de presionar el botón de enviar.

### **¿Cómo puedo configurar el precio del gas?**

Puede ajustar el precio y el límite del gas cuando usa la billetera MetaMask. Al presionar el botón de enviar, verá una ventana emergente de MetaMask. Haga clic en "EDITAR" y verá opciones de velocidad.

Para personalizar la tarifa de transacción, seleccione Opciones avanzadas:

Puede ingresar manualmente el precio del gas \(GWEI\) y el límite del gas. También puede hacer clic en el gráfico de predicciones de gas en vivo.

![](../.gitbook/assets/image%20%289%29.png)

### **¿Debo reducir el límite de gas?**

No, no deberías. El límite de gas es el presupuesto de la transacción. El gas no utilizado se reembolsará a su billetera. Sin embargo, si el gas cuesta más que su límite de gas, todo se revertirá, pero NO se devolverá el gas.

## 📖 **Otras preguntas frecuentes**

### **¿Cómo ajusto los fondos iniciales?**

La cantidad de fondos iniciales se actualiza automáticamente.

Solo necesita ajustar los números en los cubos, luego la cantidad requerida de fondo inicial se actualizará en consecuencia.

### **¿Por qué necesito firmar dos veces?**

Normalmente, debe enviar 2 transacciones para procesar una transferencia de token que no sea ETH. Por ejemplo, si desea cambiar DAI a COMP, debe firmar dos veces en su billetera:

1. Aprobar: para otorgarle a Furucombo el permiso para mover sus tokens.
2. Enviar: para ejecutar su transacción. En este ejemplo, para cambiar su DAI a COMP.

### **¿Cuántas veces tengo que aprobar?**

Depende de los token que tengas y de los cubos que vayas a utilizar.

La cantidad de veces que debe aprobar se basa en la cantidad de condiciones que se indican a continuación y en la cantidad de tokens ERC-20 aprobados que le otorga a Furucombo para mover.

* Primera vez para usar tokens ERC20 como fondos iniciales
* Primera vez que utilizo cualquiera de los siguientes cubos:
  * Maker retirar
  * Maker Generar
  * Staking en Curve
  * Reclamar Curve

Cantidad del token ERC-20 aprobado:

* Por consideraciones de seguridad, la cantidad de token ERC-20 predeterminada de aprobación será precisamente la cantidad gastada en Furucombo.
* También puede personalizar una mayor cantidad de tokens de aprobación. Al hacerlo, antes de que se agote el límite de aprobación del token, no es necesario enviar otras transacciones de aprobación del token.
  * MetaMask: al aprobar Furucombo para gastar sus tokens, puede hacer clic en "Editar permiso" para personalizar un límite de gasto más alto.
  *   Tenga en cuenta que la transacción fallará si la ajusta a un límite de aprobación menor.

![](https://gblobscdn.gitbook.com/assets%2F-MJ0u2YbMrrM5MnNGC9b%2F-MUvjHgTFFIX2nXE4SMd%2F-MUvksbxxc0tFcojpeKj%2F%E6%88%AA%E5%9C%96%202021-03-04%20%E4%B8%8B%E5%8D%881.42.39.png?alt=media&token=14907771-3e8c-45bf-a669-64b195359fc4)

Ejemplos:

* Por primera vez Alice usará un Combo: Intercambiar ETH a DAI
  * No es necesario aprobar \(ETH no es un token ERC-20\)
* Por primera vez BOB usará un Combo: Intercambiar $500 DAI a ETH
  * Necesita aprobar una vez para DAI
  * Y ajusta el límite de gasto de DAI en Furucombo a $1000.
* Bob utiliza por segunda vez un combo: intercambia $200 DAI por COMBO
  * No es necesario aprobar \(porque todavía tiene el límite de aprobación $500 DAI\).
* Bob utiliza por segunda vez un combo: Deposita WBTC en Maker y genere DAI
  * Necesita aprobar dos veces \(una vez para WBTC, una vez para Maker Generar\)

### **¿Por qué sigue diciendo que mi transacción fallará?**

En la mayoría de los casos, se debe a que el precio ha cambiado y necesita actualizar los números.

Si usa cubos de préstamos flash y ve el mensaje de error, significa que necesita actualizar los números de los cubos dentro del par de préstamos flash.

### **¿Por qué falló mi transacción?**

IEn la mayoría de los casos, se debe a que el precio cambió, lo que hace que su combinación se aleje demasiado de su conjunto original. Puede evitar este tipo de fallas dejando más espacio para el deslizamiento:

Por ejemplo, desea intercambiar 1 ETH por DAI y luego agregar DAI al grupo Curve como Proveedor de liquidez \(LP\):

Buen combo:

* Cubo 1: intercambia 1 ETH por 400 DAI
* Cubo 2: agregue 380 DAI al grupo Curve

Mal combo:  

* Cubo 1: intercambia 1 ETH por 400 DAI
* Cubo 2: agregue 400 DAI al grupo Curve

Cuando ingresa 400 DAI en el Cubo 2, su transacción fallará una vez que el resultado del intercambio en el Cubo 1 le dé menos de 400 DAI, lo cual no es infrecuente. Dejar una diferencia en la entrada del segundo cubo puede aumentar significativamente las posibilidades de éxito. En el ejemplo de "Buen combo", la transacción sólo fallaría cuando el precio de ETH cayera por debajo de $380 \(&gt; 5%\) entre el momento en que configura el combo y lo envía.

### **¿Por qué no puedo enviar aunque sé que fallará?**

Es un mecanismo para evitar que pierda dinero fácilmente.

### **¿Cómo cancelo mi transacción pendiente?**

Puede utilizar el botón "cancelar" en la aplicación si está utilizando MetaMask o Trust. Para otras carteras, puede consultar sus sitios web oficiales para obtener más detalles. Alternativamente, también puede enviar otra transacción con la misma billetera y el **mismo nonce** con un precio de gas más alto. 

### **Mi transacción está bloqueada, pendiente de confirmación**

En esta situación, asegúrese de no seguir enviando transacciones. Cada nueva transacción quedará pendiente hasta que se confirme la transacción más antigua. Puede deshacerse de la transacción atascada acelerándola o cancelandola, dependiendo de si la billetera que está usando tiene esa opción de forma nativa. Por ejemplo, Metamask o Trust Wallet tienen opciones para cancelar o acelerar las transacciones.

Alternativamente, si su proveedor de billetera no tiene una opción de acelerar o cancelar, aún puede eliminar la transacción atascada enviando una transacción de 0 ETH a su dirección \(a usted mismo\) usando el mismo nonce \(número de identificación\). Puede inspeccionar el nonce en su transacción en [Etherscan](https://etherscan.io/) y usar servicios como [MEW](https://www.myetherwallet.com/) y [MyCrypto](https://mycrypto.com/) para enviar esta transacción con un costo de gas más alto y reemplazar la atascada.

### **No puedo presionar el botón de enviar**

Intente volver a conectar su billetera.

### **No sé qué construir, ¿hay algún combo de ejemplo?**

Visita [la página Explorar](https://furucombo.app/explore) para inspirarte.

### **¿Cómo guardo mi combo?**

Cuando configure un combo, haga clic en el ícono de cadena debajo del botón de enviar. Obtendrás un enlace al combo actual.

![](../.gitbook/assets/image%20%2820%29.png)

### **¿Cómo comparto mi combo?**

Cuando configure un combo, habrá un enlace "compartir" en la parte inferior, haga clic en el icono de la cadena para obtener el enlace o haga clic en el icono de Twitter para compartirlo en Twitter.

![](../.gitbook/assets/image%20%2815%29.png)

### **Actualizo el precio y todavía dice que fallará**

En la mayoría de los casos, se debe a que el precio volvió a cambiar y es necesario actualizar los números.

Además, si está utilizando un cubo de 1inch y ve este mensaje de error varias veces, intente utilizar otro cubo de intercambio para obtener una cotización más estable.

### **El sitio no se carga**

Los siguientes pasos pueden resolver sus problemas:

* Si usa el navegador Brave, cambie a otro navegador para descartar los problemas del navegador. Si está relacionado con el navegador Brave, algunas acciones a tomar que pueden ayudar son:
  * Borrar datos de caché y cookies para el sitio
  * Actualización completa con control + F5 \(or cmd + r\)
  * Desactive la billetera Brave \(o se ha utilizado la billetera no predeterminada, por ejemplo, metamask, dapper, etc.\)
  * U otras extensiones que podrían estar interfiriendo con la conexión adecuada de la billetera
  * Si después de intentar todos los pasos anteriores, sigue fallando. Desafortunadamente, le sugerimos que acceda a Furucombo usando otro navegador, ya que esas incompatibilidades provienen del navegador Brave.
* Asegúrese de que su conexión a Internet funcione y sea estable
* Reinicie el navegador e intente conectarse nuevamente
* Intente actualizar el sitio con control + F5
* Verifique si hay alguna actualización para su navegador o proveedor de billetera utilizado, si es así, actualícelo a la última versión.



🧊 Special thanks to [Crypto Lunatico](https://www.youtube.com/c/CryptoLunatico) for translating this page.


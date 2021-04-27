---
description: 'Tutorial: Create Flashloan Combo on Furucombo'
---

# Combo Prestamo Flash

![](../.gitbook/assets/image%20%2825%29.png)

## **¿Qué es Flashloan?**

Los Flashloan son introducidos por [Aave](https://app.aave.com/home), un protocolo de préstamos de código abierto para que cualquiera pueda depositar y pedir prestado activos criptográficos. Básicamente, los flashloans permiten a los usuarios pedir prestado cualquier monto hasta la liquidez total disponible sin ninguna garantía, siempre que el préstamo se reembolse en la misma transacción. Si el préstamo no se reembolsa, se revertirá toda la transacción. Con flashloan, cualquiera puede acceder a una gran cantidad de liquidez y utilizar el préstamo con otros protocolos como desee. Puedes convertirte en una "ballena" sin tener capital.

En el momento de redactar este artículo, hay tres grupos que ofrecen Flashloan:

* **Aave**: 22 tokens disponibles con una tarifa del 0.09%
* **dYdX:** 3 tokens disponibles sin tarifa \*
* **Uniswap V2:** más de 100 tokens disponibles con una tarifa del 0.3%

```text
*Tenga en cuenta que flashloan en dydx no es una función del consumidor.
Se logra mediante el encadenamiento de las acciones de Retiro, Llamada y Depósito de los desarrolladores.
```

Entonces, flashloan parece una muy buena oferta. ¿Para qué lo puedes usar exactamente? [Marc Zeller](https://twitter.com/lemiscate) de Aave ha escrito [un artículo](https://medium.com/aave/sneak-peek-at-flash-loans-f2b28a394d62) muy agradable que demuestra algunos de los principales casos de uso de flashloan.

Resumimos los casos de uso:

* Operaciones de arbitraje
* Permuta de garantías
* Auto-cobertura
* Autoliquidación
* \(Deuda\) Swap de tipos de interés
* \(Deuda\) Canje de monedas

El caso de uso más popular con diferencia son **las operaciones de arbitraje**. Para aquellos que no están familiarizados, el arbitraje es la estrategia de obtener ganancias de las diferencias de precios entre diferentes mercados. Para obtener una cantidad significativa de ganancias, necesitará un capital sustancial para comenzar. Y aquí es donde ocurre la magia: usamos flashloan para generar dinero gratis sin costo inicial.

## **Antes de empezar**

Hay algunas cosas importantes que debe comprender:

> Para los comerciantes de arbitraje, Furucombo reduce las barreras de entrada para construir legos de dinero, proporcionando todos los elementos necesarios para crear estrategias de arbitraje, incluidos los flashloan hasta ahora solo para programadores. Pero tenga en cuenta que Furucombo **NO** encuentra oportunidades de arbitraje para usted. Tendrás que encontrarlo tú mismo. ✊🏻

Suficiente con el descargo de responsabilidad, vayamos a la lista de verificación. 👇🏻

```text
Encuentre una oportunidad de arbitraje >0.09% para cubrir la tarifa de flashloan
Tenga algo de ETH en su billetera, suficiente para pagar la gasolina
```

El ejemplo que usamos a continuación es una oportunidad de arbitraje encontrada entre KyberSwap y Uniswap V1 hace unos meses.

```text
Diferencia de tarifa: 20 +%
1 DAI = 1,2411 sUSD en Uniswap
1 sUSD = 0,9927 DAI en Kyberswap
👉🏻 Compre bajo, venda alto: Compre sUSD en Uniswap y véndalo en Kyberswap
```

Ahora que encontró la diferencia de tarifas, empecemos a crear el combo. El combo completo debería verse así:

```text
Pedir prestado 100 DAI en Flashloan
Cambie 100 DAI a 122.83649 sUSD en Uniswap
Intercambia 122.83649 sUSD a 122.83429 DAI en Kyberswap
Pague 100.09 DAI a Flashloan
Te quedas con 22.74429 DAI de ganancia.
```

## **Paso a paso**

### 1. Va a [Furucombo](https://furucombo.app/) <a id="9194"></a>

### 2. **Agregue un cubo Uniswap V1** <a id="126f"></a>

![](../.gitbook/assets/uni-v1.png)

```text
1️⃣ Haga clic en el cubo con el símbolo '+'
2️⃣ Elija 'Swap Token' en la sección Uniswap V1
3️⃣ Ingrese la entrada: 100 DAI
4️⃣ Salida generada desde Uniswap: 122.83649s USD
5️⃣ Haga clic en 'set'
```

### 3. **Agregar un cubo Kyberswap** <a id="dcdb"></a>

![](../.gitbook/assets/kyber%20%281%29.png)

```text
1️⃣ Haga clic en el cubo con el símbolo '+'
2️⃣ Elija 'Swap Token' en la sección Kyberswap
3️⃣ Ingrese la entrada: 122.83649 sUSD
4️⃣ Salida generada desde Kyberswap: 122.83429 DAI
5️⃣ Haga clic en 'set'
```

{% hint style="success" %}
**💡 Sugerencias:** si su entrada coincide con la salida del cubo anterior, introduzca una cantidad ligeramente menor en lugar de la cantidad exacta. De esta manera, puede evitar fallas en el combo debido a la diferencia de tarifas.
{% endhint %}

### 4. **Agregar cubo Flashloan** <a id="de6a"></a>

![](../.gitbook/assets/flashloan.png)

```text
1️⃣ Haga clic en el cubo con el símbolo '+'
2️⃣ Elija 'flashloan' en la sección Aave
3️⃣ Ingrese la cantidad: 100 DAI
4️⃣ Haga clic en 'set'
5️⃣ Aparecen dos cubos. El primer cubo pide prestado 100 DAI y el segundo cubo se pagan 100.09 DAI
```

### 5. **Arrastra el primer cubo de flashloan a la parte superior** <a id="81e4"></a>

Esto es simplemente ajustar el orden de ejecución. Desea pedir un flashloan desde el principio para tener el capital inicial. Entonces, simplemente haga clic y arrastre el cubo de préstamo a la parte superior y mantenga el cubo de pago en la parte inferior.

El combo final se vería así …

![](../.gitbook/assets/arb.png)

### 6. **Conectar billetera** <a id="72ba"></a>

### 7. **Ejecutar** <a id="a283"></a>

🎉 ¡Bravo! Ha ganado dinero con cero capital. No olvide compartir su resultado en Twitter. 🎉

![](../.gitbook/assets/0_kfym6huwloi4txxa.gif)



🧊 Special thanks to [Crypto Lunatico](https://www.youtube.com/c/CryptoLunatico) for translating this page.


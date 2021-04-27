# Guía para principiantes

![](../.gitbook/assets/image%20%2817%29.png)

Bienvenido a Furucombo. En esta guía, analizaremos todos los conceptos básicos que necesita saber para crear un combo con éxito. Antes de comenzar, hablemos de "¿qué es Furucombo?".

Furucombo es una herramienta creada para que los usuarios finales optimicen su estrategia DeFi simplemente arrastrando y soltando. Es como construir tus propios legos DeFi, pero no necesitas saber cómo codificar. Visualiza complejos protocolos DeFi en cubos. Los usuarios solo necesitan ingresar entradas / salidas y configurar órdenes de los cubos \(a esto lo llamamos un “combo”\), luego Furucombo empaquetará todos los cubos en una transacción y los enviará. Esta es una gran herramienta para las personas que desean realizar acciones a través de diferentes protocolos, especialmente aquellos que desean aprovechar el flashloan. \(Cubrimos flashloan en el artículo [aquí](https://medium.com/furucombo/create-flashloan-combo-on-furucombo-c7c3b23267f0)\).

Ahora tienes una idea de lo que es Furucombo, ¡comencemos!

## **Guía de interfaz Furucombo**

### ・DeFi Menu <a id="e7c5"></a>

![](../.gitbook/assets/image%20%2829%29.png)

Para comenzar a crear un combo, primero, deberá seleccionar un protocolo DeFi. Haga clic en el cubo “＋” y aparecerá un menú de protocolos DeFi. Aquí puede elegir qué protocolo DeFi desea poner en su combo. Cada botón representa un cubo a configurar. Cada cubo significa una acción a ejecutar. La función de búsqueda en la parte superior le permite buscar por nombre del token y acción defi \(por ejemplo, intercambiar, agregar liquidez, etc.\)

### ・**Fondos iniciales** <a id="1bcf"></a>

![](../.gitbook/assets/image%20%2830%29.png)

Cuando comience a configurar cubos, es posible que vea una sección en la parte superior izquierda llamada "Fondos iniciales". Significa los fondos que debe proporcionar al comienzo del combo para iniciar la transacción.

Los fondos iniciales se envían directamente **desde su billetera**. Dicho esto, debe tener suficiente saldo de los tokens en su billetera, de lo contrario, la transacción **NO** se ejecutará. Cuando su billetera esté conectada, el saldo de la billetera de cada token se mostrará aquí para que siempre pueda verificar antes de enviar el combo.

### ・**Usted recibirá** <a id="5cd0"></a>

![](../.gitbook/assets/image%20%281%29.png)



A la izquierda, verá una sección "**Recibirás**". Estos son los fondos que se devolverán a su billetera al final de la transacción. Es el resultado de todas las entradas y salidas que ha creado a la derecha, que se actualizan cada vez que se realiza un cambio en un cubo.

```text
👩🏻‍🏫 Solo piensa que 
"Fondos iniciales" es la cantidad que inviertes y 
"Recibirás" es la cantidad que obtienes al final.
```

## **Paso a paso**

### **Paso 1: configurar cubos** ⚙️ <a id="0903"></a>

![](../.gitbook/assets/image%20%2831%29.png)

Cuando selecciona un protocolo, se le indica que ingrese los detalles del cubo. Aquí verá con frecuencia los términos "Entrada" y "Salida".

```text
Entrada significa cuánto token gastará al ejecutar esta acción.
Salida significa la cantidad de token que recibirá al ejecutar esta acción.
```

La fuente de entrada pueden ser tokens que tenga en su billetera o pueden ser salidas de cubos anteriores. Una vez que haya configurado el cubo, siempre puede editarlo haciendo clic en el icono de bolígrafo o eliminarlo haciendo clic en la papelera que está en la parte superior derecha de cada conjunto.

### **Paso 2: Arrastra y suelta** 🖱 ✋🏻 📦 <a id="5853"></a>

![](../.gitbook/assets/1_ioy6idmu4smf-3gcuoebmw.gif)

Todos los cubos que configure se pueden arrastrar. Simplemente **arrástrelos** en el orden que desee. Cuando se envía el combo, las acciones se ejecutan según el orden de los cubos.

> Ejemplo: cuando crea flashloan, verá aparecer dos cubos. \(El primer cubo significa "pedir prestado" y el segundo cubo significa "pagar prestamo"\). Lo siguiente que debe hacer es agregar más cubos \(acciones que desea hacer con los tokens prestados\) y arrastrarlos entre los dos cubos flashloan.

### **Paso 3: conecta tu billetera** 👛 <a id="f5ac"></a>

![](../.gitbook/assets/1_oqusodpu0ues59xxpalg0q.gif)

Puede crear un combo sin conectar su billetera. Pero si desea ejecutar el combo, debe conectar su billetera. Simplemente haga clic en el cubo con un icono de billetera. Luego elija su billetera para conectarse.

### **Paso 4: ejecutar un combo** 🔗 🎉 🎁 <a id="bafb"></a>

![](../.gitbook/assets/1_n7ovqm9e2xx-z8vawws52a.gif)

El flujo completo de ejecutar un combo sería:

1️⃣ Haga clic en "Aprobar" cuando sus fondos iniciales sean tokens ERC20. Solo necesita hacer esto una vez por token.

2️⃣ Haga clic en "Enviar", luego Furucombo ejecutará una estimación de su combo. Si la transacción falla, aparecerá un mensaje como recordatorio para que pueda modificar su combinación.

3️⃣ Una vez que su combo se envía correctamente, el botón cambia a "**Nuevo Combo**" y aparece un mensaje con el enlace de la transacción. Cuando vea estos cambios, ¡felicidades!

¡Has completado un combo! No olvide compartir su resultado en Twitter simplemente haciendo clic en el ícono de Twitter.

También hicimos un video tutorial de esta guía. Échale un vistazo 👇🏻

{% embed url="https://www.youtube.com/watch?v=wCfMm2a91qs" %}



🧊 Special thanks to [Crypto Lunatico](https://www.youtube.com/c/CryptoLunatico) for translating this page.


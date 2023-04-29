---
description: RTFM
---

# 🛠 Configurando

Si tienes algun problema, visita las [Preguntas Más Frecuentes](faq.md).

Antes de configurar, asegurate de haber habilitado el estado de actividad en la configuración de Discord:

<figure><img src="https://cdn.discordapp.com/attachments/1030245442358886455/1030245477175795752/Captura_de_pantalla_2022-10-13_172632.png" alt=""><figcaption></figcaption></figure>

## Proceso de Configuración

* Dirigete a https://discord.com/developers/applications/.
* Click en **New Application** en la esquina superior derecha

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Escoge un nombre para la Aplicación, este será mostrado como "Jugando" en el estado; dale a **Create**.
* Copia la **Application ID** y copialo en el campo de **ID** en CustomRP, luego dale a **Conectar**. Si lo hiciste bien, tu estado de Discord debería decir "Jugando a **\[Nombre de la App]**".
  * Nota: Si tienes un estado personalizado (el que tiene emoji), tendrá prioridad sobre tu CustomRP. Sin embargo, se verá en la ventana emergente del perfil.

![image](https://cdn.discordapp.com/attachments/1030245442358886455/1030250456749965322/Captura_de_pantalla_2022-10-13_174558.png)

* En la página de su aplicación, vaya a Rich Presence -> Art Assets y cargue al menos una imagen en Rich Presence Assets si desea utilizarlos. En CustomRP, hay un práctico botón **Cargar activos** en el menú Archivo (también puede usar Ctrl+U) que lo llevará allí si su campo de ID está configurado correctamente.
  * Alternativamente, puede simplemente insertar una URL a la imagen en el campo **Key**.
  * Nota: Si bien puedes nombrar tu estado con cualquier nombre de hasta 999 caractéres, la API solo aceptará nombres con 256 caractéres como máximo.
* Navegue a la página del visualizador para configurar los campos **State, Details, Large Image Key, Large Image Text, Small Image Key, Small Image Text, Party Size, Party Max**. Todos esos son opcionales.
* Una vez que hayas encontrado la configuración que te gusta, copia los valores en los campos correspondientes de CustomRP.
  * Tip: Puedes pasar el cursor sobre casi cualquier control en la aplicación (incluida la línea de etiquetas **Detalles**) y obtendrá información sobre herramientas.
* Si también quieres configurar botones, completa los campos Texto y URL.
  * Nota: Cuando haga clic en los botones en su propia presencia, no funcionarán, pero no se preocupe, funcionarán para todos los demás. Es un problema del lado de Discord.
* Presiona **Actualizar Presencia** (o **Conectar** si aún no estás conectado).
* Felicidades, has terminado!

### Uso más de un cliente de Discord, ¿qué hago?

Si tienes más de un cliente de Discord y quieres que su presencia se muestre en una cuenta diferente de la aplicación elegida automáticamente, presiona **Desconectar**, luego manten presionadas las teclas Ctrl+Shift en tu teclado y presiona **Conectar* *. Aparecerá una ventana con la entrada de un número, ingresa el número 1, cierra la ventana y presiona **Conectar** nuevamente, sin Ctrl+Shift. En caso de que vuelva a ser una cuenta incorrecta, intenta con el número 0, luego con el 2 y así sucesivamente hasta llegar al 9.

Ten en cuenta que si tienes varios clientes de Discord ejecutándose al inicio, es posible que el número de tubería asignado a cada cliente no sea persistente de inicio a inicio y puede cambiar según el cliente que se inició primero. Para evitar eso, puedes iniciar clientes adicionales manualmente o usar el Programador de tareas de Windows para retrasar el inicio de los clientes.

Si tienes 2 cuentas que usas al mismo tiempo y quieres que cada una de ellas tenga una presencia diferente, entonces sigue estos pasos:

* Configura tu cuenta principal primero con las instrucciones anteriores.
* Descarga la última versión **portable (.zip)** de CustomRP (ya sea de nuestra [página web](https://www.customrp.xyz) o [la página de Versiones de GitHub](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) y descomprimela donde sea
  * Esto solo funciona con las versiones 1.16 y anteriores.
* Abre `Start Second Instance.bat` o crea un acceso directo a CustomRP.exe con un argumento `--second-instance` (o `-2`) al final
* Configura el programa de la misma manera que hiciste con tu instancia principal.
  * Tip: Si ya tienes un ajuste preestablecido que te gustaría usar con tu segunda instancia, puedes editar el archivo .bat o el acceso directo para incluir la ruta al ajuste preestablecido. Ejemplo: `CustomRP.exe -2 "C:\Alguna Carpeta\Preestablecido.crp"` (Las comillas alrededor de la ruta son necesarias si la ruta tiene espacios).
* Antes de conectar, cambia la tubería como se describe anteriormente y conecta.

Mensaje del Desarrollador: Si usas 3 o más cuentas al mismo tiempo, entonces... ¿por qué? Pero también si muchos de ustedes me regañan, agregaré soporte para usar más instancias.

## Notas

* Si no quieres configurar una imagen pequeña o grande, deja en blanco todos los campos relacionados en el programa.
* Si no se establece una imagen grande, se ignorará la configuración de imagen pequeña.

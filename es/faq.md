# ❓ Preguntas Más Frecuentes

## Preguntas

### Puedo añadir mas de dos botones?

Nop, lastimosamente es una limitación de Discord

### Puedo Usar Otro Tipo de Actividad (Ej. Escuchando, Viendo, Transmitiendo)?

Nop, también es una limmitación de Discord

### Por qué si configuro una marca de tiempo un par de días en el futuro, Discord solo muestra cuántas horas quedan?

Adivinaste, tambíen es una limitación de Discord

### Habrá una Versión para Linux/Mac?

La app esta construida usando una biblioteca solo de Windows, por lo tanto lanzar versiones para Linux/Mac significaría reescribir toda la app desde 0 en una biblioteca/lenguaje de programación diferente lo cual aún no esta planeado

### Se abrió una ventana llamada "Pipe/Tubo" por alguna razón, ¿qué es esto?

Se abrió porque presionó Ctrl + Shift y hizo clic en el botón Conectar (o Ctrl y el botón Conectar o Reconectar en el menú del ícono de la bandeja en versiones anteriores). Déjalo en -1 y ciérralo. Se usa para situaciones en las que tiene más de un cliente de Discord ejecutándose al mismo tiempo. Cambiar el número de tubería elige efectivamente en qué cliente desea que esté su presencia.

## Solución de Problemas

Antes de intentar nada, asegurate de contar con la ultima versión de CustomRP

### Cuando hago clic en los botones de mi perfil, no funcionan.

Los botones no funcionarán para usted en el cliente de escritorio con el que está usando CustomRP, es una peculiaridad de Discord. Puede probar sus botones desde un cliente móvil o web, o simplemente preguntarle a otra persona.

### He instalado CustompRP pero no se inicia

Lo más probable es que su antivirus impida que se inicie la aplicación. Agregue la carpeta `%appdata%\CustomRP` a las excepciones.

### Instalé CustomRP, permití el análisis y la aplicación ya no funciona.

Elimine la aplicación en el Administrador de tareas, elimine la carpeta `%localappdata%\maximmax42`, inicie la aplicación nuevamente y no permita el análisis.

### La aplicación se ha conectado, pero no veo el estado en mi perfil.

Asegúrate de haber habilitado el estado de actividad en la configuración de Discord:

<figure><img src="https://user-images.githubusercontent.com/2225711/188219661-49713f90-fa76-4645-b04a-fc1bc0f029bd.png" alt=""><figcaption></figcaption></figure>

### La aplicación funcionaba, pero ahora se conecta indefinidamente.

Es posible que haya obtenido un tiempo de espera de Discord debido a la conexión/cambio de presencia mucho. Desconecte, espere de 5 a 10 minutos, intente conectarse de nuevo. Reiniciar Discord también podría ayudar.

### La aplicación dice "¿ID Incorrecto?"/"¿Se está ejecutando Discord?" o se conecta indefinidamente aunque estoy seguro de que hice todo bien y Discord se está ejecutando.

Aquí tienes algunas cosas que puedes probar:
- **Asegúrate de estar usando un cliente independiente de Discord (no en el navegador).**
- Si tienes instalado BetterDiscord/Vencord/etc, desinstálalo, permite que CustomRP se conecte a Discord al menos una vez y luego vuelve a instalarlo.
- Si usas varios clientes de Discord, cierra temporalmente todos excepto el que deseas usar para la RichPresence.
- Ejecuta CustomRP como administrador (Click Derecho al programa y opción "Ejectuar como Administrador).
- Agrega `%appdata%\CustomRP` o, en caso de que estés utilizando una versión portátil, la carpeta donde hayas extraído CustomRP, a las excepciones del firewall y/o antivirus, luego reinicia tu PC por completo.
- Reinstala Discord.

Si nada de eso ayudó, lamentablemente no puedo sugerirte nada más, perdón.

### La aplicación funcionaba antes, pero luego se bloqueó y ahora no se inicia en absoluto.

Tal vez haya insertado una cadena larga de texto elegante (o texto en un idioma que usa letras no latinas) en un campo y eso bloqueó la aplicación. Para solucionar esto, presione Win+R, escriba `%localappdata%\maximmax42` y elimine o cambie el nombre de las carpetas con CustomRP en el nombre, luego inicie la aplicación. Tenga en cuenta que esto restablece la aplicación por completo.

### La aplicación sigue fallando al actualizar/intentar conectarse/etc.

Si puede iniciar la aplicación y obtener un informe de bloqueo, y dice `System.IO.FileNotFoundException: no se pudo cargar el archivo o el ensamblaje...`, reinstale la aplicación.

Si no puedes resolver el problema, escribenos en el canal de `#support` en el [Servidor de Discord de CustomRP](https://www.customrp.xyz/discordserver), O envia un Mensaje al Creador (maximmax42#5572),(O puedes comunicarte conmigo, el Traductor de Español, en Discord Como: SirAmong#1868) o [Abre un Problema](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).

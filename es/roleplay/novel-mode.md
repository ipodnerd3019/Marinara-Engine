# Novel Mode: escribir una historia en conjunto

Esta guía explica Novel Mode en Marinara Engine. Novel Mode convierte un chat de Roleplay en una sola página continua, como un manuscrito, donde tú y la IA escriben una historia en conjunto. Cubre cómo empezar una novela, escribir y editar pasajes, guiar a la IA y escuchar la historia.

## Qué es Novel Mode

Novel Mode es un estilo de visualización para los chats de Roleplay. La historia se lee como una sola página en lugar de un chat: no hay avatares, nombres, marcas de tiempo ni burbujas de mensaje. Cada vez que la IA escribe, añade un pasaje a la página. Los párrafos llevan sangría como en un libro impreso, y los pasajes se suceden sin cortes.

A diferencia de un roleplay normal, la IA también escribe a tu protagonista. Escribe sus acciones, diálogos y pensamientos, así que la historia avanza sin esperar tu turno. Tú la guías de otra manera: escribes pasajes propios, editas lo que ya está en la página y das instrucciones breves para el siguiente pasaje.

Por debajo, una novela sigue siendo un chat de Roleplay. Los lorebooks (libros de trasfondo), los resúmenes, la memoria, las ramas y los agentes funcionan igual que en cualquier roleplay.

Con varios personajes, una novela usa siempre el modo de grupo **Merged** (fusionado): la IA escribe a todos los personajes con una sola voz, como lo hace un novelista, así que no hay turnos que tomar. En las novelas, **Chat Settings** (Ajustes del chat) oculta las opciones de modo de grupo, orden de respuesta y color de diálogo. El **Scenario Override** (Escenario alternativo) del grupo sigue aplicándose.

## Empezar una novela

1. Empieza un nuevo chat de Roleplay.
2. En el primer paso del asistente de configuración, establece **Display style** (Estilo de visualización) en **Novel** (Novela).
3. Termina el asistente. Los personajes y la persona son opcionales. Añade personajes solo si quieres que sus tarjetas de personaje estén en el contexto de la historia.

Al elegir **Novel** conservas tus agentes, como en cualquier roleplay. Los sprites, el HUD y los efectos del clima aparecen cuando los agentes que los generan están activados (Expression Engine, World State y los agentes de seguimiento); quita esos agentes en el asistente o en **Chat Settings** para tener una página limpia. Las novelas muestran un icono de libro en la lista de chats.

Elegir **Novel** también selecciona **Marinara's Novel Preset**, que le indica a la IA que escriba a tu protagonista (ver más abajo). Puedes elegir otro preset (ajuste guardado) en el paso **Preset** del asistente o más tarde en **Chat Settings**. Si vuelves a otro estilo de visualización en el mismo asistente, regresa tu preset anterior, salvo que hayas elegido uno distinto mientras tanto.

## Escribir y editar

- **Añadir tu propio texto:** escribe en la línea al final de la página, que dice **Keep writing, or press Send…** (Sigue escribiendo o pulsa Enviar). Cuando sales de la línea o pulsas **Send** (Enviar), tu texto se convierte en el siguiente pasaje de la historia.
- **Editar cualquier cosa de la página:** toda la página es un solo editor. Haz clic en cualquier lugar y escribe, como en un procesador de texto. Tus cambios se guardan solos un momento después de que dejas de escribir, y **Ctrl+Z** los deshace.
- **Formato:** el texto de un pasaje puede ir en *cursiva* o en **negrita**. Selecciónalo y pulsa **Ctrl+I** o **Ctrl+B** (**Cmd** en una Mac). Se guarda como markdown, como `*italic*` y `**bold**`, y los `*text*`, `_text_`, `**text**` y `__text__` que ya estén en un pasaje se muestran en cursiva y en negrita. Cualquier otro marcado, como encabezados, listas, enlaces y HTML, se muestra como texto sin formato y no recibe ningún tratamiento especial. Los saltos de línea se conservan: un pasaje cuyos párrafos están en líneas simples los mantiene así cuando lo editas.
- **Seleccionar entre pasajes:** puedes seleccionar, copiar y borrar texto que abarca varios pasajes. Cada pasaje sigue siendo su propia parte de la historia: borrar a través de varios quita texto de cada uno, nunca los pasajes en sí. Si vacías un pasaje por completo y sigues adelante, Marinara te pregunta si quieres eliminarlo.
- **Acciones del pasaje:** apunta a un pasaje, o pon el cursor en él, para ver sus acciones en el margen: copiar, traducir, reintentar, marcador, fijar o nota, **Mark as new start** (Marcar como nuevo inicio), ocultar a la IA, crear una rama y eliminar, además de **Speak** (Hablar) cuando la conversión de texto a voz está activada. El último pasaje también tiene **Peek prompt** (Ver el prompt), y un pasaje escrito con una instrucción tiene **Stored guidance** (Guía guardada), que muestra la dirección que se le dio. En un teléfono, toca el pasaje, o mueve el cursor a él, para mostrarlas.

## Pedirle más a la IA

La barra de mensajes bajo la página funciona como en cualquier roleplay, con una diferencia: lo que escribes ahí nunca se convierte en un mensaje. Solo guía el siguiente pasaje.

- **Send** con la barra vacía escribe los siguientes párrafos de la historia.
- Escribe una dirección breve, como `a storm arrives` ("llega una tormenta"), y pulsa **Send**. La IA guía el siguiente pasaje hacia ella sin escribirla en la historia.
- Los comandos slash, el dictado y los selectores de conexión y de persona funcionan como siempre. No se ofrecen los adjuntos ni las respuestas rápidas **Post only** (Solo publicar) y **Guide reply** (Guiar la respuesta): nada de lo que publicas se convierte en un mensaje, y **Send** ya envía tu texto como instrucción.
- Impersonate no se ofrece en una novela: no tienes un turno que escribir, porque la IA ya escribe a tu protagonista. El comando `/impersonate`, la respuesta rápida Impersonate y los ajustes de Impersonate del chat están ocultos.
- Con el agente CYOA activado, elegir una de sus opciones guía el siguiente pasaje hacia ella, como una instrucción. Nunca se convierte en un mensaje tuyo, así que el interruptor de Impersonate de las opciones está oculto. Con **Add CYOA choices to the message box instead of sending them** (Añadir las opciones CYOA al cuadro de mensaje en lugar de enviarlas) activado, la opción va a la barra de mensajes, donde puedes combinarla con tu propia instrucción.
- Para volver a escribir un pasaje, usa reintentar (**Regenerate**, Regenerar) en sus acciones. Tus ediciones se guardan primero. Con **Guide swipes/regens with chat input** (Guiar swipes/regeneraciones con la entrada del chat) activado en **Settings** (Configuración) y texto en la barra de mensajes, el botón dice **Regenerate (guided)** y guía la nueva versión hacia ese texto, igual que **Send**. Cuando un pasaje tiene más de una versión, las flechas debajo de él cambian entre ellas, y cualquier edición que estuvieras escribiendo se guarda en la versión en la que la escribiste.
- Mientras la IA escribe, **Send** se convierte en **Stop** (Detener).

## Cómo se le indica a la IA que escriba una novela

**Marinara's Novel Preset** es un preset integrado escrito para novelas. Le dice a la IA que está coescribiendo un solo manuscrito contigo, que escribe a todos los personajes, incluido tu protagonista, y que escribe prosa de libro: párrafos, diálogos entre comillas, *cursiva* solo para pensamientos y énfasis, y ningún otro markdown. Cada pasaje continúa desde donde termina la página y se detiene en una pausa natural, nunca en una pregunta para ti. Sigue la instrucción que escribes en la barra de mensajes sin citarla ni escribir notas sobre ella en el pasaje.

Quién es el protagonista depende de cómo configures la novela:

| Configuración | Protagonista | Elenco |
| --- | --- | --- |
| Sin persona ni personajes | El protagonista al que ya sigue el manuscrito. En una página vacía, la IA establece uno con un nombre, una voz y algo que desea, y lo mantiene coherente. | Sin elenco preparado. La IA introduce personajes a medida que la historia los necesita. |
| Una persona y personajes | Tu persona. Su perfil forma parte de la biblia de la historia. | Tus personajes, cada uno fiel a su tarjeta. |
| Personajes pero sin persona | El protagonista al que ya sigue el manuscrito. Si no lo hay, con un solo personaje, ese personaje, salvo que su tarjeta describa a otra persona, en cuyo caso la IA crea a esa persona. Con varios, la IA elige a uno de ellos, o a un personaje nuevo si las tarjetas apuntan a otra persona. | Tus personajes. |
| Una persona pero sin personajes | Tu persona. | Sin elenco preparado. |

Una persona cuenta cuando tiene una descripción u otro texto. Una que solo tiene nombre cuenta como ninguna persona, ya que la IA nunca ve su nombre. Sin persona, una tarjeta que menciona `{{user}}` se lee como "User", así que las tarjetas escritas para una novela sin persona se leen mejor cuando nombran al protagonista o no mencionan `{{user}}`.

El preset hace algunas preguntas al empezar la novela: la clasificación del contenido (**NSFW** o **SFW**), el punto de vista (tercera, primera o segunda persona), el estilo de narración (cercano al protagonista, alternando entre personajes de punto de vista en los cambios de escena, u omnisciente), el tiempo verbal, la longitud del pasaje (**Length**, Longitud) y el idioma. La primera opción de cada una es la predeterminada.

Al igual que Marinara's Universal Preset, el preset Novel es de solo lectura y no se puede eliminar. Ábrelo en **Presets** y crea una copia editable para cambiar su redacción. Usa tus ajustes de generación de la conexión y del chat en lugar de los suyos propios. Consulta [Editor de presets y gestor de prompts](../prompts/presets.md).

Algunas cosas que conviene saber:

- En los chats de Roleplay, una conexión con su propia sustitución de preset usa ese preset en su lugar, también en las novelas.
- Cambiar más tarde una novela a Visual Novel o Classic con el interruptor **Visual Novel display** (Visualización de novela visual) en **Settings > Appearance** (Configuración > Apariencia) conserva el preset Novel. Elige otro preset en **Chat Settings** si ya no quieres que la IA escriba a tu protagonista. El interruptor también cambia tu estilo de visualización predeterminado para los chats de Roleplay sin un estilo guardado, no solo la novela abierta.
- Otro preset también funciona en una novela, pero la mayoría de los presets de roleplay le dicen a la IA que nunca escriba a tu personaje. Marinara's Universal Preset lo hace, así que con él la IA te deja a tu protagonista.

## Escuchar la historia

Cuando la conversión de texto a voz está activada, las acciones de cada pasaje incluyen **Speak**. Con **Only read dialogues** (Leer solo los diálogos) desactivado, también se lee la narración, con la voz del narrador cuando **Use separate narrator voice** (Usar una voz de narrador aparte) está activado. Con **Only read dialogues** activado, solo se lee el diálogo entre comillas.

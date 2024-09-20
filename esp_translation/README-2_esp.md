# Documentación de Linea

[Linea](https://linea.build/) ies una red de capa 2 lista para desarrolladores, que escala Ethereum proporcionando un entorno equivalente a Ethereum en el que ejecutar transacciones, que luego se envían a Ethereum Mainnet a través de un rollup de conocimiento cero.

Este repositorio de documentación está construido usando [Docusaurus](https://docusaurus.io/), y el sitio en sí está publicado en [`docs.linea.build`](https://docs.linea.build/).

Consulta [más](https://docs-template.consensys.net/) información sobre cómo Consensys utiliza Docusaurus.

## Contribuye a la documentación

¿Ves algo que falta? ¿Error en nuestra documentación? Crea un problema [aquí](https://github.com/Consensys/doc.linea/issues).

¡Alternativamente, ayúdanos a mejorar nuestra documentación! [Haz un fork de nuestro repositorio](https://github.com/ConsenSys/doc.linea/fork),
crea una solicitud de extracción y etiquétanos para revisión. (Para ayuda con esto, consulta [más abajo](#how-to-submit-a-suggestion-or-change)).

Echa un vistazo a algunos [buenos primeros problemas](https://github.com/ConsenSys/doc.linea/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
para comenzar.

### Cómo enviar una sugerencia o cambio

La mejor manera de sugerir un cambio a esta documentación es a través de un proceso conocido como **pull request**.
Si no estás familiarizado con cómo funciona, consulta la [guía de GitHub aquí](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

Si tienes la intención de enviar una solicitud de extracción, abre primero un problema y [enlázalo en tu solicitud de extracción](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue). **Esto es especialmente importante si eres un contribuyente del ecosistema** —
enviar tus detalles en un problema primero hará que sea mucho más fácil para nuestro equipo de documentación procesar tus contribuciones.


Si ese proceso es demasiado complicado para ti, siempre puedes abrir un hilo en el [foro de la comunidad](https://community.linea.build/),
o un ticket en la [página de soporte](https://support.linea.build/hc/en-us).

Si estás familiarizado con hacer una solicitud de extracción, **e recomendamos encarecidamente que ejecutes una versión de esta documentación localmente y previsualices tus cambios localmente antes de enviarlos.**.
De hecho, es parte del proceso de PR.

### Contribuir a tutoriales comunitarios

Si has creado guías y tutoriales detallados, o tienes la intención de hacerlo, nos encantaría presentar tu contenido en nuestra [sección de tutoriales comunitarios](developers/guides/community).

Primero, crea un problema describiendo el contenido que deseas agregar o que tienes la intención de agregar. Si representas a una organización (como una dapp), utiliza el formulario de contribución al ecosistema.

Cuando estés listo para comenzar a trabajar [haz un fork de nuestro repositorio](https://github.com/Consensys/doc.linea/fork),
crea una solicitud de extracción y etiquétanos para revisión.

### Contribuir al Glosario de Conocimiento Cero

¿Te estás adentrando en los rollups de conocimiento cero y te estás topando con la jerga técnica? Hemos comenzado un glosario de conocimiento cero de código abierto para definir algunos términos comunes que podrías encontrar mientras exploras el panorama de L2.

[Forkea nuestro repositorio](https://github.com/Consensys/doc.linea/fork), y agrega un término en orden alfabético a  `docs/reference/glossary.md`. Luego, haz una solicitud de extracción y etiquétanos para revisión.

### Recursos Adicionales

Consulta las [directrices de contribución a la documentación de Consensys](https://docs-template.consensys.net/) para obtener información sobre cómo:

- [Enviar una contribución](https://docs-template.consensys.net/contribute/submit-a-contribution) utilizando forks y solicitudes de extracción.
- Consultar la [guía de estilo de documentación](https://docs-template.consensys.net/contribute/style-guide).
- [Formatear tu Markdown](https://docs-template.consensys.net/contribute/format-markdown) correctamente.
- [Previsualizar la documentación](https://docs-template.consensys.net/contribute/preview) localmente.

## Ejecutar localmente

Necesitarás tener **Node.js** nstalado para ejecutar las vistas previas en vivo de la documentación localmente.

Se recomienda encarecidamente usar una herramienta como [`nvm`](https://github.com/nvm-sh/nvm#installing-and-updating)
para gestionar las versiones de Node.js en tu máquina.

### Instalación de la versión recomendada de Node.js con `nvm`

1. Sigue las instrucciones anteriores para instalar `nvm` en tu máquina, o ve [aquí](https://github.com/nvm-sh/nvm#installing-and-updating).
2. Ve a la carpeta raíz de este proyecto en tu terminal.
3. Ejecuta `nvm install` seguido de `nvm use`. Esto instalará la versión especificada por este proyecto en el archivo `.nvmrc`.

### Ejecutar este proyecto

1. Navega a la carpeta raíz del proyecto después de instalar Node.js.
2. Ejecuta lo siguiente en secuencia, lo cual solo necesita hacerse una vez:

   ```bash
   npm install
   npm run prepare
   ```

3. Para previsualizar y para cada vez después de eso:

   ```bash
   npm run start
   ```

### Construir

    $ npm run build

Este comando genera contenido estático en el directorio `build` y puede ser servido usando cualquier servicio de alojamiento de contenido estático.

### Agregar nuevas palabras al diccionario

Este repositorio incluye un _linter_, que puedes pensar como un corrector ortográfico que también verifica el formato del código y estándares, y mucho más. Es posible que uses una palabra en tu contenido que no sea reconocida por el linter, y tu construcción o commit fallará.

Puedes ejecutar el linter en cualquier momento con el comando `npm run lint`.

Si el linter encuentra una palabra que no reconoce, revisa `project-words.txt` en el directorio raíz; si la palabra que el linter detectó está correctamente escrita, y deseas que pase la prueba del linter, agrégala a `project-words.txt`, guarda, añade y confirma esos cambios, y verifica si pasa.

Para mantener el orden, asegúrate de adherirte al orden alfabético establecido en `project-words.txt`.

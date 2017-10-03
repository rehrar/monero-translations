# ¿Qué es Kovri y por qué es importante para Monero?

Agosto 24, 2017 11:43 por Jamie Holmes

En el último episodio de OpenHours salido el 17 de agosto, algunos colaboradores de Monero se unieron al programa para discutir el proyecto Kovri. El proyecto tiene el objetivo de seguir mejorando la privacidad de la red Monero por medio de hacer la información sobre transacciones prácticamente imposible de deducir. Asimismo, Kovri puede hacerse potencialmente la herramienta perfecta para ocultar direcciones IP.
## La relación entre Kovri y Monero
Kovri es una implementación del router I2P en C++. En pocas palabras, es una red superpuesta de anonimato con propósito general que es similar a Tor. Un router I2P típico está escrito en Java, mientras que Kovri está escrito en el lenguaje C++ que asegura la compatibilidad con la criptomoneda centrada en la privacidad, Monero (XMR). Actualmente, 48 colaboradores están trabajando en el proyecto para lanzar la versión alpha.

¿Qué es Kovri y cómo comenzó? Riccardo Spagni, el mantenedor principal del proyecto Monero, explicó que “puesto que Monero se enfoca en la privacidad, comenzamos a adoptar otros proyectos que no son sólo provechosos al ecosistema de Monero sino beneficiosos a los entusiastas de la privacidad a todas partes. Es cómo comenzó Kovri”.

El comienzo de Kovri replica lo de Monero. Los dos se bifurcaron de los proyectos de código abierto por la falta de confianza en los equipos originales de desarrollo. En el caso de Monero, fue BitMonero. En el caso de Kovri, fue i2pd.

Al principio de 2015, el autor original de i2pd, que es la implementación de I2P en C++, se hizo el único colaborador una vez que un desarrollador realizó un commit en GitHub. Esta acción ofensiva a otros desarrolladores resultó en la terminación del proyecto C++. Más tarde en el otoño de 2015, Anonimal, quien ahora encabeza el desarrollo de Kovri, intentó resucitar el proyecto y hacer paz a los desarrolladores actuales de i2pd.

El primer autor de i2pd no respondió y al contrario comenzó a trabajar en Github de nuevo, fuera de la rama manejada por la comunidad. Por un lado, fue el gesto desafiante y la señal de advertencia, por otro lado, para los desarrolladores que querían perseguir el proyecto.

Para mitigar los daños a las perspectivas de la implementación de I2P en C++, Anonimal dirigió una serie de reuniones que formaron la base del proyecto Kovri, comenzando en el noviembre de 2015. Este grupo hizo la bifurcación de i2pd por el impedimento puesto en su desarrollo.

Anonimal explicó el objetivo de Kovri en el episodio de OpenHours, su primera discusión pública del proyecto: “Básicamente, podremos llevar el anonimato de transacciones Monero al nivel más alto en comparación con la funcionalidad actual de Monero, técnicamente a la capa de red".

En la propuesta del final de 2016, Anonimal explicó el razonamiento para considerar Kovri como alternativa al proyecto Tor:

> "Mientras que me gusta mucho Tor y voy a defenderlo con uñas y dientes, en este tiempo hay dos asuntos que me preocupan más con respecto al proyecto:

> Primero, bajo una nueva administración, el estado actual del proyecto está en la corriente cuestionable: los voluntarios claves que han estado con el proyecto desde el principio lo están abandonando, hay conflictos abiertos en la organización y muchos rumores (fundados y sin fundamento) sobre la interferencia del gobierno estadounidense en el proyecto.

> Segundo, el talón de Aquiles de Tor es lo que autoridades, consenso, y enrutamiento de cebolla ("onion-routing") basado en los flujos y actualmente implementado en Tor no son realmente descentralizados."

Pero, ¿no ofusca Monero a los destinos y los montos de transacciones? Sí, pero cuando un usuario realiza una transacción, dice a la red que quiere ser incluido al próximo bloque. Su dirección IP, junto con otros metadatos, se filtra. Pero su dirección IP no se registra para siempre en la cadena de bloques.

Los agentes malintencionados podrían averiguar direcciones IP si vigilan activamente la red, lo cual explica por qué Kovri es tan importante. El colaborador de Monero SamsungGalaxyPlayer (SGP) dijo: "Con Kovri será extremadamente difícil, ojalá imposible, vigilar esta información."

Spagni añadió que, aunque sea posible, este tipo de ataque sería difícil de realizar. "Su dirección IP no está integrada en la transacción. Los agentes necesitan ejecutar sus propios nodos y tienen que observar cuál nodo transmite la transacción primero, por eso es un ataque difícil de hacer. Sucedió con Bitcoin en el pasado y quizá pueda estar pasando con Monero, no sabríamos..."

### "El proyecto Monero nunca terminará... Kovri es importante para la privacidad y descentralización"

Una de las preguntas más interesantes hechas durante el programa fue lo siguiente: "Supongamos que Kovri está integrado y hay monederos móviles para XMR. ¿Cuáles son los desafíos más grandes a largo plazo a los que se enfrenta Monero?

SGP respondió que dos desafíos más importantes son seguir siendo descentralizado y mejorando la privacidad. "Ahora no tenemos sistemas perfectamente privados. Necesitamos seguir llegando a esta meta", SGP continuó. "Estamos en el momento cuando Monero está suficientemente privado, ahora hay que hacerlo suficientemente eficaz".

Por la ofuscación, las transacciones de Monero son más grandes que las de Bitcoin porque más datos se acumulan en la cadena de bloques. Reducir el tamaño de las transacciones ha sido una prioridad clave del equipo Monero. Hay dos maneras efectivas de hacerlo según la transcripción de la reunión reciente de desarrolladores en Monero: RingCT 2.0 y las firmas sublineales de anillo + CT ("sublinear ring signatures") del investigador Tim Ruffing, los cuales no requieren la instalación confiable.

> "El proyecto Monero nunca terminará, por eso siempre habrá más trabajo. Creo que Kovri es una parte importante para hacerlo más descentralizado y privado." - SGP

Mientras que Kovri mejora la descentralización y la privacidad de Monero, también ayudará a aumentar la adopción y el valor de XMR. La gente pondrá más confianza en la criptomoneda si está segura que cada transacción mantiene su anonimato. Después del lanzamiento de la versión beta de Kovri, se incluirá por defecto y cada usuario se beneficiará de la capa adicional del anonimato I2P.

## La comunidad ideológica impulsa el desarrollo

Otros temas de discusión durante el episodio de OpenHours fueron el consenso de cadena de bloques y el progreso de desarrollo. "Lo que es más interesante que el precio (de XMR) es el progreso constante en el desarrollo", dijo Spagni.

> "Hemos visto nuevos colaboradores unirse al proyecto regularmente. Algunos de ellos se quedan por un corto tiempo mientras que otros se quedan por mucho tiempo. Están trabajando sin compensación. Hay unos colaboradores que recaudaron fondos mediante nuestro sistema de financiación colectiva ("crowdfunding") pero la gran mayoría trabaja en Monero porque lo disfrutan y lo consideran interesante y estimulante y no porque piensan que van a enriquecerse." - Riccardo Spagni

Como Brandon Goodell, el doctor en matemáticas, quien se reunió a Monero para aumentarlo, Anonimal fue financiado por la comunidad mediante el sistema interno de financiación colectiva. Insinuó en el programa que los dos van a trabajar en Kovri juntos.

Con más de 7,000 XMR recaudados para Anonimal, un colaborador veterano de Monero, puede trabajar en el proyecto a tiempo completo. Spagni mencionó que dos desarrolladores y un investigador han sido financiados de esta manera. "Es bueno porque va a probar que aunque hay muchos fraudes en el espacio cripto, todavía hay un proyecto que es impulsado principalmente por los ideólogos y que tiene una comunidad que está dispuesta a financiar el desarrollo y desarrolladores sin problemas", comentó.

## Kovri es importante no sólo para Monero sino para la privacidad

Kovri no es exclusivo a Monero. Como el sistema independiente, Kovri será útil para todos que necesiten el anonimato, por ejemplo, para informantes o periodistas.

Como explicó Anonimal, "A largo plazo quisiera reducir lo que necesitamos y mejorar lo que ya tenemos. Además, quisiera transformar Kovri en una aplicación del anonimato que sea independiente del sistema en cuanto al uso de API. Mientras que un propósito importante del proyecto es el uso de API en Monero, Kovri podría hacerse la próxima generación de los sistemas del anonimato... Queremos un proyecto que sea útil para todo el mundo así como sea una solución de anonimato a largo plazo para Monero".

Mientras que se usaron XMR para financiar a Anonimal, su trabajo tendrá efectos positivos fuera del ecosistema de Monero.

Kovri ya no tiene la fecha del lanzamiento, sin embargo, es un proyecto emocionante que es anticipado por mucha gente en la comunidad de criptomonedas. Kovri no es valioso sólo para Monero sino es importante en general para la privacidad también. Tendrá una doble función como un enrutador I2P autónomo y el interfaz fácil de usar en la GUI de Monero.

Hablando de la criptografía que se emplea en el proyecto durante el programa, Anonimal expresó su convicción que Kovri es el proyecto más emocionante entre todos para cada criptógrafo:

> "[Kovri] Es como un bufé cripto... Es muy divertido, es el proyecto ideal para unirse porque tenemos muchas cosas en las cuales se puede trabajar y unas ideas excelentes que ya se han desarrollado durante más de una década..."


El texto original está disponible en https://btcmanager.com/what-is-kovri-why-is-it-important-for-monero/. 


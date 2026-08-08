# Criadero Diosesmon

Calculadora de crianza para conseguir Pokémon con los 6 IV a 31, pensada para el servidor de Minecraft **Diosesmon**. Cubre las tres primeras generaciones (386 especies).

La idea es sencilla: apuntas los Pokémon que tienes con sus IV, y la página te dice con quién cruzarlos, qué objeto ponerle a cada padre y qué probabilidad real tienes de sacar el 6×31.

## Qué hace

**Mi Caja** — Añades tus Pokémon con especie, mote, sexo y sus 6 IV. Se agrupan por especie y te marca cuántos IV perfectos lleva cada uno.

**Emparejar** — Eliges dos y te dice si son compatibles, qué especie saldrá de la cría, **qué objeto lleva cada padre** y la probabilidad de 6×31 por huevo. Además genera un ranking automático con las mejores parejas de toda tu caja.

**Buscar Pokémon** — Grupos de huevo de cualquier especie, su ratio de sexo y la lista completa de con quién puede cruzarse.

**Grupos Huevo** — Todas las especies de cada grupo, con sus grupos secundarios.

**Cómo funciona** — Las reglas de crianza explicadas y la tabla de objetos de poder.

## Las reglas que usa

Un Pokémon solo puede llevar **un objeto**. Lo habitual es Lazo Destino en un padre y objeto de poder en el otro.

- **Lazo Destino**: la cría hereda 5 de los 6 IV de los padres, elegidos al azar entre los 12 valores disponibles. El sexto IV sale aleatorio.
- **Objeto de poder**: fija ese stat concreto desde el padre que lo lleva, y cuenta como uno de los 5 que pasa el Lazo.

Consecuencia importante: **siempre queda un IV al azar**. Aunque los dos padres sean 6×31 perfectos y todo esté bien puesto, la probabilidad por huevo es del **3,125%** (1 entre 32). Es el techo matemático, no mala suerte.

| Objeto | Stat que asegura |
|---|---|
| Peso Fuerza | PS |
| Brazal Fuerza | Ataque |
| Cinto Fuerza | Defensa |
| Lente Fuerza | Ataque Especial |
| Banda Fuerza | Defensa Especial |
| Tobillera Fuerza | Velocidad |

Otras reglas contempladas: la cría siempre sale de la especie de **la madre**; Ditto cría con todo menos con otro Ditto y con el grupo Desconocido; los legendarios, los bebés, Nidorina y Nidoqueen no crían; y las formas bebé (Pichu, Azurill, Tyrogue...) se avisan al calcular.

## Uso

Es un único archivo HTML sin dependencias. Funciona sin conexión y sin instalar nada.

Los datos se guardan en el navegador de cada persona, así que cada uno tiene su propia caja. Con los botones **Exportar** e **Importar** puedes hacer copia de seguridad o llevarte la caja a otro equipo.

> Si borras los datos de navegación se pierde la caja. Exporta de vez en cuando.

## Datos

Especies, grupos de huevo y ratios de sexo obtenidos de [PokeAPI](https://pokeapi.co). Se usan los grupos de huevo **actuales**, no los originales de la tercera generación. Hay dos líneas afectadas: Ralts/Kirlia/Gardevoir (hoy Humanoide + Amorfo) y Trapinch/Vibrava/Flygon (hoy Bicho + Dragón).

## Aviso legal

Proyecto de fans sin ánimo de lucro, creado como herramienta de apoyo para la comunidad del servidor Diosesmon. Sin afiliación, patrocinio ni aprobación oficial.

Pokémon es marca registrada de Nintendo, Creatures Inc. y GAME FREAK inc. Todos los derechos sobre la franquicia pertenecen a sus respectivos propietarios. Esta página no incluye ningún recurso gráfico ni sonoro de los juegos.

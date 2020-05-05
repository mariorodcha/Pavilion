# Pavilion
## Introuducción

Pavilion se trata de un videojuego de capturar la bandera por equipos en tres dimensiones. En cada partida, dos equipos se enfrentan para obtener una bandera situada en espacio neutral y llevarla a su base. 
Cada equipo está formado por tres jugadores donde cada uno tendrá un rol específico. Para ello, los personajes podrán pertenecer a tres clases distintas: asalto, especialista y protección. 

## Desarrollo

En esta sección se actualizan todos los elementos del juego desarrollados y testeados. 

### Interfaz:
  - Formularios para iniciar sesión y registrarse
  - Pantalla principal
  - Creación de partidas
  - Seleccion de personaje y mapa
  - HUD en partida del jugador: Actualiza vida y munición
  - HUD en partida para la puntuación de las rondas 
  - Enlace Iniciar Sesión ---- Menú principal
  - Enlace Menú Principal ---- Crear Partida
  - Enlace Crear Partida ---- Lobby (seleccionar mapa y personaje
  - Enlace Lobby ---- Partida
### Personajes
  - Personaje base: Movimiento y carrera, movimiento de cámara, salto, disparo, recarga, coger bandera, soltar bandera, parámetros y muerte.
  - Personaje base: Animaciones de disparo, recarga y muerte.
### Lógica de Partida
  - Asignación de equipos en el lobby
  - Marcador de rondas
  - Bases de ambos equipos en el mapa
  - Spawn de personajes en la base de su equipo y bandera en terreno neutral
  - Reseteo de ronda cuando un equipo gana
### Multijugador en línea
  - Configuración de sesiones online: configurar un server como host y unirse al server como cliente
  - Configuración del lobby: muestra y actualiza la información de los jugadores quue se unen al lobby
  - Lógica para buscar o crear una partida
## Problemas
Los problemas y bugs encontrados por ahora son los siguientes: 

  - Para implementar el multijugador en línea nos hemos respaldado en el subsistema online de Steam disponinble en los plugins de Unreal Engine 4, pero la documentación que hemos seguido es de hace unos años y no hemos conseguido conectar clientes a un server todavía.
  - Los inputs del ratón en la partida nos están dando problemas: para rotar la cámara hay que hacer click y mantener (la idea es que gire al mover el ratón, sin click).
  - Hay un bug temporal en el seleccionar personaje. Cuando seleccionas un personaje, se guarda en el slot y la siguiente vez que lanzas el juego, el personaje seleccionado se mantiene. Cuando se añada el fin de partida en la lógica, ese campo se limpia.
  
## Recursos
  - Para el multijugador en línea:
      - Todos los videos de esta playlist oficial de Unreal Engine 4: https://www.youtube.com/watch?v=abmzWUWxy1U&list=PLZlv_N0_O1gYqSlbGQVKsRg6fpxWndZqZ
      - Todos los videos de esta playlist: https://www.youtube.com/watch?v=qW2XxWPQSlg&list=PLn5SJYtWkakK1SfOdn8_fKMiyy3It4EVU
      - Documentación de Unreal Engine:
          - https://docs.unrealengine.com/en-US/Gameplay/Networking/Blueprints/index.html
          - https://docs.unrealengine.com/en-US/Gameplay/Networking/Actors/index.html
          - https://docs.unrealengine.com/en-US/Gameplay/Networking/Actors/Roles/index.html
      - Libros:
           - Algorithms and Networking for Computer Games - Jouni Smed, Harri Hakonen
           - Networking and Online Games: Understanding and Engineering Multiplayer Internet Games - Grenville Armitage, Mark Claypool, Philip Branch



Introducción actores 
==========

 #### Instalar entorno
Instalar elixir en mac: ```brew install elixir```
(también instala erlang)

 #### Uso de la consola de elixir
 
- Inicializar: ``` iex ```
- Cerrar: Apretar dos veces ``` ctrl + c ```

Para ejecutar el ejemplo y poder crear actores dentro de la consola:

```
elixirc intro_actors.ex
iex
```

 #### Importante

**Spawn** es la primitiva para crear un actor, y se le puede pasar una función que sea un loop que se llame a sí mismo y de acuerdo al mensaje que reciba realizará una acción. Esta es la manera más simple de que un actor quede vivo después de procesar los mensajes que tiene en el mailbox.

El método **receive/1** permite que se pueda buscar el mensaje a partir de su estructura, mediante pattern matching. receive/1 soporta guardas y varias clausulas como case/2, entre otras.

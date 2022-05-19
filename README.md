# 1gigabyte-web-client

# Este es el cliente web de 1gigabyte

### Ejemplos Debug

En la consola de Chrome:

* `bot.chat('test')` Te deja usar el chat
* `bot.chat(JSON.stringify(Object.values(bot.players).map(({username, ping}) => ({username, ping}))))` Da el ping de todos
* `window.bot.entity.position.y += 5` Saltos
* `bot.chat(JSON.stringify(bot.findBlock({matching:(block) => block.name==='diamond_ore', maxDistance:256}).position))` finds the position of a diamond block
* `bot.physics.stepHeight = 2` Te deja ir sobre bloques
* `bot.physics.sprintSpeed = 5` Caminas mas rapido
* `bot.loadPlugin(pathfinder.pathfinder)` then `bot.pathfinder.goto(new pathfinder.goals.GoalXZ(100, 100))` Va a la posicion 100, 100

For more debugging ideas, read the [mineflayer](https://github.com/PrismarineJS/mineflayer) doc.

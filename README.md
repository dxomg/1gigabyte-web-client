# 1gigabyte-web-client

# Este es el cliente web de 1gigabyte

### Some debugging examples

In Chrome DevTools:

* `bot.chat('test')` allows you to use the chat
* `bot.chat(JSON.stringify(Object.values(bot.players).map(({username, ping}) => ({username, ping}))))` display the ping of everyone
* `window.bot.entity.position.y += 5` jumps
* `bot.chat(JSON.stringify(bot.findBlock({matching:(block) => block.name==='diamond_ore', maxDistance:256}).position))` finds the position of a diamond block
* `bot.physics.stepHeight = 2` allows you to walk about blocks
* `bot.physics.sprintSpeed = 5` walks faster
* `bot.loadPlugin(pathfinder.pathfinder)` then `bot.pathfinder.goto(new pathfinder.goals.GoalXZ(100, 100))` goes to position 100, 100

For more debugging ideas, read the [mineflayer](https://github.com/PrismarineJS/mineflayer) doc.

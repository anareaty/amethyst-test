<%*
let commands = app.commands.commands
let keys = Object.keys(commands)

let result = ""
keys.forEach(key => {
result = result + "- " + commands[key].name + " — \"" + commands[key].id + "\"\n"
})

%><%* tR += result %>
<%*
const ts = tp.date.now("YYYYMMDDHHmmss")
const title = await tp.system.prompt("Short slug?")
await tp.file.rename(`${ts}-${title}`)
%>

# <% tp.file.title %>
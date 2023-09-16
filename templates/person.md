---
type: 
name:
sex: 
race: 
height: 
weight: 
alignment: 
location: 
factions:
---

<% tp.file.title %>
<% await tp.file.move("/World/People/PCs/" + tp.file.title) %>


<%*
const hasTitle = !tp.file.title.startsWith("NewNPC");
let title;
if (!hasTitle) {
    title = await tp.system.prompt("Enter NPC Name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>


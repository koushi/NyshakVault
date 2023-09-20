---
type: 
name: 
sex: 
connections: 
race: 
alignment: 
location: 
age: 
class: 
languages: 
factions: 
subclass:
---
<%*
const hasTitle = !tp.file.title.startsWith("Untitled");
let title;
if (!hasTitle) {
    title = await tp.system.prompt("Enter NPC Name");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>

<% tp.file.title %>
<% await tp.file.move("/World/People/PCs/" + tp.file.title) %>

> [!infobox]
> # `=this.file.name`
> ![[z_Assets/Misc/ImagePlaceholder.png|cover hsmall]]
> [[z_Assets/Misc/ImagePlaceholder.png|Show To Players]]
> ###### Basic Information
> Type |  Stat |
> ---|---|
> Home | `=this.location` |
> Group | `=this.faction` |
> Sex | `=this.sex` |
> Race | `=this.race` |
> Age | `=this.age` |
> Condition | `=this.factions` |
> ###### Rules Info
> Type |  Stat |
> ---|---|
> Alignment | `=this.alignment` |
> Class | `=this.class` |
> Sub Class | `=this.subclass` |

# `=this.file.name`
> [!column|clean no-title] 
>> [!example|bg-c-black ]- Column 1 
>> Use another callout for columns 
>
>> [!note|clean no-title] Column 2 



## Profile

**<Add description here, extend it with AI Text Generator using Ctrl J>**



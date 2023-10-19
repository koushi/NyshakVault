---
type: 
name: 
sex: 
connections: 
race: 
alignment: 
location: 
age: 
languages: 
factions: 
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

<% await tp.file.move("/World/People/Entities/" + tp.file.title) %>

> [!infobox]
> # `=this.file.name`
> ![[z_Assets/Misc/ImagePlaceholder.png|cover hsmall]]
> [[z_Assets/Misc/ImagePlaceholder.png|Show To Players]]
> ###### Basic Information
>  |  |
> ---|---|
> Sex | `=this.sex` |
> Race | `=this.race` |
> Age | `=this.age` |
> Languages | `=this.languages` |
> Home | `=this.location` |
> Group | `=this.factions` |
> Alignment | `=this.alignment` |

# `=this.file.name`
`=this.name` is a `=this.sex` `=this.race` `=this.subclass` `=this.class`. 
> [!column|clean no-title] 
>> [!abstract|c-red ]- Contents
>> 1. [[#Description]]
>> 	- [[#Appearance]]
>> 	- [[#Personality]]
>> 2. [[#Biography]]
>> 	- [[#Background]]
>> 	- [[#Campaign]]
>
>> [!note|clean no-title] Column 2 



## Description
### Appearance
### Personality
## Biography
### Background
### Campaign
## Relationships





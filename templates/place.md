---
type: 
name: 
nickname:
builtdate:
leader:
plane:
region:
districts:
population:
affiliation:
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
<% await tp.file.move("/World/Places/" + tp.file.title) %>

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
> ###### Rules Info
>  |   |
> ---|---|
> Alignment | `=this.alignment` |
> Class | `=this.class` |
> Sub Class | `=this.subclass` |
> ###### Stats
>  | | |
> ---|---|---|
> HP | AC | DC |
> `=this.HP` | `=this.AC` | `=this.DC` |
> Str | Dex | Con |
> `=this.str` | `=this.dex` | `=this.con` |
> Int | Wis | Cha |
> `=this.int` | `=this.wis` | `=this.cha`|

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




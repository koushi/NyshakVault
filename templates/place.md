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
> ###### General Information
>  |  |
> ---|---|
> Name | `=this.name` |
> Nickname | `=this.nickname` |
> Built | `=this.builtdate` |
> Leader | `=this.leader` |
> ###### Location Information
>  |   |
> ---|---|
> Plane | `=this.plane` |
> Region | `=this.region` |
> Districts | `=this.districts` |
> ###### Societial Information
>  |   |
> ---|---|
> Population | `=this.plane` |
> Affiliation | `=this.affiliation` |

# `=this.file.name`
`=this.name` is a `=this.sex` `=this.race` `=this.subclass` `=this.class`. 
> [!column|clean no-title] 
>> [!abstract|c-red ]- Contents
>> 1. [[#Description]]
>> 2. [[#Map]]
>> 3. [[#History]]
>> 4. [[#Society]]
>
>> [!note|clean no-title] Column 2 



## Description
## Map
### Background
### Campaign
## History
## Society
### Demographics
### Notable People




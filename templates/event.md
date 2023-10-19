---
type:
name:
location: 
year:
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

<% await tp.file.move("/World/Events/" + tp.file.title) %>


# `=this.file.name`

> [!column|clean no-title] 
>> [!abstract|c-red ]- Contents
>> 1. [[#Description]]
>> 2. [[#Details]]
>
>> [!note|clean no-title] Column 2 



## Description
## Details
### Background




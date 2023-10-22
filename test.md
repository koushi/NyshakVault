---
type: 
date: 
location:
---
<%*
const hasTitle = !tp.file.title.startsWith("Untitled");
let title;
if (!hasTitle) {
    title = tp.date.now(format: string = "dddd, MMMM Do YYYY");
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>

<% await tp.file.move("/World/Sessions/" + tp.file.title) %>

#  `=this.file.title`
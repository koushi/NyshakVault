---
type: 
date: 
location:
---
<%*
const hasTitle = !tp.file.title.startsWith("Untitled");
let title;
if (!hasTitle) {
    title = tp.date;
    await tp.file.rename(title);
} else {
    title = tp.file.title;
}
_%>

<% await tp.file.move("/World/Places/" + tp.file.title) %>
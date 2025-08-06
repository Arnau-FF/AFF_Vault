<%*
// V1.2
let variable_name = await tp.system.prompt("Note Title");  
// if title not null
if (variable_name) {
  let parent = tp.config.active_file.basename; // Parent name
 
  let parentPath = tp.file.path(true); // Parent Path
  let dir = parentPath.slice(0, parentPath.length - parent.length - 4);// remove: /parent.md characters from path
  let path = "/"+dir+"/Notes/"+variable_name; // New Note Path
 
  let time = "yyyy.MM.dd - HH:mm";
  let escaped_time = "\"" + time + "\""; // escaped allows to add"" as part of string
  let char = ""
  let escapedchar = "\"" + char + "\""


  let new_file_content ="\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1.2\n>Creation:: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified::  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+parent+"]]\n> #Notes\n```button\nname +\ntype command\naction Templater: Insert Templates/Notes/MOC5/Template_New_Child.md\n\n```\n>[!Multi-Column]\n>>[!Children] Children \n>>```dataview\n>>LIST \n>>FROM "+escapedchar+" \n>>WHERE parent = [[]] and file.name != this.file.name\n>>```\n>\n>>[!mentioned] Mentioned On:\n>>```dataview\n>>List \n>>from [[]]\n>>Where Parent != [[]] and file.name != this.file.name\n>>```\n>>\n\nSources :: \n***\n# Body:\n\n\n\n\n\n\n\n\n\n\n\n" 

; // New Note contents
  
  // Create and move note
  let new_file = await tp.file.create_new(new_file_content, variable_name);
  //await tp.file.move(path);
  // Open note
  await sleep(100)
  await app.workspace.openLinkText(variable_name, path);
  }


%>
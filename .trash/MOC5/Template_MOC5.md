<%*  
// V2
let variable_name = await tp.system.prompt("Note Title");  

  let parent = tp.config.active_file.basename; // Parent name
  let parentPath = tp.file.path(true); // Parent Path
  let dir = parentPath.slice(0, parentPath.length - parent.length - 4);// remove: /parent.md characters from path
  let path = "/"+dir+"/"+variable_name+"/"+variable_name; // New Note Path
  let time = "yyyy.MM.dd - HH:mm";
  let escaped_time = "\"" + time + "\""; // escaped allows to add"" as part of string


// New Note contents MOC5
  let new_file_content ="# `= this.file.link`\n>[!Properties]- | `= this.Parent.Parent.Parent.Parent` |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` | `BUTTON[note]`\n>Version:: 2\n>Parent:: [["+parent+"]]\n>Tags: #Notes #MOC/5\n```meta-bind-embed\n[[Search Moc5]]\n```\nSource::\nRelated to::\n***\n# Body:\n\n\n\n\n\n\n\n\n\n# Foot\n```meta-bind-embed\n[[Foot MOC5]]\n```" ; 

//Create Moc5 Notes
if (variable_name) {   // Notes

  // Create and move note
  let new_file = await tp.file.create_new(new_file_content, variable_name);
//  await sleep(500)
  await tp.file.move(path);
 // await sleep(500)
  // open note
  await app.workspace.openLinkText(variable_name, path);
}
	
%>
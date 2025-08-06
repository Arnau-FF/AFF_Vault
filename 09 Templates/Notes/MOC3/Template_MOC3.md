<%*  
// V3.0

// Add Title
let variable_name = await tp.system.prompt("Note Title");  

// if title not null
if (variable_name) {
  let parent = tp.config.active_file.basename; // Parent name
  let parentPath = tp.file.path(true); // Parent Path
  let dir = parentPath.slice(0, parentPath.length - parent.length - 4);// remove: /parent.md characters from path
  let folder = "/"+dir+"/"+variable_name; // New Folder Path
  let path = "/"+dir+"/"+variable_name+"/"+variable_name; // New Note Path
  

// Note contents 
  let new_file_content ="# `= this.file.link`\n>[!Properties]- | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` | `BUTTON[note]` \n>Version:: 3\n>Parent:: [["+parent+"]]\n>Tags: #MOC/3\n```meta-bind-embed\n[[Search Moc3]]\n```\n# Body:\n\n\n\n\n\n\n\n\n\n# Foot\n```meta-bind-embed\n[[Foot MOC3]]\n```" ; 

// Create and move note
  let new_file = await tp.file.create_new(new_file_content, variable_name,false,folder);
  
// open note
  await app.workspace.openLinkText(variable_name, path);
}
	
%>
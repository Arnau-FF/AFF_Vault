<%*  
//v3.0 

// Add Title
let variable_name = await tp.system.prompt("Note Title"); 

// if title not null
if (variable_name) {
  let folder = "00 Notes"+ "/"+variable_name; // Folder Path

// Note contents
  let new_file_content = "# `= this.file.link` \n>[!Properties]- | `= this.Parent` | `= this.file.link` | `BUTTON[moc3]`\n>Version:: 3.0\n>Parent:: [[Dashboard]]\n> Tags: #MOC/2\n```meta-bind-embed\n[[Search Moc2]]\n```\n\n\n\n\n\n\n\n# Foot\n```meta-bind-embed\n[[Foot MOC2]]\n```" ; 
  

// Create and move note
  let new_file = await tp.file.create_new(new_file_content, variable_name,true,folder);
  
  }



%>
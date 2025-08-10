<%*  
// V3

//Add Title
let variable_name = await tp.system.prompt("Note Title");  

// if Title not null
if (variable_name) {
  let parent = tp.config.active_file.basename; // Parent name
  let parentPath = tp.file.path(true); // Parent Path
  let dir = parentPath.slice(0, parentPath.length - parent.length - 4);// remove: /parent.md characters from path
  let path = "/"+dir+"/Notes/"+variable_name; // New Note Path
 
// YAML frontmatter with Type: Note 
  let yaml = `---\nType: Note\n---\n`;
  
// New Note contents
  let new_file_content =""+yaml+"# `= this.file.link`\n>[!Properties]- |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` | `BUTTON[note]` \n>Version:: 3\n>Parent:: [["+parent+"]]\n>Tags:\n```meta-bind-embed\n[[Search note]]\n```\nSource::\nRelated To::\n***\n# Body:\n\n\n\n\n\n\n\n\n\n# Foot\n```meta-bind-embed\n[[Foot note]]\n``` " ;

 // Create and move note
  let new_file = await tp.file.create_new(new_file_content, variable_name,false);

// wait Mili seconds, avoid not having parent displayed properly
    await sleep(01)
    
// open note ( File.create_new argument open note dosent work, not update properly)
  await app.workspace.openLinkText(variable_name, path);
  }



%>
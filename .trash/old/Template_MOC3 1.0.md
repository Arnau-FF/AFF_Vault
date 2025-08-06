<%*  
// Add Title
let variable_name = await tp.system.prompt("Note Title");  
// if title not null
if (variable_name) {
  let parent = tp.config.active_file.basename; // Parent name
  let Folder = "Notes"+ "/"+variable_name; // New Note Path
  let path = "Notes"+ "/"+variable_name+"/"+variable_name; // New Note Path


  let time = "yyyy.MM.dd - HH:mm";
  let escaped_time = "\"" + time + "\""; // escaped allows to add"" as part of string
  let char = "MOC/4"
  let escapedchar = "\"" + char + "\""
  let char1 = "MOC/5"
  let escapedchar1 = "\"" + char1 + "\""
  let char2 = "#MOC/5"
  let escapedchar2 = "\"" + char2 + "\""

  let new_file_content = "\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1\n>Creation: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified:  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+parent+"]]\n\n#Notes #MOC/3\n___\n# Content:\n```button\nname +\ntype command\naction Templater: Insert Templates/Notes/MOC4/Template_MOC4.md\ncolor default\n```\n```dataview\nTABLE WITHOUT ID \nfile.link as "+escapedchar+",\nfilter(file.inlinks, (x)=> contains(x.file.tags, "+escapedchar2+")) as Notes \n\nFrom   #MOC/4 and #Notes  and !#template\nWHERE contains(file.outlinks, this.file.link)\nSort ascending\n```" ; // New Note contents
  

  // Create Folder if not exist
  if (!tp.file.exists(Folder)) {
  await this.app.vault.createFolder(Folder)
}
  // Create and move note
  let new_file = await tp.file.create_new(new_file_content, variable_name);
  await tp.file.move(path);
  
  // open note
  await app.workspace.openLinkText(variable_name, path);
  }



%>
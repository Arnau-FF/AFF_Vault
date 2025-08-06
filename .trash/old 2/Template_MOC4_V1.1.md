<%*  
// V1
let variable_name = await tp.system.prompt("Note Title");  

  let parent = tp.config.active_file.basename; // Parent name
  let parentPath = tp.file.path(true); // Parent Path
  let dir = parentPath.slice(0, parentPath.length - parent.length - 4);// remove: /parent.md characters from path
  let path = "/"+dir+"/"+variable_name+"/"+variable_name; // New Note Path
  let time = "yyyy.MM.dd - HH:mm";
  let escaped_time = "\"" + time + "\""; // escaped allows to add"" as part of string

// other notes
  let variable_name1 = variable_name+ "_Notes";
  let path1 = "/"+dir+"/"+variable_name+"/Notes/"+variable_name1;
  let variable_name2 = variable_name+ "_Projects";
  let path2 = "/"+dir+"/"+variable_name+"/Notes/"+variable_name2;
  let variable_name3 = variable_name+ "_Resourses";
  let path3 = "/"+dir+"/"+variable_name+"/Notes/"+variable_name3;
  let variable_name4 = variable_name+ "_Key";
  let path4 = "/"+dir+"/"+variable_name+"/Notes/"+variable_name4;
  let variable_name5 = variable_name+ "_Archive";
  let path5 = "/"+dir+"/"+variable_name+"/Notes/"+variable_name5;

// New Note contents MOC4
  let new_file_content ="\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1.1\n>Creation:: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified::  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+parent+"]]\n> #Notes #MOC/4\n___\n```button\nname +\ntype command\naction Templater: Insert Templates/Notes/MOC5/Template_First_Child.md\n\n```\n>[!Multi-Column]\n>>[!Notes] Notes\n>>```dataview\n>>list\n>>From  [[]] and !#template and #Notes and !#Project and !#Resourse and !#Archive and !#Key\n>>\n>>```\n>\n>>[!Project] Projects\n>>```dataview\n>>list\n>>From   [[]]  and !#template and #Notes and #Project \n>>\n>>```\n>\n>>[!Key] Key\n>>```dataview\n>>list\n>>From   [[]]  and !#template and #Notes  and #Key\n>>\n>>```\n\n>[!Archive]- Archive\n>```dataview\n>list\n>From   [[]]  and !#template and #Notes and #Archive \n>```\n\n# Summary:" ; 

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
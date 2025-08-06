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
  let new_file_content ="\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1\n>Creation: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified:  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+parent+"]]\n\n#Notes #MOC/4\n___\n```button\nname +\ntype command\naction Templater: Insert Templates/Notes/MOC5/Template_First_Child.md\n\n```\n>[!Multi-Column]\n>>[!Notes] [["+variable_name1+"|Notes]]\n>>```dataview\n>>list\n>>From  [[]] and !#MOC/5 and !#template and #Notes and !#Project and !#Resourse and !#Archive and !#Key\n>>\n>>```\n>\n>>[!Resourses] [["+variable_name3+"|Resourses]]\n>>```dataview\n>>list\n>>From   [[]] and !#MOC/5 and !#template and #Notes and #Resourse\n>>\n>>```\n>\n>>[!Project] [["+variable_name2+"|Projects]]\n>>```dataview\n>>list\n>>From   [[]] and !#MOC/5 and !#template and #Notes and #Project \n>>\n>>```\n>\n>>[!Key] [["+variable_name4+"|Key]]\n>>```dataview\n>>list\n>>From   [[]] and !#MOC/5 and !#template and #Notes  and #Key\n>>\n>>```\n>\n>>[!Archive] [["+variable_name5+"|Archive]]\n>>```dataview\n>>list\n>>From   [[]] and !#MOC/5 and !#template and #Notes and #Archive \n>>\n>>```\n\n# Summary:" ; 

// Notes
  let new_file_content1= "\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1\n>Creation: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified:  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+variable_name+"]]\n\n#Notes #MOC/5\n___\n>[!Multi-Column]\n>>[!Notes]\n>>```dataview\n>>list\n>>From   !#MOC/5 and !#moc/4 and !#template and #Notes and !#Project and !#Resourse and !#Archive and !#Key\n>>WHERE contains(parent, this.parent) and file.name != this.file.name\n>>```\n" ; 


// Project
  let new_file_content2= "\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1\n>Creation: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified:  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+variable_name+"]]\n\n#Notes #MOC/5\n___\n>[!Multi-Column]\n>>[!Notes]\n>>```dataview\n>>list\n>>From   !#MOC/5 and !#moc/4 and !#template and #Notes and !#Project and !#Resourse and !#Archive and !#Key\n>>WHERE contains(parent, this.parent) and file.name != this.file.name\n>>```\n" ; 

// Resourses
  let new_file_content3= "\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1\n>Creation: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified:  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+variable_name+"]]\n\n#Notes #MOC/5\n___\n>[!Multi-Column]\n>>[!Notes]\n>>```dataview\n>>list\n>>From   !#MOC/5 and !#moc/4 and !#template and #Notes and !#Project and !#Resourse and !#Archive and !#Key\n>>WHERE contains(parent, this.parent) and file.name != this.file.name\n>>```\n" ; 
// Key
  let new_file_content4= "\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1\n>Creation: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified:  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+variable_name+"]]\n\n#Notes #MOC/5\n___\n>[!Multi-Column]\n>>[!Notes]\n>>```dataview\n>>list\n>>From   !#MOC/5 and !#moc/4 and !#template and #Notes and !#Project and !#Resourse and !#Archive and !#Key\n>>WHERE contains(parent, this.parent) and file.name != this.file.name\n>>```\n" ; 
// Archive

 let new_file_content5= "\n>[!Properties]- `$= dv.current().Parent` \n>Version:: 1\n>Creation: `=dateformat(this.file.ctime,"+escaped_time+" )`\n>Last modified:  `=dateformat(this.file.mtime, "+escaped_time+")`\n>Parent:: [["+variable_name+"]]\n\n#Notes #MOC/5\n___\n>[!Multi-Column]\n>>[!Notes]\n>>```dataview\n>>list\n>>From   !#MOC/5 and !#moc/4 and !#template and #Notes and !#Project and !#Resourse and !#Archive and !#Key\n>>WHERE contains(parent, this.parent) and file.name != this.file.name\n>>```\n" ; 
  
//Create Moc5 Notes
if (variable_name) {   // Notes
	
	
	let new_file1 = await tp.file.create_new(new_file_content1, variable_name1);
	await sleep(500)
	await tp.file.move(path1);
	await sleep(500)
	
	let new_file2 = await tp.file.create_new(new_file_content2, variable_name2);
	await sleep(500)
	await tp.file.move(path2);
	await sleep(500)

	let new_file3 = await tp.file.create_new(new_file_content3, variable_name3);
	await sleep(500)
	await tp.file.move(path3);
	await sleep(500)
	
	let new_file4 = await tp.file.create_new(new_file_content4, variable_name4);
	await sleep(500)
	await tp.file.move(path4);
	await sleep(500)
	
	let new_file5 = await tp.file.create_new(new_file_content5, variable_name5);
	await sleep(500)
	await tp.file.move(path5);
  await sleep(500)
  // Create and move note
  let new_file = await tp.file.create_new(new_file_content, variable_name);
  await sleep(500)
  await tp.file.move(path);
  await sleep(500)
  // open note
  await app.workspace.openLinkText(variable_name, path);
}
	
%>
---
Type: Note
sub-type: 
---
# `= this.file.link`
>[!Properties]- |  `= this.Parent.Parent.Parent` | `= this.Parent.Parent` | `= this.Parent` | `= this.file.link` | `BUTTON[note]` 
>Version:: 3
>Parent:: [[Plugins]]
>Tags:
```meta-bind-embed
[[Search note]]
```
Source:: [GIT](obsidian://show-plugin?id=obsidian-git)
Related To::
***
# Set UP:

[Start here - Git Documentation - Obsidian Publish](https://publish.obsidian.md/git-doc/Start+here)
1. Install Software GIT
2. Install Github Desktop ( Optional)
3. Install git Plugging ➔ Auto sync 5 minutes

## How to recover deleted File.
[Recovering Deleted Files in GitHub](https://rewind.com/blog/recovering-deleted-files-in-github/#:~:text=If%20you%20have%20not%20staged,exist%20in%20the%20index%20anymore.)

# Backup
## Ignore File
Vault directory ➔ Create file .gitignore.txt
```
.obsidian/workspace.json
<<<<<<< HEAD
=======
.obsidian/workspace.json
.obsidian/workspace-mobile.json
.trash/
.DS_Store
>>>>>>> origin/main
```
### If file was previously synced 

It needs to stop to be tracked if not it will not work.

**Open CMD :**
*  Navigate to Project Folder
```
cd C:\Users\xxx\Documents\Obsidian_Vault
```
*  Run Git Commands
```
git rm --cached .obsidian/workspace.json
git commit -m "Stop tracking .obsidian/workspace.json"
```
*  Initialize
```
git init
```






# Foot
```meta-bind-embed
[[Foot note]]
``` 
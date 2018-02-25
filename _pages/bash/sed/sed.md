---
layout: default
---
#### Substitution of Characters

Example lowecase y to UpperCase Y --> to new File

g - flag indicates the substitution

  ```sh
  sed 's/term/replacement/flag/' file

  sed '/s/y/Y/g' child1.txt > child2.txt
  ```

If you want to search or replace a special character (such as /, \, &) 

you need to escape it, in the term or replacement strings, with a backward slash.

 ```sh
 sed 's/and/\&/g;s/^I/You/g' ahappychild.txt 
 ```

Another use of sed is showing (or deleting) a chosen portion of a file.
In the following example, we will display the first 5 lines of /var/log/messages from Jun 8.
 ```sh
 sed -n '/^Jan 8/ p' /var/log/massages | sed -n 1,5p
 ```

Finally, it can be useful while inspecting scripts or configuration files to inspect the code itself and leave out comments. The following sed one-liner deletes (d) blank lines or those starting with # (the | character indicates a boolean OR between the two regular expressions).
 ```sh
 sed '/^#\|^$/d' apache2.conf
 ```

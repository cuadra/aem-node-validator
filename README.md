# NodeFresh - AEM Node Validator
Prepares AEM node lists for replication by normalizing paths and removing invalid entries.

<img width="1012" height="494" alt="image" src="https://github.com/user-attachments/assets/591f3271-83f1-420f-91aa-3e24fc0c29ee" />

## Interface
<img width="1432" height="1316" alt="image" src="https://github.com/user-attachments/assets/8a5b03b3-2220-4056-ac59-070ff2d21a71" />

## Rules
Coming soon...
## Example
```
sfdsdf 
Include this file
/content/division/brand/locale/folder/file.html
content/division/brand/locale/otherfolder/file.html
/* Hold on these */
/content/division/brand/locale/folder/file.html
//becomes
/content/dam/division/brand/locale/folder/file.css
12122345 234
{(s<w
content/division/otherbrand/locale/folder/file.html
/dam/division/brand/locale/folder/file.jpg
```
is transformed to:
```
/content/division/brand/locale/folder/file/jcr:content
/content/division/brand/locale/otherfolder/file/jcr:content
/content/division/brand/locale/folder/file/jcr:content
/content/dam/division/brand/locale/folder/file.css
/content/division/otherbrand/locale/folder/file/jcr:content
/content/dam/division/brand/locale/folder/file.jpg
```

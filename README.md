# sbviewer

**What's this?** 
A viewer for [Starboard](https://starboard.gg/) files hosted on github/gist, in the spirit of nbviewer for jupyter files. 

**How to use it?** 
Just open/share 
https://bmacho.github.io/sbviewer/?sb=PATH
type links. 

 - For notebooks hosted on gist, the syntax is
https://bmacho.github.io/sbviewer/?sb=gist/USER/GISTNUMBER/?revision/?file 
where both revision and file name are optional. If there are multiple files in a gist, it will open the first one.
- For notebooks hosted on github, the syntax is 
https://bmacho.github.io/sbviewer/?sb=github/USER/REPO/BLOB/BRANCHorCOMMIT/FILEPATH 
e.g.: 
- You also can use any other URL that your browser can get, http urls, or relative paths. 
e.g.:  https://bmacho.github.io/sbviewer/?sb=index.sb  should open index.sb in the same folder. You can download the index.html file, and place in your repo. 

### License 
It's a very slightly modification of starboard-notebook, both the original, and all of my modification is licensed under MPL2. 

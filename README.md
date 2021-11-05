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
  - https://bmacho.github.io/sbviewer/?sb=gist/bmacho/67188d770d96b050ea329991b3cbe898/procedural-art.sb
  - https://bmacho.github.io/sbviewer/?sb=gist/bmacho/67188d770d96b050ea329991b3cbe898/e9a4c960b371ac3136b9afc7765abf51565f868c/README.md
- For notebooks hosted on github, the syntax is 
https://bmacho.github.io/sbviewer/?sb=github/USER/REPO/BLOB/BRANCHorCOMMIT/FILEPATH e.g.: 
  - https://bmacho.github.io/sbviewer/?sb=github/bmacho/sbviewer/blob/main/README.md
  - https://bmacho.github.io/sbviewer/?sb=github/bmacho/sbviewer/blob/09be7302b55262066ac9fb8bb05332133be69af6/README.md

- You also can use any other URL that your browser can get, http urls, or relative paths. e.g.:  
  - https://bmacho.github.io/sbviewer/?sb=index.sb
should open index.sb in the same folder, if you host the index.html file in a local folder (needs a webserver bc of CORS), or on an own website.   

### License 
It's a very slightly modification of starboard-notebook, both the original, and all of my modification is licensed under MPL2. 

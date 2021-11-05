# sbviewer

**What's this?** 
A viewer for [Starboard](https://starboard.gg/) files hosted on github/gist, in the spirit of [nbviewer](https://nbviewer.org/) for jupyter files. 

**How to use it?** 
Just open/share 
https://bmacho.github.io/sbviewer/?sb=PATH
type links. 

- For notebooks hosted on gist, the syntax is
https://bmacho.github.io/sbviewer/?sb=gist/USER/GISTNUMBER/?revision/?file 
where both revision and file name are optional. If there are multiple files in a gist, it will open the first one. E.g. for the gist https://gist.github.com/bmacho/67188d770d96b050ea329991b3cbe898/ you can do 
  - https://bmacho.github.io/sbviewer/?sb=gist/bmacho/67188d770d96b050ea329991b3cbe898/procedural-art.sb or
  - https://bmacho.github.io/sbviewer/?sb=gist/bmacho/67188d770d96b050ea329991b3cbe898/e9a4c960b371ac3136b9afc7765abf51565f868c/README.md
- For notebooks hosted on github, the syntax is 
https://bmacho.github.io/sbviewer/?sb=github/USER/REPO/BLOB/BRANCHorCOMMIT/FILEPATH e.g. in this repo : 
  - https://bmacho.github.io/sbviewer/?sb=github/bmacho/sbviewer/blob/main/README.md
  - https://bmacho.github.io/sbviewer/?sb=github/bmacho/sbviewer/blob/09be7302b55262066ac9fb8bb05332133be69af6/README.md

- You also can use any other URL that your browser can get, http urls, or relative paths. e.g.:  
  - https://bmacho.github.io/sbviewer/?sb=index.sb
should open index.sb in the same folder, if you host the index.html file in a local folder (needs a webserver bc of CORS), or on an own website.   

**Features/automatisms**
- If the file extension is md/js, it creates a markdown/javascript cell. (Does not recognise the file type, if there is no extension.)
- Trims down trailing newline characters from the last cell, because my text editor attaches to the ends of files, and it looks ugly when opened. 
- If no sb source given, it defaults to index.sb
- 404 notebook: https://bmacho.github.io/sbviewer/?sb=VALID_NOTEBOOK_NAME_BUT_NOT_REACHABLE

### License 
It's a very slightly modification of starboard-notebook, both the original, and all of my modification is licensed under MPL2. 

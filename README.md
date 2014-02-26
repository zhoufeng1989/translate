translate
=========

translate command tools baseed on google translate   

**usage**:

usage: translate [-h] [-sl SOURCE LANGUAGE] [-tl TARGET LANGUAGE] [-r]      
                 text [text ...]

translate use translate.google.com

positional arguments:     
  text                  text to be translated

optional arguments:          
  -h, --help            show this help message and exit    
  -sl SOURCE LANGUAGE, --source language SOURCE LANGUAGE   
                        translate from the source language   
  -tl TARGET LANGUAGE, --target language TARGET LANGUAGE   
                        translate to the target language   
  -r, --reverse         change target language to en, useful when from zh-CN


**install**:
```bash
wget https://raw.github.com/zhoufeng1989/translate/master/translate
chmod u+x translate
# move it wherever in your PATH
mv translate /bin/
```


**example**:
```bash
translate python
=>蟒蛇
# multiple words
translate very good
=>很
=>好
# from zh-CN to en
translate -r 中国
=>china
```

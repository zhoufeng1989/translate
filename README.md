translate
=========

translate command tools baseed on google translate   

**usage**:    
    **translate [-h] [-sl SOURCE LANGUAGE] [-tl TARGET LANGUAGE] [-r] text [text ...]**

translate use translate.google.com

positional arguments:     
+   **text**   
    text to be translated

optional arguments:          
+   **-h, --help**     
    show help messages and exit    
+   **-sl SOURCE LANGUAGE, --source language SOURCE LANGUAGE**   
    translate from the source language   
+   **-tl TARGET LANGUAGE, --target language TARGET LANGUAGE**   
    translate to the target language   
+   **-r, --reverse**         
    change target language to en, useful when translate from zh-CN


**install in *nix**:
```bash
wget --no-check-certificate https://raw.github.com/zhoufeng1989/translate/master/translate
chmod u+x translate
# move it wherever in your PATH
mv translate /bin/
```


**examples**:
```bash
translate python
=>蟒蛇
# multiple words
translate very good
=>很
=>好
# translate phrase
translate 'come on'
=>来吧
# from zh-CN to en
translate -r 中国
=>china
```

**dependencies**:
+   [requests](https://github.com/kennethreitz/requests)
+   [python](http://python.org/) above 2.7

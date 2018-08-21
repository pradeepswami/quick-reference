# Markdown quick reference

### Head text using structure enhanced text  
```
=== First level  
--- Second level  
```
Header1 text
===
Header2 text
----

### Header text using ATX  
```
# First level  
## Second level  
### Third level  
...  
###### Sixth level  
```
# Header1 text
## Header2 text  
### Header3 text
...
###### Header6 text

### Horizontal rules (html hr tag)
```
---  
***  
___
```

____

### Block quote
```
> Level1  
>> Level2
```

> Level1
>> Level2



### Italicize
```
*world*  
_world_  
```

Hello *world*

### Bold
```
**world**  
__world__  
```
Hello __world__



### Unordered list
```
*  
+  
-  
```

+ Item1
+ Item2
+ Item3

### Ordered list
```
1.
2.
3.
```
1. Item1
2. Item2
3. Item3

### Inline link
```
[ Text ]( url " Title " )
```

The [BBC](https://www.bbc.co.uk/ "BBC title") is a British public service broadcaster

### Inline link image  

```
![ Text ]( url " Title " )  
```
![Linux](https://upload.wikimedia.org/wikipedia/commons/thumb/3/35/Tux.svg/280px-Tux.svg.png "Linux")

### Reference link  
```
[ Text ][ Ref link ]  

Reference link declaration  [ Ref link ]: url
```

The [BBC][bbclink] is a British public service broadcaster
[bbclink]:https://www.bbc.co.uk/

### Reference image link  
```
![ Text ][ img link ]  
Reference link declaration  [ img link ]: url  
```

![Linux][lx1]  
[lx1]:https://upload.wikimedia.org/wikipedia/commons/thumb/3/35/Tux.svg/280px-Tux.svg.png

### Inline url link
 < url \>  
 Go to <https://wwww.google.com>


### Inline code
\` < html element>\`  Content between back tick will be placed with html `<code>` element  
Example text with inline code  `<input type="text" name="test" >`  , ` var amount = 12;`



### Code block
Four space or 1 tab  

    var amount = 100;
    function add( a, b){
      return a + b;
    }

### Code block - Github flavor

\`\`\` lanuge ...code... \`\`\`

```html
   <input type="text" name="test">
```   

### Anchor tag - Github flavor

Github adds anchor tag for all head elements.  
\[ Link name \]\( #headername \)

### Table - Github flavor  
```
| Column1 | Column2 |
|---------|---------|
|  value1 | value2  |
```
| Column1 | Column2 |
|---------|---------|
|  value1 | value2  |

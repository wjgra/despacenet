# despacenet
Copy the below code to a bookmark, then click the bookmark when on a new Espacenet page to be transported back to the corresponding classic Espacenet page! This should work as long as classic Espacenet is kept online 'for a little while longer', though bookmarklets are a dying breed too so this may not have terribly much longevity.
```
javascript:currenturl = window.location.href;index = currenturl.search("worldwide.espacenet.com/patent/search/");if (index == -1){alert("This only works on new Espacenet document pages!");}else{index = currenturl.search("/publication/");currenturl = currenturl.substring(index+13);temp = currenturl.split("?");window.location.href = "https://worldwide.espacenet.com/publicationDetails/biblio?ND=3&locale=en_EP&FT=D&CC="+temp[0].substring(0,2)+"&NR="+temp[0].substring(2);}
```
N.B. At least on Edge/Chrome, this only seems to work when the bookmark is accessed via the bookmark bar.
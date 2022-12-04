# despacenet
Escape new Espacenet with this bookmarklet
'''
javascript:currenturl = window.location.href;index = currenturl.search("worldwide.espacenet.com/patent/search/");if (index == -1){alert("This only works on new Espacenet document pages!");}else{index = currenturl.search("/publication/");currenturl = currenturl.substring(index+13);temp = currenturl.split("?");window.location.href = "https://worldwide.espacenet.com/publicationDetails/biblio?ND=3&locale=en_EP&FT=D&CC="+temp[0].substring(0,2)+"&NR="+temp[0].substring(2);}
'''
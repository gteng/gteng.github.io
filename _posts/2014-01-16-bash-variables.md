---
layout: post
title: Bash Variables Tips
---

{{ page.title }}
================
#bash variables
1. general assignment value to variable  
var=12  
var=string  
var=(a b c )  
array[index]=value  
${array[*]}  
${array[index]}  
${array[@]}  
unset var  
unset array[index]  
unset array  

2. declare  
syntax: declare OPTION(s) VARIABLE=value  
options: i(int),a(array),f(function),p(dispaly),r(read-only),t(trace),x(export)

3. length of variable  
${#var}  

4. substitution  
${var-word}  
${var=word}  
${var+word}  

5. substring  
${var:offset:length}  

6. head trim  
${var#pattern}  
${var##pattern}  

7. tail trim  
${var%pattern}  
${var%%pattern}  

8. replace pattern  
${var/pattern/string}  
${var//pattern/string}

# BASH basics
**[Bash memo link](https://devhints.io/bash)** 

#!/bin/bash/

---

*Declaration*
>No space after '=', use the var with '$' caracter.  
>var="value"  
>echo $var

*Debbuging*
> keyword set - to start a section to debug and set - to end it  
> bash -x xx.sh to start the debug mode.

*Parameter*
> \$0 : name of the executable  
> \$1..\$n : user arguments entry while starting the bash  
> \$# : number of arguments  
> \$\$ : bash PID

*Read user entry*
> read  
> read var #*store entry to a variable*

*Arrays*
>array=('ele0','ele1','ele2')
>echo ${array[@]} # print all elements of the array  
>unset # remove an element  
>array[0]='value'

*Comparator*
> if [ op1 operator op2 ] then  
> ..  
> else  
> ..  
> fi  
> ***Operator:***  
> - eq : equal
> - ne : not equal
> - gt : greater than
> - lt : lesser than
> - ge : greater of equal
> - ...
>
> ***Option***
> if [ -option var ]
> - f: test if file exist
> - w: test if we have writting permission
> ...
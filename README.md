# os-emad-el-din
1- 

#!/bin/bash

echo "Enter a number of seconds "

read number

m=$(( $n / 3600 ))

b=$(( $n % 3600))

v=$(( $b / 60 ))

c=$(( $b % 60 ))

echo " $m : $v : $c "

---
2-

#!/bin/bash

echo "Enter a temperature in degrees Celsius "

read degree

x=`expr $degree \* 5`

y=`expr $x / 9`

z=`expr $y + 32` 

echo "$z" 

---

3-

#!/bin/bash

echo "Enter your salary "

read salary

x=$salary

if [ $x -gt 2000 ]

then

m=`expr $x \* 15`

s=`expr $m / 100`

r=`expr $salary - $s`

echo " $r "

elif [ $b -lt 2000 -a $x - 1000 ]

then 

y=`expr $x \* 10`

z=`expr $y / 100`

p=`expr $salary - $z`

echo " $p "

else

echo "No tax" 

---

4-

#!/bin/bash

echo "Enter  your number:"

read num

echo "Enter a power:"

read number

x=$num

y=$number

total=1

while [ $y -gt 0 ]

do

total=`expr $x \* $total`

x=`expr $x - 1`

done

echo "total =  $total"

---

5-

#!/bin/bash

echo "enter your number:"

read num

x=$num

z=`expr $x % 2`

if [ $x -eq 2 ]

then 

echo " $x is a primer number  "

elif [ $z -eq 0 ]

then



echo " $x is not a primer number  "



else

echo " $x is  a primer number  "

fi

---

6-

#!/bin/bash

echo "Please Enter a number or 0 To exit  "

read number

if [ $number -lt 0 ]

then 

echo "please enter positive number "

read num

else 

continue

fi       

total=0

n=0

average=0

while [  $num != 0 ]; 
do              
            

total=`expr $num + $total

n=`expr $n + 1`

echo "Please Enter a number or 0 To exit  " 

read number

if [ $number -lt 0 ]

then 

echo "please enter positive number "

read num

else 

continue

fi       

done



average=`expr $total / $n 



echo "The average of values is : $average "

---

7-

#!/bin/bash

echo "Enter a number"

read number

x=0

y=0

total=0

num=0

while [ $number -gt 0 ]

do

x=$(( $umber % 10 ))

y=$(( $y *\ 10 + $x ))

number=$(( $number / 10 ))

total=$(($total + $x))

num=$(($num + 1))

done

ave=$(( $total/ $num ))

echo " The eeverse number of entered digit is $y"

echo "the total of the digits $total"

echo "average of the digits $ave"


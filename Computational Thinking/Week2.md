# $L2.1:$ Conditional termination in iteration

Exiting a iteration basesd on specific condition 

- $Example:$ 
  - Suppose we are looking for specific cards which have Food and Apparel from shopping bills dataset and exit after that.
    - We would have to match food and apparel in the items category list and exit after that, so we don't need to iterate after we are done wit our objective and we can exit the loop.
  - Suppose We want to find the fist verb in the third line. We have to keep track of line number first, When we reached the third line then we start looking for the verb and exit after we find the verb.

```flowchart
e=>end
op1=>operation: Found= False
op2=>operation: Found= True
op3=operation: Other operations
cond1=>condition: Anoter card and not(Found)
cond2=>condition: Correct card

op1->cond1
cond1(yes,bottom)->cond2
cond1(no,rigt)->e
cond2(yes,rigt)->op2
cond2(no,bottom)->op3
op2->op3
op3(left)->cond1
```

# $L2.2:$ Local operations and max in a single iteration (Part 1)

- Suppose we want to find out the student has got the highest total marks
  - We have to keep track of highest marks card as we iterate through the scores dataset
  - Lets initialize a variable `max=0` since the marks can't be lower than `0`.

  - as we iterate through we see the max variable change from low to high

<center>

|max|~~0~~|~~174~~|~~209~~|~~227~~|~~254~~|~~261~~|281|
|-|-|-|-|-|-|-|-|

</center>

This is also an example of an iterator with filter in it. The filter compares the total marks in the card  and `max` variable and updates max if its smaller than the total in card.

# $L2.3:$ Local operations and max in single iteration (Part 2)

- Suppose we want to find out the longest sentence (max words).
  - We have to now keep track of two variable `count=0` and `longestSentence=0`
  - we count number of words until a word ends with `.`, Then compare `count` with `longestSentence`, if `longest sentence` is less than `count` we update it. Then we assign `count=0` and repeat untill no more words left.


|count|~~0~~|~~1~~|~~2~~|~~3~~|4|
|-|-|-|-|-|-|

|count|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|7|
|-|-|-|-|-|-|-|-|-|

|count|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|~~7~~|8|
|-|-|-|-|-|-|-|-|-|-|

|count|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|~~7~~|~~8~~|~~9~~|~~10~~|~~11~~|~~12~~|~~13~~|~~14~~|~~15~~|~~16~~|~~17~~|~~18~~|~~19~~|20|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|

|count|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|~~7~~|~~8~~|~~9~~|~~10~~|~~11~~|~~12~~|~~13~~|~~14~~|~~15~~|~~16~~|~~17~~|~~18~~|~~19~~|~~20~~|~~21~~|~~22~~|~~23~~|~~24~~|25|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|

|logestSentence|~~0~~|~~4~~|~~7~~|~~8~~|~~20~~|25|
|-|-|-|-|-|-|-|

# $L2.4:$ Local operations and max in single iteration (Part 3)

- Suppose we want to find out which shops are doing well. Well in the sence of number of bills they generate.
  - Since we don't know how many stors are there we are going to add a new count variable each time we see a new store.
    - The first card saw is from "SV Stores" so we add a new count variable `SV=0` and add 1 to it.

|SV|~~0~~|1|
|-|-|-|

- - - Now we see anoter new store `Big Bazar` so we add a new count variable `BB=0` and add 1 to it.

|SV|~~0~~|~~1~~|~~2~~|3|
|-|-|-|-|-|

|BB|~~0~~|~~1~~|2|
|-|-|-|-|

- - - Now we see anoter new store `Sun General` so we add a new count variable `SG=0` and add 1 to it.

|SV|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|~~7~~|~~8~~|~~9~~|~~10~~|~~11~~|~~12~~|~~13~~|~~14~~|15|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|

|BB|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|6|
|-|-|-|-|-|-|-|-|

|SG|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|~~7~~|~~8~~|9|
|-|-|-|-|-|-|-|-|-|-|-|

- - No we have to go throug another iteration to find which count is higest to find the shop that is doing well

- Suppose we want to find out the max in single iteration. so we also keep track of a variable `max=0` and update it if any seen shop bill counts have count more than max
  - Since we don't know how many stors are there we are going to add a new count variable each time we see a new store.
    - The first card saw is from "SV Stores" so we add a new count variable `SV=0` and add 1 to it.

|SV|~~0~~|1|
|-|-|-|

|max|~~0~~|1|
|-|-|-|

- - - Now we see anoter new store `Big Bazar` so we add a new count variable `BB=0` and add 1 to it.

|SV|~~0~~|~~1~~|~~2~~|3|
|-|-|-|-|-|

|BB|~~0~~|~~1~~|2|
|-|-|-|-|

|max|~~0~~|~~1~~|~~2~~|3|
|-|-|-|-|-|

- - - Now we see anoter new store `Sun General` so we add a new count variable `SG=0` and add 1 to it.

|SV|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|~~7~~|~~8~~|~~9~~|~~10~~|~~11~~|~~12~~|~~13~~|~~14~~|15|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|

|BB|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|6|
|-|-|-|-|-|-|-|-|

|SG|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|~~7~~|~~8~~|9|
|-|-|-|-|-|-|-|-|-|-|-|

|max|~~0~~|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|~~6~~|~~7~~|~~8~~|~~9~~|~~10~~|~~11~~|~~12~~|~~13~~|~~14~~|15|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|

# $L2.5:$ Local operations and max in single iteration (Part 4)

- When we were counting the bills we noticed that even though sv stores was producing ig number of bills but the total value of eac bill was less compared to Big Bazar.
- so the sum of total bill amount may be the better indicator of which shop is doing better.

  - Since we don't know how many stors are there we are going to add a new sum variable each time we see a new store.
    - The first card saw is from "SV Stores" so we add a new count variable `SV=0` and add the total value of card to it.

|SV|~~0~~|567|
|-|-|-|

|max|~~0~~|567|
|-|-|-|

- - - Now we see anoter new store `Big Bazar` so we add a new sum variable `BB=0` and add the total value of card to it.

|SV|~~0~~|~~567~~|~~1908~~|2031|
|-|-|-|-|-|

|BB|~~0~~|~~1525~~|5699|
|-|-|-|-|

|max|~~0~~|~~567~~|~~1525~~|~~1908~~|~~2031~~|5699|
|-|-|-|-|-|-|-|

- - - Now we see anoter new store `Sun General` so we add a new sum variable `SG=0` and add total value of card to it.

|SV|~~0~~|~~567~~|~~1908~~|~~2031~~|~~2127~~|~~3020~~|~~3299~~|~~3902~~|~~4494~~|~~5116~~|~~5244~~|~~6132~~|~~6224~~|~~6500~~|~~7014~~|7120|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|

|BB|~~0~~|~~1525~~|~~5699~~|~~8831~~|~~9426~~|~~12486~~|13284|
|-|-|-|-|-|-|-|-|

|SG|~~0~~|~~354~~|~~732~~|~~918~~|~~1574~~|~~1803~~|~~1990~~|~~2305~~|~~3669~~|4009|
|-|-|-|-|-|-|-|-|-|-|-|

|max|~~0~~|~~567~~|~~1525~~|~~1908~~|~~2031~~|~~5699~~|~~8831~~|~~9426~~|~~12486~~|13284|
|-|-|-|-|-|-|-|-|-|-|-|

# $L2.6:$ Max in a single iteration and max in two iterations (non-nested)

- $Example:$ It was Monday morning. Swaminathan was reluctant to open his eyes. He considered Monday specially unpleasant in the calendar. After the delicious freedom of Saturday and Sunday, it was difficult to get into the Monday mood of work and discipline. He suddered at the very thougt of school: that dismal yellow building; the fire-eyed Vedanayagam, his class-teacher; and the Head Master with his thin long cane...
<center>

|Word|count|Word|count|Word|count|Word|count|
|-|-|-|-|-|-|-|-|
|It|2|specially|1|get|1|building|1|
|was|3|unpleasant|1|into|1|fire-eyed|1|
|Monday|3|in|1|mood|1|Vedanayagam|1|
|morning|1|the|6|work|1|class-teacher|1|
|Swaminathan|1|calendar|1|discipline|1|Head|1|
|reluctant|1|After|1|suddered|1|Master|1|
|to|2|delicious|1|at|1|with|1|
|open|1|freedom|1|very|1|thin|1|
|his|2|of|3|thought|1|long|1|
|eyes|1|Saturday|1|school|1|cane|1|
|He|2|and|3|that|1|difficult|1|
|considered|1|Sunday|1|dismal|1|yellow|1|

|Max-frequency|~~1~~|~~2~~|~~3~~|~~4~~|~~5~~|6|
|-|-|-|-|-|-|-|
</center>

# $L2.7:$ Max in a single iteration witout losing information and applications of frequency count.

- Suppose we want to find out 

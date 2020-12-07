# Pain, Suffering, and Big O. 

## Mindset: there's a reason its called boot camp

the Codefellows curriculum and stacked module format is incredibly intense. It feels like I imagine Neo felt when he jacked into the matrix for the first time from the Nebuchadnezzar; but, much like Neo it isn't long before we look up and say some code-variant of "I know kung fu" 

The intensity of course is painful. It hurts, It creates a fertile environment for self doubt and second guessing, and it stretches and distorts our perception of time; feeling like it will never end. 

dealing with these feelings is a key componenet of succeeding and overcoming. this has a lot to do with out perception about the pain we experience. Our perception of the pain is the difference between being able to embrace the suck and achieve greatness, or drown ourselves in suffering. 

By focusing on the "Why", the reason we are subjecting ourselves to it we can better endure when it gets rough. it gives meaning to the pain and ultimately makes it worth it. I can't recall who said it but " pain, is inevitable, suffering is a choice" stay focused on the underlying values, and things that give meaning to the journey. fall in love with the process and no amount of pain will make you suffer. 

## Big O notation

this is a method of evaluating the effectiveness/efficiency of an Operation on a Data-set based on both the memory it requires and the time that it takes to complete given an input. 

*Constant Time* O(1)
This is the most efficient "grade" that an Operation can recieve. It states that: 

```
for any Input^Nth value time = 1 where 1 is a static unit of time. 

```
*Linear Time* O(N)

The second best grade an operation can recieve stating that: 

``` 
for any Input, time will be <= timeValue of Input

```
*Exponential Time* O(N^x)

Operations that take exponentially more time to complete for Inputs of greater size have much greater time to complete with the worst being noted at O(N^4) also called *Quadratic Time* ***avoid this at all costs***

## Python: Values, Names, References

Notes summarized from [Talk by Ned Batchelder](https://www.youtube.com/watch?v=_AEJHKGk9ns)

- Names **refer** to *values*
- Any number of Names can refer to the same value
- Names are reassigned independently therefore a name that refers to the same value as a second name(by way of reference to the first name) can be re-assigned to a new value and the second name will still point to the same value as the previous assignment of the first name. 

- Assignment NEVER copies data
- Values are broken into two types, mutable and immutable.
- the word change is unclear, when reasoning about code it can be better to use 're-bind' or 'mutate' respective to what you are actually trying to do.
- names have no type but values do, conversely values have no scope, but names do. 

- Avoid functions that mutate values; return a new value instead. (particularly relevant with lists).


#### [Return to Main index of Notes](./README.md)


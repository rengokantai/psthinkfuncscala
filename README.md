# psthinkfuncscala





##4. Placing Functions on Par with Objects as First Class Entities
###2 Converting Methods to Functions
original function
```
def getCircleArea(r:Double):Double=PI*r*r
```
we convert to expression:
```
val calcCircleArea :(Doublr)=>Double = getCircleArea
```
same as
```
val calcCircleArea = getCircleArea _
```
##5. Encouraging Functional Thinking via Cleverly Designed Collections
###1 Tuples as Lightweight Containers


###2 Creating and Using Lists
```
allDays forall (_ !="z")
alldays endsWith weekEnds
```

###3 Maps as Sets of Key-value Pairs
```
stateCodes.forEach((p:(String,String))=>println(p._1+"="+p._2))
```
```
(list1 zip list2).toMap
map.keySet.toList
```

###4 Options for Error-handling
```
fraction(22,7) match
{
  case Some(pi)=>pi
  case None=>"error"
}
```

####05:16
```
var stateCode = util.Try(stateCodes("NoSuchState"))
```

###5 Mutable Collections and Arrays
create a mutable list
```
var listBuilder = List.newBuilder[Int]
someLumbers.forEach(listBuilder+=_)
val result = listBuilder.result
```
##6. Understanding Precisely How Scan, Fold, and Reduce Work
###1 Simple Higher Order Methods
```
val weekDays = List("a','b')
weekDays.forEach(println(_))
```

```
weekDays.map(_ == "a")
```

create a function
```
val IsMonday = (s:String)=>{s=="a"}:Boolean

weekDays.map(isMonday)
```

filter and partition
```
weekDays.partition(isMonday)
```
returns List[String],List[String]) = (List(Mon,List(tue,Wed,Thu,Fri))


sortBy (create a new list, original list is unchanged)
```
weekDays.sortBy(_(0))   //sort by 1st char
```



###2 Scan Right
```
List(10,20,30,40,50,60)
```


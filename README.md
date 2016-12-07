# psthinkfuncscala

##5. Encouraging Functional Thinking via Cleverly Designed Collections
###1 Tuples as Lightweight Containers

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


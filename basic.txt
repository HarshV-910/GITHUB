jab bhi aap ek folder bnaate hai git ko kuchh nahi pata aapke folder ke
baare mein, isliye aap waha pe git ko initialize karte ho, ab git ko
permissions mili hai to git aapke folder ko pehchaanta hai, to ab kyuki git kaam kar skta hai is folder per ab ham yaha par untracked, tracked,modified, staged, and saved checkpoints create kar skte hai, git kuchh
interesting cheeje kar skta hai jaise ki aap chaahe to kisi bhi moment par
ye check kr skte ho aapki kitni files kis stage par hai

-> initialize karo : 
```
git init
```

-> check kr skte ho aap konsi file kis stage mein hai
```
git status -s
```

-> check kr skte ho aap kitne saved checkpoints hai 
```
git log --oneline --graph
```

git status bataata hai commit ke pahle and baad ki file stage
git log bataata hai saare commit histories
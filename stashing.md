jab aap kisi branch mein kaam kr rhe ho and aapne kuchh code likha hai and aapne us code ko commit nahi kiya hai, aur aap doosri branch mein jaane ki koshish krte ho to git aapko bolta hai ki bhai saved nahi changes delete o jaayege hum chaahe to un chnages ko delete hone yaa fir un chnages ko draft kr skte hai, jab bhi draft
karege to wo changes naa hi delete honge na hi add hobnge but beech mein kahi dale rahege fir aap us branch mein Yab waapas aaye to wo changes waapas se apply kr skte ho.


basically stashing is like drafting a codes or messages. Such messages that now we not want to do commit or staged(added) at that time we can keep it as stash(draft) and then we can change branch, and when we want we can get back.

for stashing : ```git stash```
for get back stashed messages : ```git stash apply```
#  Billo bage billiya de ki karegi Git padhake tu kya karegi 😂🤮🤣😒❤️❤️❤️❤️😊
#  Pyari si shuruaat pyare se logo ke sath welcome to msdelta_t coding.

# 1.GitHub
    => working on a central code base is called GitHub.

# 2.Git 
    => managing project on our system in different variant like creating different version and saving them as different - different check points

# Note:
    terminal m git run kar raha h tho usse exit karne ka tarika h ya close karne k liye -> Press Q

# 3.More INFO about GIT: 
[Click here](intro.md)

# Note:
    -> agar apan ko koi file ignore karni h tho we add .gitignore file in our folder, tho git isse track nhi karega

# Note:
    -> agar apan ko ek step piche jana h tho we use (git reset --hard HEAD~1) ye hamari commit kari hue chijo ko previous commit pe le aaega jisse hame hamara pichala code milega par ye recent wale ko delete kar dega and then previous pe leke jaega. and jitane step piche jaege utana forward step delete ho jaega. previous step pe jane ke liye we use for more than one we change here (git reset --hard HEAD~1/2/3/4) 1 ki jagh 2, 3, ya 4 use kare tho ye utane step piche chala jaega and file untracked reh jaegi.

    --> and there are three level of reset :
    1. hard
    2. soft
    3. mixed

## Example Image
![Privious commit image](<Screenshot 2026-06-23 090116.png>)

# Link for add images in vscode 
YOUTube link :- [link](https://www.youtube.com/watch?v=jpeh1WorrWM)

# How to use preview
![alt text](<Recording 2026-06-23 093018.gif>)

# 4.According to lecture 3:
    -> check kar skte ho aap konsi file kis stage mein hai -> ( git status -s) and this code is run on terminal, git status srf unka status bataayega jo files committed nahi hai ya fir commit hone ke baad change ki gayi h.

    mota mota:- git status bataata hai saare commit histories.

    -> check kr skte ho aap kitne saved checkpoint hai -> (git log --oneline --graph) 

# 5.Lets see branching  concept:-
    Branching :- main branch se ek copy leke another branch m use karna it is called branching.
    and jo other branch h uska code commit karne ke baad hi us branch ka banega.
    tho sabse pahale branch banane ke liye apan code use karege (git branch branch_name) then main branch se switch karne ke liye we use (git switch branch_name). 
    Agar koi branch delete karni h tho we use (git branch -d branch_name).
# eg:- Preview of branching:
  <video controls src="Screen Recording 2026-06-24 113822.mp4" title="Branch"></video>

# 6.Merging concept in branching:-
    merge karne ke liye main branch pe hona zaruri h. then u use code (git merge branch_name) esa karne se sub branch se code main branch m aajaega.

# eg:- Preview of merge branch:-
<video controls src="Screen Recording 2026-06-24 152835.mp4" title="Title"></video>

# 7.Branches conflict problem:-
    -> if we add a new line in main branch and a new different line in sub-branch then it will conflict to avoid this git give us 3 options 
    1. Accept current change :- apply main branch change
    2. Accept incoming change :- apply sub-branch change
    3. Accept both changes :- apply both changes
    4. Compare changes (non of out buss..)
# for eg:- 
  <video controls src="Screen Recording 2026-06-24 160646.mp4" title="Conflict problem"></video>

# Note: 
  all branches are deleted if you want to try merging and anything create a branch by yourself. and merge karne ke baad branch ka kaam khatam ho jata h tho hume usse delete kar dena chahiye(baaki tumhari marzi😤😤).

# 8.Three way merging:-
    isme sabse pahale ek main branch and ek sub-branch m kuch code likhe hoge and inn code ko me dono jagh hi changes kiye jaege main branch m ek different code hoga and sub-branch m different fir unhe jab merge karege tho first main commited h and 2 nd main commited and sub-branch 2nd commited inn tinoko include karke banega three way merging.

# eg for better understanding, Same as above merging:-
  <video controls src="Screen Recording 2026-06-24 160646.mp4" title="Title"></video>

## 9.Stashing Samajhna:
  # Note:
    jab aap kisi branch mein kaam kr rhe ho and aapne kuchh code likha hai and aapne us code ko commit nahi kiya hai. aur aap doosri branch mein jaane ki koshish krte ho to git aapko bolta hai ki bhai saved nahi changes delete o jaayege hum chaahe to un changes ko delelte hone yaa gir un changes ko draft kr skte hai, jab bhi draft karege to wo changes naa hi delete honge na hi add hobnge but beech mein kahi dale rahege fir aap us branch mein jab waapas aaye to wo changes waapas se apply kr skte ho.
      --> mota mota:- bina commit kare sub-branch pe switch karna h then we use (git stash) this command will save your uncommited changes in git memory and when we want to apply those changes we use:- (git stash apply) and then we commit our changes.

# eg of stash:- 
  <video controls src="Screen Recording 2026-06-24 213206.mp4" title="Stash making"></video>

# eg of stash clear:-
  -> to clear stash we use (git stash clear).
  <video controls src="Screen Recording 2026-06-24 213525.mp4" title="Stash clear"></video>

# 10.Git and GitHub collaboration:
    -> to learn collaboration in git and github checkout the git collaboration folder. ('git collaboration' = name of a folder in which i understand git and git collaboration)

    -> git collaboration ke liye sabse pahale ek git account banake uspe ek repository (public,private doesn't matter) bano fir apane vscode pe aake kuch file create karo and usme ek .md file bano by using this code(echo "# collaboration_with_msdeltat" >> README.md) and then git ko initalise karo by using this code(git init) and then tumhe sari files ko stage karlena h by this command (git add .) and then aapko unhe commit karna h by using this command(git commit -m "first commit ") and then main branch p aane ke liye aapan use kare h (git branch -M main) and then we add our repository url to tell git where our this code have to go by using this code (git remote add origin your_git_repository_URL) and then we push our code by using code (git push -u origin main) yaha par apna main bande ka kaam khatam.

    -> now collaborator ka kaam vo apne email par jake invite accept karke repo ko khudh ke vscode me cloning karega clone karne ke liye link vo github se lelega fir use this code(git clone copy_kiya_hua_URL) isse sari files uske system par aayaegi fir vo jo folder uske system me aaega usse terminal par active karke fir vo ek branch banaega fir uss branch ke andar change kar sakata h fir vo usse commit karke push kar dega apani sub_branch m hi and apani sub_branch push karege main nhi (git push -u origin sub_branch) fir aapke change kiye hue code ki branch github pe chali jaegi and main banda usse fetch (git fetch) karke usse fir main bande ko apani main branch se merge karke aapke code ko main central code base pe commit kar dega.
    and ek or baat jab collaborator apane main branch pe aaega tho usse vo change kiya hua code nhi milega tho vo main branch pe aake code use karega (git pull) to get all changes and fetch and merge bhi ho jaega.

  # Note:
    apan fecth and merge ek saath kar sakate h by useing (git pull) ye code fetch and merge dono kar dega.

  # For more info:
  [for better understand](https://www.youtube.com/watch?v=cn8l5bXhTBM&list=PLbtI3_MArDOlJ4036mWiUKaQToUS8MZVu&index=6)
# 1.Steps of how to use git:
    -> git installation

# 2.Stages:
    U - untracked
    A - added or staged
    M - Modified file after commited
    C - commited

# 3.Install extensions:
    git blame
    git theme
    git auto config

# 4.Setup golobally commands use these commands in cmd:
    git config --global user.name "name"
    git config --global user.email "email@dfa"
    git config --global core.editor "code --wait" jab git problem face karega tab terminal open ho jaega and uspe likha aaega waiting.
    git config --global core.autocrlf 
    auto crlf ke liye value set karni padati h like core.autocrlf "input".

# 5.Commands you need to know:
git config --global -e :- it will show our username and above entries.
git status -s => to know current status and staged files
git log --online => to know current status of saved points

# 6.Managing your own projects:
    making git available in our project making a checkpoint or saved point 
        adding files 
        staging them 
        commiting them
# 7.Going back to some previous saved point:
    logging everything
    reverting back to the previous saved point

## -> agar apan ko koi (untracked)file ignore karni h tho we add .gitignore file in our folder, tho git isse track nhi karega

## 8.Lecture 3 :
    --> Learning about status and logs - making possibilities - branching
        1. status dekhna
        2. logs check karna with graph option
        3. branch samajhna
        4. branch merge karna 

    -> merging techniques - (ff merge, three way merge) - only these two are necessary, squash merging, recursive strategy merge, rebase and merge

    conflicts handle karna 
    branch delete karna 
    ~ stashing samajhna

# 9.Git and GitHub Collaboration:
    -> Common Steps:-
    main banda(person) folder and initial files banaaye
    ab usse github par daal de
    collaborators add kare

        saare bande us repo se cloning karein
        [Very important] apni branch create karein
        apna code usi branch mein likhein
        complete hone par commit dein
        inform karein teammate ko about the commit 
        merger banda fetch karega and merge karega and re-push.
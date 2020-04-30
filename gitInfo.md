# NPM full info

[all npm camand wotch this](https://docs.npmjs.com/cli-documentation/cli)

[full info for NPM](https://blog.bitsrc.io/a-beginners-guide-to-npm-5c021d519c4c)

***

[full info about packij.json](https://dev.to/easybuoy/understanding-the-package-json-file-3fdg)
A pack.json- ը JSON ֆայլ է, որը գոյություն ունի Javascript / Node նախագծի հիմքում: Այն պարունակում է նախագծին վերաբերող մետատվյալներ և այն օգտագործվում է ծրագրի կախվածության, սցենարների, վարկածի և այլնի կառավարման համար:

Կան կանոններ որոնց պետք է հետևել

- must be lowercase
- must be one word
- can contain hyphens and underscores
- should not start with an underscore(_) or dot(.)

 - Version   property denotes the current version of the module for the project.

- description The description property is used in describing and providing more information about the project.

 - engines The engines property is a JSON object of key/value pairs that are used to denote/specify the version of the libraries and runtimes on which the application should run.

- dependencies The dependencies property denotes the list of the required modules/packages for your application to function. After installing a dependency, it is added to the dependencies list.To install a dependency, run npm i package or npm install package on your terminal. Where the package is the name of the package you are trying to install.

- scripts
The script property takes a JSON object of key/value pairs. Each script can be used in performing different sets of tasks, like building, testing, linting the application.

- main
The main property serves as the entry point of your application and should point to the file that serves as the entry point to your application.

- homepage
The homepage property is used to specify the landing page for the application/package.

- private
The private property is false by default but can be set to true to prevent the application/package to be published.

- license
This property denotes the type of license that's being used by the project

- author
This property denotes the creator/owner of the project

- repository
The repository keyword is a JSON object of key/value pairs that are used to specify the version control system being used to manage the application. You can specify the type of version control being used,
the URL to the repository, as well as an optional directory within the repository.

- bugs
The bugs property is used to point to the issues page of the repository for the application or anywhere the project issues can be reported.

- keywords
The keywords property is an array of keywords that helps in identifying your project or make your project easier to find when a user searches those keywords.

- Custom Properties
The package.json file can also be used for package specific commands like Babel, ESLint, Jest and lots more. You can find the usage in the package documentation.
Find an example of a custom property for Jest below.

[whole property in packije.json see here](https://docs.npmjs.com/files/package.json)

***

-npm init: Helps to initialize a project by asking a series of question such as name, version, author and so on. At the end a brand new package.json file is created with that information. You also have the ability to provide a custom initializer to customize the processed to your particular stack.

Սա կապ չունի git init-ի հետ:

## git-init 
 **Create an empty Git repository or reinitialize an existing one.** Most other Git commands are not available outside of an initialized repository, so this is usually the first command you'll run in a new project. Git doesn’t require you to create a repository, import files, and check out a working copy. Additionally, Git does not require any pre-existing server or admin privileges. All you have to do is cd into your project subdirectory and run git init, and you'll have a fully functional Git repository.A quick note: git init and git clone can be easily confused. At a high level, they can both be used to "initialize a new git repository." However, git clone is dependent on git init. git clone is used to create a copy of an existing repository. Internally, git clone first calls git init to create a new repository. It then copies the data from the existing repository, and checks out a new set of working files. 

 Create a new git repository for an existing code base
- cd /path/to/code \
- git init \
- git commit

Create a new bare repository

- git init --bare /path/to/repo.git

**aliasian**
- $ git config --global alias.co checkout
- $ git config --global alias.br branch
- $ git config --global alias.ci commit
- $ git config --global alias.st status
 - [alias]

            - co = checkout
            - br = branch
            - ci = commit
            - st = status

Git aliases are a powerful workflow tool that create shortcuts to frequently used Git commands. Using Git aliases will make you a faster and more efficient developer. Aliases can be used to wrap a sequence of Git commands into new faux Git command. Git aliases are created through the use of the git config command which essentially modifies local or global Git config files.



# GitInfo

***

You’ll learn how to:

1. Create and use a repository
2. Start and manage a new branch
3. Make changes to a file and push them to  GitHub as commits
5. Open and merge a pull request
*** 

## git add

 - ***git add*** -անելուց հետո այն չի երեում ***repository*** -ում:Ավելացնում է լոկալ հիշողության մեջ,"*save*"-է անեւմ,և կարող էնք հետ բերել:
  
    - y - stage this hunk
    - n - do not stage this hunk
    - q - quit; do not stage this hunk or any of the remaining ones
    - a - stage this hunk and all later hunks in the file
    - d - do not stage this hunk or any of the later hunks in the file
    - g - select a hunk to go to
    - / - search for a hunk matching the given regex
    - j - leave this hunk undecided, see next undecided hunk
    - J - leave this hunk undecided, see next hunk
    - k - leave this hunk undecided, see previous undecided hunk
    - K - leave this hunk undecided, see previous hunk
    - s - split the current hunk into smaller hunks
    - e - manually edit the current hunk
    ? - print help
***

 ## staging area
  Այն տարացքն է որտեղ լցվում է get add արածը:համարվում է **git** - ի <երեք ծառերից մեկը>,working directory and commit history:
  
  ***

## git cmmit 
 -***git cmmit*** -ավելացնում է լոկալ "repository"-ի մեջ:Այն կարելի համարել "projecti"-ի <անվտանգ> վարկածներ:փոփոխությունները լցվում են լոկալ "repository"-ներ և դա ոչ մի փոխազդեցություն չունի այլ "repository"-ի հետ,հետագայում այն կարեղ է մղվել հեռավոր պահեստներ:



***
## git diff
[Diff-i comandnery tesnelu hamar anceq aystexov](https://www.atlassian.com/git/tutorials/saving-changes/g)

Difing - գործառույթ է, որն իր մեջ ներառում է երկու մուտքային տվյալների հավաքածու և արդյունքներ է տալիս դրանց միջև տեղի ունեցող փոփոխություններին: Git diff հրամանը հաճախ օգտագործվում է git կարգավիճակի և git log- ի հետ միասին ՝ Git repo- ի ներկայիս վիճակը վերլուծելու համար:
Եթե չի նշվում ֆայլի հասցեն,ապա համեմատությունը կատարվում է ամբողջ repositoriayum ընդ որում լոկալ:
Քննարկեցինք, թե ինչպես կարելի է կարդալ git dif արդյունքը և արտադրանքի մեջ ներառված տարբեր տվյալները: Տրվեցին օրինակներ, թե ինչպես կարելի է փոխել git diff արդյունքը կարևորելով և գույներով: Քննարկեցինք տարբեր տարբեր ռազմավարություններ, ինչպիսիք են `ինչպես տարբեր ֆայլերը մասնաճյուղերում և հատուկ հանձնառությունները: Բացի git diff հրամանից, մենք նաև օգտագործել ենք git log և git checkout:

*** 

## Git stash

- Stashing your work
- Re-applying your stashed changes
- Stashing untracked or ignored files
- Managing multiple stashes
- Viewing stash diffs
- Partial stashes
- Creating a branch from your stash
- Cleaning up your stash
- How git stash works

Եթե ունեմ change բայց չեմ ուզում այն cmmit անել stash եմ անում պահումա հիշողուրյան մեջ հետո վերցնում եմ:
Git stash հրամանը տանում է ձեր աննկատ փոփոխությունները (ինչպես բեմադրված, այնպես էլ չկատարված), դրանք պահպանում է հետագա օգտագործման համար, այնուհետև դրանք վերադարձնում է ձեր աշխատանքային օրինակից:
Նկատի ունեցեք, որ ստանդարտը տեղական է ձեր Git պահեստարանին. սեղմելիս stashes- ը չի փոխանցվում սերվերին:

Կարող եք նորից վերականգնել git stash pop նախկինում տեղադրված փոփոխությունները.

Այսպիսով, եթե մենք ավելացնում ենք երրորդ ֆայլ,բայց այն մի stage (այսինքն `մենք չենք գործարկում git հավելված), git stash- ը չի ստացվի:Ավելացնելով -u տարբերակը (կամ --include-untracked) ասում է git stash- ը նաև ստվերում անթափանց ֆայլեր.Դուք կարող եք ներառել փոփոխություններ անտեսված ֆայլերի վրա, ինչպես նաև git stash- ը գործարկելիս անցնելով –a տարբերակը (կամ - all):

Դուք չեք սահմանափակվում միայն մեկ stash: Կարող եք մի քանի անգամ գործարկել git stash ՝ բազմակի stashes ստեղծելու համար, այնուհետև դրանք դիտելու համար օգտագործել git stash ցուցակը: Լռելյայն, stashes- ը նույնացվում է պարզապես որպես «WIP» ՝ ընթացքի մեջ աշխատող, մասնաճյուղի վերևում և պարտավորվում է, որ դուք ստեղծեք stash: 
Մի փոքր ավելի շատ համատեքստ ապահովելու համար լավ պրակտիկա է, որ ձեր stashes- ը նկարագրեք նկարագրությամբ ՝ օգտագործելով git stash save «հաղորդագրություն».
Լռելյայն, git stash փոփը նորից կկիրառի ամենավերջին ստեղծված stash- ը. Stash @ {0 Կարող եք ընտրել, թե որ շտեմարանը նորից դիմի ՝ իր նույնացուցիչը փոխանցելով որպես վերջին փաստարկ, օրինակ.$ git stash pop stash@{2}.

Git stash շոուի հետ կապված Stash- ի համառոտ նկարագիրը կարող եք դիտել.
$ git stash show .
Կամ անցեք -p տարբերակը (կամ --patch) ՝ դիտելու stash- ի ամբողջական տարբերությունը.
$ git stash show -p.

Կարող եք նաև ընտրել միայն մեկ ֆայլ, ֆայլերի հավաքածու կամ ֆայլերի ներսում անհատական փոփոխություններ: Եթե անցնեք -p տարբերակը (կամ - patch) ստանդարտացման իրավունք ստանալու համար, ապա դա կկրկնկի յուրաքանչյուր փոփոխված« որսի »միջոցով ձեր աշխատանքային օրինակով և հարցնում է `ցանկանո՞ւմ եք այն ներբեռնել:
- You can hit ? for a full list of hunk commands. Commonly useful ones are:
  - /	search for a hunk by regex
  - ?	help
  - n	don't stash this hunk
  - q	quit (any hunks that have already been      - selected will be stashed)
   - s	split this hunk into smaller hunks
  - y	stash this hunk

Բացակայում է «դադարեցնելու» հրամանը, բայց CTRL-C (SIGINT) հարվածելը կասեցնի փորձնական գործընթացը:


Եթե ​​ձեր մասնաճյուղում կատարված փոփոխությունները տարբերվում են ձեր ստանդարտի փոփոխությունից, կարող եք բախումներ առաջանալ ձեր when popping or applying: Փոխարենը, դուք կարող եք օգտագործել git stash մասնաճյուղ ՝ նոր մասնաճյուղ ստեղծելու համար ՝ ձեր ստացված փոփոխությունները կիրառելու համար.
Սա ստուգում է new branche`հիմնվելով այն commit պարտավորության վրա, որից դուք ստեղծել եք ձեր stash, և այնուհետև արձակում է ձեր վրա դրված փոփոխությունները:

Եթե ​​որոշեք, որ այլևս կարիք չկա որոշակի ստանդարտի, կարող եք ջնջել այն $ git stash drop stash@{1}:Կամ դուք կարող եք ջնջել ձեր բոլոր ստաշերը հետևյալի միջոցով.$ git stash clear

Եթե մեզ հետաքրքիր է թե ոնց է աշխատում stash -ը [կարեղ էք անցնել այստեղով](https://www.atlassian.com/git/tutorials/saving-changes/git-stash)


***
# .gitignore
Git sees every file in your working copy as one of three things:

1. tracked - a file which has been previously staged or committed;
2. untracked - a file which has not been staged or committed
123. ignored - a file which Git has been explicitly told to ignore.

Ignored ֆայլերը սովորաբար լինում մեքենայական ֆայլեր, որոնք կարող են ստացվել ձեր պահեստի աղբյուրից:Դրանք հիմնականում լինում են:
 - /node_modules or /packages
 - compiled code, such as .o, .pyc, and .class files
 - build output directories, such as /bin, /out, or /target
 - files generated at runtime, such as .log, .lock, or .tmp
 - hidden system files, such as .DS_Store or Thumbs.db
 - personal IDE config files, such as .idea/workspace.xml

 Ignored ֆայլերը հետևվում են հատուկ ֆայլում .gitignore անունով, որը ստուգվում է ձեր պահեստի հիմքում: Ոչ մի հստակ git անտեսման հրաման չկա. Փոխարենը .gitignore ֆայլը պետք է խմբագրվի և կատարվի ձեռքով, երբ ունեք նոր ֆայլեր, որոնք ցանկանում եք անտեսել:
 - Ignoring files in Git
    [kardal sranc masin aystex](https://www.atlassian.com/git/tutorials/saving-changes/gitignore)
    - Git ignore patterns
    - Shared .gitignore files in your repository
    - Personal Git ignore rules
    - Global Git ignore rules
    - Ignoring a previously committed file
    - Committing an ignored file
    - Stashing an ignored file
    - Debugging .gitignore files

** -Այս բացատրությունները ենթադրում են, որ ձեր .gitignore ֆայլը գտնվում է ձեր պահեստի վերին մակարդակի գրացուցակում, ինչպես և կոնվենցիան: Եթե ձեր պահեստը ունի բազմաթիվ .gitignore ֆայլեր, պարզապես մտավոր փոխարինեք «պահեստի արմատը» «գրացուցակը պարունակող .gitignore ֆայլը» գրացուցակով (և հաշվի առեք դրանք միավորելը ձեր թիմի առողջության համար):

#### Բացի այս նիշերից, ձեր .gitignore ֆայլում մեկնաբանությունները ներառելու համար կարող եք օգտագործել #:
#### Կարող եք օգտագործել \ .Gitignore- ի օրինակելի նիշերից խուսափելու համար, եթե դրանք պարունակող ֆայլեր կամ դիրեկտորիաներ ունեք.


մենք կարող եք սահմանել Git- ի գլոբալ անտեսումը մեր տեղական համակարգի բոլոր պահեստարանների համար `սահմանելով Git այսպես

- $ touch ~/.gitignore
- $ git config --global core.excludesFile ~/.gitignore

Եթե ցանկանում եք անտեսել նախկինում կատարված ֆայլը, ապա ձեզ հարկավոր է ջնջել ֆայլը ձեր պահեստից, այնուհետև դրա համար ավելացնել gitignore կանոն: Git rm- ով պահված տարբերակը օգտագործելը նշանակում է, որ ֆայլը կջնջվի ձեր պահեստից, բայց կմնա ձեր աշխատանքային գրացուցակում `որպես անտեսված ֆայլ:

- $ echo debug.log >> .gitignore
- $ git rm --cached debug.log
rm 'debug.log'
- $ git commit -m "Start ignoring debug.log"


Հնարավոր է ստիպել, որ անտեսված ֆայլը հանձնվի պահեստարան `օգտագործելով -f (կամ - forc) տարբերակը git ավելացնելով.

- $ cat .gitignore
*.log
- $ git add -f debug.log
- $ git commit -m "Force adding debug.log"

Եթե ունեք բարդ .gitignore նախշեր կամ բազմաթիվ .gitignore ֆայլերի վրա տարածված նախշեր, դժվար է պարզել, թե ինչու է որոշակի ֆայլ անտեսվում: Կարող եք օգտագործել git check-անտեսման հրամանը –v (կամ --verbose) տարբերակով ՝ որոշելու, թե որ օրինաչափությունն է առաջացնում որոշակի ֆայլի անտեսում.
- $ git check-ignore -v debug.log
.gitignore:3:*.log debug.log

The output shows:
<file containing the pattern> : <line number of the pattern> : <pattern> <file name>

Ցանկության դեպքում կարող եք մի քանի ֆայլի անուններ փոխանցել, որպեսզի git check-check- ը անտեսվի, և անուններն իրենք անգամ պարտադիր չեն համապատասխանելու այն ֆայլերին, որոնք առկա են ձեր պահեստում:


***

## git status
-***git status*** -հրամանը կարող է օգտագործվել staging area -ի վիճակը հետազոտելու և կատարված պարտավորությունների կատարման համար:
Git status հրամանը ցույց է տալիս աշխատանքային գրացուցակի վիճակը և բեմադրության տարածքը: Այն թույլ է տալիս տեսնել, թե որ փոփոխությունները բեմադրվել են, որոնք չկան, և որ ֆայլերը չեն դիտարկվում Git- ի կողմից: Կարգավիճակի արդյունքը ձեզ որևէ տեղեկատվություն չի ցույց տալիս կատարված նախագծի պատմության վերաբերյալ: Դրա համար անհրաժեշտ է օգտագործել git log:

Այն համեմատաբար պարզ հրահանգ է և տալիս է 3 արժեք:
- modified: hello.py
- modified: main.py
- hello.pyc

Լավ պրակտիկա է `փոփոխություններ կատարելուց առաջ ստուգեք ձեր պահեստի վիճակը, որպեսզի պատահականորեն չկատարեք այնպիսի բան, որը չեք նկատի: Այս օրինակը ցուցադրում է պահեստի կարգավիճակը նախքան և հետո նկարահանումները կատարելուց և կատարելուց.

- git status
- git add hello.py
- git status
- git commit
- git status

***
## Undoing Changes
Git պահեստի պատմությունը վերանայելու լավագույն կոմունալ ծառայություններից մեկը git log հրամանն է:Հրամանի git branch օգտագործվում է այլ մասնաճյուղեր դիտելու և այցելելու համար: Հրավիրելով հրամանը ՝ git branch -a կվերադարձնի բոլոր հայտնի մասնաճյուղերի անունները: Այս մասնաճյուղերի անուններից մեկը այնուհետև կարող է գրանցվել git log <branch_name> օգտագործմամբ:
- git log --online
- b7119f2 Continue doing crazy things
- 872fa7e Try something crazy
- a1e8fb5 Make some important changes to - hello.txt
- 435b61d Create hello.txt
- 9773e52 Initial import

**git checkout a1e8fb5**

Սա ձեր աշխատանքային գրացուցակը դարձնում է a1e8fb5 ստանձնած պարտավորության ճշգրիտ վիճակին: Կարող եք նայել ֆայլեր, կազմել նախագիծը, գործարկել թեստեր և նույնիսկ խմբագրել ֆայլերը ՝ առանց մտավախություն ունենալու նախագծի ներկայիս վիճակը կորցնելու մասին: Այստեղից ոչ մի գործ չի պահվի ձեր պահեստում: Շարունակելու զարգացումը, դուք պետք է վերադառնաք ձեր նախագծի «ներկայիս» վիճակին.

**git checkout master**

Սա ենթադրում է, որ դուք զարգանում եք defoult master branch: Վերադառնալուն պես վարպետության մասնաճյուղում, կարող եք օգտագործել կամ git revert կամ git reset ՝ անցանկալի փոփոխություններ չեղարկելու համար:

**git reset or git revert**

Reverting

<!-- ![Revert and Resert](C:\Intel\picture1.jpg) -->


              ->->->->
             /        \
            /          \
O------->X-------> O ------->O

1. Reverting երկու կարևոր առավելություն ունի rendering-i հետ կապված: Նախ, այն չի փոխում նախագծի պատմությունը, ինչը այն դարձնում է «անվտանգ» գործողություն այն հանձնարարականների համար, որոնք արդեն հրապարակվել են ընդհանուր պահոցում:

2. Երկրորդ, git revert- ը ի զորու է նպատակ ունենալ անհատին կատարել պատմության կամայական կետում, մինչդեռ git reset-ը կարող է միայն հետընթաց աշխատել ընթացիկ պարտավորությունից: Օրինակ, եթե դուք ցանկանում եք հետարկել հին գործառույթը git reset , ապա պետք է հեռացնեք թիրախային հանձնառությունից հետո տեղի ունեցած բոլոր հանձնառությունները, հանեք այն, ապա կրկին կատարեք հետագա բոլոր հանձնառությունները: Ավելորդ է ասել, որ սա էլեգանտ լուծում է: 


Փոփոխությունները չեղարկելու այս եղանակը ամենաամաքուր ազդեցությունն է ունենում պատմության վրա: Reset կատարելը հիանալի է տեղական փոփոխությունների համար, սակայն դա բարդություններ է ավելացնում, երբ աշխատում է հեռակա պահեստի հետ աշխատելիս: Եթե մենք ունենք մի հեռավոր պահոց, որը 872fa7e պարտավորությունն է դրել դրան, և մենք փորձում ենք git push մի ճյուղ, որտեղ մենք վերականգնել ենք պատմությունը, Git- ը դա կբռնի և սխալ կխփի: Git- ը ենթադրելու է, որ մbranch-y, որը push է linum, արդիական չէ, քանի որ բացակայում է cmmity: Այս սցենարներում git revert-y պետք է լինի նախընտրելի վերացման մեթոդ:

               <-<-<-<-
              /         \
             /           \
O-------->O--------->O--------->X


When working on a team with remote repositories, extra consideration needs to be made when undoing changes. Git reset should generally be considered a 'local' undo method. A reset should be used when undoing changes to a private branch. This safely isolates the removal of commits from other branches that may be in use by other developers. Problems arise when a reset is executed on a shared branch and that branch is then pushed remotely with git push. Git will block the push in this scenario complaining that the branch being pushed is out of date from the remote branch as it is missing commits.

The preferred method of undoing shared history is git revert. A revert is safer than a reset because it will not remove any commits from a shared history. A revert will retain the commits you want to undo and create a new commit that inverts the undesired commit. This method is safer for shared remote collaboration because a remote developer can then pull the branch and receive the new revert commit which undoes the undesired commit.


git reset vs git checkout

***git checkout***
 
|a|----|b|----|c|----|d|<----|master|

         ^
         |
         |
       |head|


***git reset***

[a]----[b]  aranzin branchea [c]-----[d]

         |
         |
    [head,master]


***

## git clean
Այս բաժնում մենք կանդրադառնանք git clean հրամանի մանրամասն քննարկմանը: Git clean որոշ չափով «հետադարձ» հրաման է: Git cleany կարելի է համարել լրացում այլ հրամանների git reset և git checkout: Այն դեպքում, երբ այս մյուս հրամաններն աշխատում են Git- ի հետևելու ինդեքսում նախկինում ավելացված ֆայլերի վրա, git- ի clean հրամանը գործում է չկարգավորված ֆայլերի վրա: Չհրապարակված ֆայլերը ֆայլեր են, որոնք ստեղծվել են ձեր repo- ի աշխատանքային գրացուցակում, բայց դեռ չեն ավելացվել պահեստի դիտարկման ինդեքսում օգտագործելով git add հրամանը: Լրիվ կատարման դեպքում, git Clean- ը կդառնա ֆայլերի համակարգի կոշտ ջնջում,այսինքն բոլոր չճշտված ֆայլերը կջնջվեն:Համոզվեք որ ուզում եք ամբողջությամբ ջնջել այն:

**$ git clean -n** տարբերակը կկատարի git մաքուր «չոր գործարկում»: Սա ցույց կտա ձեզ, թե որ ֆայլերը կհանվեն, առանց դրանք իրականում հանելու: Լավագույն պրակտիկա է, որ միշտ առաջին հերթին կատարեք git մաքուր չոր արտահոսք: Այս տարբերակը մենք կարող ենք ցույց տալ ավելի վաղ ստեղծած ցուցադրական ռեպոում:

**$ git clean -f** or --force Ուժի տարբերակը նախաձեռնում է untracked files փաստացի ջնջում ընթացիկ գրացուցակից: Սա չի հեռացնի չկարգավորված պանակները կամ ֆայլերը, որոնք նշված են .gitignore- ով:
- git clean -f <path>
- -d include directories

այս ձևով կարող ենք մեր ուզաց untracked files-ը նշել ու ջնջել:Կան նաև
- $ git clean -dn
- Would remove untracked_dir/
- $ git clean -df
- Removing untracked_dir/
- -x force removal of ignored files

 Լավագույն փորձ է նախևառաջ վերջնական ջնջումը կատարել «dry run»:

- git clean -xf

Այս օրինակը ցույց է տալիս մի համադրություն -f- ի հետ, որը կհեռացնի չկտրված ֆայլերը ընթացիկ գրացուցակից, ինչպես նաև ցանկացած ֆայլ, որը Git- ը սովորաբար անտեսում է:

Կա նաև git clean -i (interactive) որը բաղկացած է 6 քայլից
1. clean 
2. filter by pattern 
3. select by numbers 
4. ask each 
5. quit 
6. help What now

- What now> 6
- clean - start cleaning
- filter by pattern - exclude items from  deletion
- s elect by numbers - select items to be  deleted by numbers
- ask each - confirm each deletion (like  "rm -i")
- quit - stop cleaning
- help - this screen
- ? - help for prompt selection

***

## Three Trees of Git

- Working directory


Git status can be used to show changes to the Working Directory. They will be displayed in the red with a 'modified' prefix.

1. $ mkdir git_reset_test
2. $ cd git_reset_test/
2. $ git init .
Initialized empty Git repository in /git_reset_test/.git/
2. $ touch reset_lifecycle_file
2. $ git add reset_lifecycle_file
2. $ git commit -m"initial commit"
[master (root-commit) d386d86] initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 reset_lifecycle_file
2. $ echo 'hello git reset' > reset_lifecycle_file

2. $ git status 

On branch master 

Changes not staged for commit: 

(use "git add ..." to update what will be committed) 

(use "git checkout -- ..." to discard changes in working directory) 




- Staging Index

Հաջորդը «Բեմադրիչի ցուցիչ» ծառն է: Այս ծառը հետևում է աշխատանքային տեղեկատուի փոփոխություններին, որոնք առաջ են բերվել git հավելումով, որը պետք է պահվի հաջորդ պարտավորության մեջ: Այս ծառը ներքին պահեստավորման բարդ մեխանիզմ է: Git- ը սովորաբար փորձում է թաքցնել Staging Index- ի իրականացման մանրամասները օգտագործողից:

git ls-files -s ստուգում է stage index ծառի վեճակը

git ls-files -s
100644 e69de29bb2d1d6434b8b29ae775ad8c2e48c5391 0 reset_lifecycle_file

Այստեղ մենք իրականացրել ենք git ls- ֆայլեր –s կամ --stage տարբերակով: Առանց -s- ի տարբերակի, git ls- ֆայլերի ելքը պարզապես ֆայլերի անունների և ուղիների ցուցակ է, որոնք ներկայումս ինդեքսի մի մասն են: The- ի ընտրանքը ցուցադրում է լրացուցիչ մետատվյալներ ֆայլերի համար բեմականացման ինդեքսում: Այս մետատվյալները բեմականացված բովանդակության ռեժիմի բիտեր են, օբյեկտի անվանումը և փուլի համարը: Այստեղ մեզ հետաքրքրում է օբյեկտի անվանումը ՝ երկրորդ արժեքը 

 Git status հրամանի ելքը ցույց է տալիս փոփոխություններ cmmit history and stage index միջև:

- Commit history

The final tree is the Commit History. The git commit command adds changes to a permanent snapshot that lives in the Commit History. This snapshot also includes the state of the Staging Index at the time of commit.

***
## git remote

The git remote command is one piece of the broader system which is responsible for syncing changes.The git remote command is essentially an interface for managing a list of remote entries that are stored in the repository's ./.git/config file. The following commands are used to view the current state of the remote list.The git remote command is really just an easier way to pass URLs to these "sharing" commands.

- git remote

List the remote connections you have to other repositories.

- git remote -v

Same as the above command, but include the URL of each connection.

- git remote 'name' 'url'

Create a new connection to a remote repository. After adding a remote, you’ll be able to use <name> as a convenient shortcut for <url> in other Git commands.

- git remote rm 'name'

Remove the connection to the remote repository called <name>.

- git remote rename 'old-name' 'new-name'

Rename a remote connection from 

**repository URLs**
- HTTP
    - http://host/path/to/repo.git
- SHH
    - ssh://user@host/path/to/repo.git



**Showing your remotes**

- $ git remote
- origin
- upstream
- other_users_repo


- git remote -v
-     origin  git@bitbucket.com:origin_user/reponame.git (fetch)
-     origin  git@bitbucket.com:origin_user/reponame.git (push)
-     u pstream    https://bitbucket.com/upstream_user/reponame.git (fetch)
-     upstream    https://bitbucket.com/upstream_user/reponame.git (push)
-     other_users_repo    https://bitbucket.com/other_users_repo/reponame (fetch)
-     other_users_repo    https://bitbucket.com/other_users_repo/reponame (push).




## git fetch

The git fetch command downloads commits, files, and refs from a remote repository into your local repo. Fetching is what you do when you want to see what everybody else has been working on.When downloading content from a remote repo, git pull and git fetch commands are available to accomplish the task. You can consider git fetch the 'safe' version of the two commands. It will download the remote content but not update your local repo's working state, leaving your current work intact. git pull is the more aggressive alternative, it will download the remote content for the active local branch and immediately execute git merge to create a merge commit for the new remote content. If you have pending changes in progress this will cause conflicts and kickoff the merge conflict resolution flow.



**git branch -r**
- origin/master
- origin/feature1
- origin/debug2
- remote-repo/master
- remote-repo/other-feature


- git fetch 'remote' 

Fetch all of the branches from the repository. This also downloads all of the required commits and files from the other repository.

- git fetch <remote> <branch>
Same as the above command, but only fetch the specified branch.

- git fetch --all
A power move which fetches all registered remotes and their branches:


To see what commits have been added to the upstream master, you can run a git log using origin/master as a filter:  

- git log --oneline master..origin/master

To approve the changes and merge them into your local master branch with the following commands:

- git checkout master
- git log origin/master

Then we can use git merge origin/master:

- git merge origin/master

The origin/master and master branches now point to the same commit, and you are synchronized with the upstream developments.



***

## git push

**Git push usage**

- git push <remote> <branch>

Push the specified branch to <remote>, along with all of the necessary commits and internal objects. This creates a local branch in the destination repository. To prevent you from overwriting commits, Git won’t let you push when it results in a non-fast-forward merge in the destination repository.

- git push <remote> --force

Same as the above command, but force the push even if it results in a non-fast-forward merge. Do not use the --force flag unless you’re absolutely sure you know what you’re doing.

- git push <remote> --all

Push all of your local branches to the specified remote.

- git push <remote> --tags
Tags are not automatically pushed when you push a branch or use the --all option. The --tags flag sends all of your local tags to the remote repository.



git push is most commonly used to publish an upload local changes to a central repository. After a local repository has been modified a push is executed to share the modifications with remote team members.


     origin/master
           |
           |
O----------O----------O-----------O

                            |
                            |
                                Master





                            origin/master
                                  |
                                  |
O----------O----------O-----------O
                                  |
                                  |
                                Master


- git checkout master
- git fetch origin master
- git rebase -i origin/master
- Squash commits, fix up commit messages etc.
git push origin master

Since we already made sure the local master was up-to-date, this should result in a fast-forward merge, and git push should not complain about any of the non-fast-forward issues discussed above.

- git branch -D branch_name
- git push origin :branch_name


***

## git pull

[Git pull usage How it works](https://www.atlassian.com/git/tutorials/syncing/git-pull)


The git pull command is actually a combination of two other commands, git fetch followed by git merge. In the first stage of operation git pull will execute a git fetch scoped to the local branch that HEAD is pointed at. Once the content is downloaded, git pull will enter a merge workflow. A new merge commit will be-created and HEAD updated to point at the new commit.

- git checkout new_feature
- git pull < remote repo>

This example first performs a checkout and switches to the < newfeature> branch. Following that, the git pull is executed with < remote repo> being passed. This will implicitly pull down the newfeature branch from < remote repo>. Once the download is complete it will initiate a git merge.


                             



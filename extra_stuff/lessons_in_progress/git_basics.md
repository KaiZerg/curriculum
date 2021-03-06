## The Basics of how to use git
<!-- < In this blurb we should talk about what this lesson will include, the commands used here will be the ones you will probably
use the most with git etc -->

This lesson will demonstrate how to use git to manage and archive your project folders:

1. You will set up a remote repository on GitHub and then move it down onto your local machine. 
2. Once this repo is set up locally, you can begin writing code for your project and then saving it with git. 
3. When you have finalised your saves you can then push your local repo up onto GitHub to share with everyone!

Here is a reference list of commands you will need to know and remember:
* Commands related to remote repository:
  * `git clone https://github.com/user-name/repository-name.git`
  * `git push origin master`
* Commands related to workflow:
  * `git add .`
  * `git commit -m "A message describing what you have done to make this snapshot different"`
* Commands related to checking status or log history
  * `git status`
  * `git log`

The git syntax works like this: `program | action | destination`.

For example:
* `git add .` is read like `git | add | .`
* `git commit -m "message"` is read like `git | commit -m | "message"`
* `git status` is read like `git | status | (no destination)`





## Learning Outcomes
*By the end of this you should be able to:*
* Create a Git repository on GitHub and move it onto your local machine
* Describe the difference between staging and committing changes
* Describe the difference between committing your changes and pushing them onto GitHub
* Check the status of your current repository from the command line
* Look at the history of your previous commits from the comamnd line
* Look at the history of your commits on the GitHub website





## Assignment:
<!-- This assignment is really good, no need for anymore -->
<!-- Since this assignment only has one resource, cs-rail has decided to remove the '1' bullet point - bullet points are already loaded in the intro blurb -->
[Try Git from codeschool](https://try.github.io/levels/1/challenges/1).
Follow the exercises up to and including "1.11 Pushing Remotely" then jump back here.





## Basics of git tutorial
<!-- msg for kevinmulhern: Hey could you please include in your workflow instructions making a repo on GitHub? (untick initialize README) -->

Here we will describe the basic git workflow that you will use with your projects, feel free to follow along with this
<-- screen shots will be provided!->

1. Created a new folder called git_test and add a file called hello_world.txt
2. to initialize git we use `git init` this creates a hidden folder called .git/ where configuration settings for git will be stored
3. type `git status in your terminal` notice your hello_world.rb file is in red, this means it is un-staged.
4. type `git add hello_word.txt` this adds your hello_world.txt file to staging area in git.
5. now type `git status` again, notice your file is now green.
6. now type `git commit -m "Initial commit"` and type `git status again` notice it now outputs "nothing to commit" your changes have been committed.

##How does git save files?
A *save* in git is divided into two terminal commands: **add** and **commit**. The combination of these two commands gives you control of exactly what you want to be remembered in your snapshot.


###The staging Area
Think of `add` as adjusting the number of people or elements to be included in your photo.

With Git you choose the changes you want to save with `git add`. Imagine a project that contains multiple files and you have made changes to several of them. You want to save some of the changes you have made and leave some other changes to continue working on them.

###Committing
Think of `commit` as actually taking the photo, resulting in a snapshot.

We used this command to commit the hello_world.txt file `git commit -m "Initial commit"` the `-m` flag stands for message and must always be followed by a message in quotes in our case `"Initial commit"`.




#todo in the next part we will edit the file again and add another file to repeat the basic commands so the student can get used to them
Now we will add another file into the mix.

7. Create a new file in the `git_test` folder and call it `hello_mars.txt`.
8. In your terminal and type `git status`, notice `hello_mars.txt` is un-staged.
9. Now open the `hello_word.txt` in your text editor of choice and add "Inside the hello world file".
10. Back in your terminal enter `git status`, notice that `hello_word.txt` is now un-staged again.
11. Add `hello_word.txt` to the staging area with `git add hello_word.txt`
12. Can you guess what `git status` will output now? `hello_word.txt` will be displayed in green text and `hello_mars.txt` will still be in red. This means only `hello_world.txt` has been added to the staging area.
13. Now lets add `hello_mars.txt` to staging area with a different variation of add `git add .` this full stop means add all un-staged files.
14. Enter `git status` once more, everything has now been added to the staging area.
15. Finally lets commit all of our changes `git commit -m "Added hello mars file and added a line to hello world"`
16. Enter `git status` once more, nothing to commit.


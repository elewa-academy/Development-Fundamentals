# (De)bug-off

Yet another never-ending project.  Only this one is a game. 

A Player can ...
* On their repo:
  * Post a new debug challenge
  * Assign a challenge to another player(s)
  * Accept, reject, or ask for changes to proposed fixes
* On another player's repo:
  * Accept a challenge (Fork it)
  * Create a bug fix
  * Categorize the bug fix
  * Submit their solution (Pull Request)
  * Be notified if their fix was selected or not

There are no winners or losers in this game because it never ends.  You should continue to send each other harder and harder debug challenges as the course goes on.  (If the game did end there would be winners and losers.)  

Not only is this game fun, but it's educational! By the time you've been playing for a week or two you will have a reference filled with useful information on debugging.

### Index
* [Learning Objectives](#learning-objectives)
* [Specifications](#specifications)
* [Resources](#resources)

---

## Learning Objectives

* De-Bugging
* Categorizing Bugs
* De-Bugging Tools
* Issues
* Branching
* Pull Requests
* GitHub Projects
* GitHub Notifications


[TOP](#index)

---

## Specifications

### __Set-Up:__
```
A (De)bug-off repo:
|-- /zzz-challenges
|	|-- challenge.js
|	* place your challenges here
|
|-- /category-x
|	|-- challenge-fix.js
|	|	* other players send "fix" files in their pull requests
|	* other players will either place a "fix" in an existing category
|	 	or propose a new category of bug along with their "fix"
|	* you can accept, reject, or ask for changes to pull requests
|
|-- README.md
```
```
A (De)bug-off gallery:
* Repo boxes:
  * Link to repo code
  * Link to repo project
  * The user's github image
  * Who challenged who (for others' repos)
* Link to gallery repo's project for keeping score:
  * A column per user who challenged you & accepted your fix:
    * A note linking to their project
    * An issue linking to each merged PR & it's issue
```
1. Create an empty (De)bug-off repo
2. Create a new project in that repo
3. Create 4 columns in the project
   * Challenges
   * Submitted Submissions
     * Automation: _new pulls & issues_
   * Accepted Submissions
     * Automation:  _merged pull requests_
   * Rejected Submissions
     * Automation: _unmerged pull requests_
4. Create a (De)bug-off Gallery
5. Set up your score board
  


### __Game Play:__

__Posting a Challenge:__
1. Place a new JS file with buggy code in your challenges folder
2. Open an issue named after that file
3. Link to the file in the description 
    * Don't give any hints about the bug!
4. Challenge other players by assigning the issue to them
5. Place the issue in the "challenges" column of your project

__Accepting a Challenge:__
1. Pull the challenger's master branch to avoid conflicts
2. Create a new branch named after the challenge 
3. Write and categorize your fix:
    * xyz-fix.js:
      1. Link to the challenge issue
      2. Buggy code, commented out
      3. Your fix
      4. Test cases you used
      5. Description of the bug and how you fixed it
    * Place the fix in an existing or new category directory
4. Send a pull request:
    * Name it after the challenge you accepted
    * Provide a nice helpful comment
    * Mention the issue number in your comment (ie. #4)
5. Cross your fingers and wait

__Selecting a winner(s):__
1. Check incoming pull requests, move them to the project
2. Find all pull requests related to your challenge:
    * Either by their title
    * Or by opening the challenge issue and selecting them there
3. Read through them all and pass judement:
    * Merge them if you like the fix & the categorization
    * Close them if you really don't like it
    * Leave them a note if you have a question or want something changed

__Updating Your Score:__
* You will recieve a notification telling you if your fix was merged or not
* If your fix was merged, update your scoreboard (Gallery project):
    * Create a new issue in that user's column
    * Provide a link to the challenge & your pull request




[TOP](#index)

---

## Resources

GitHub:
* [Creating Folders from GitHub](https://stackoverflow.com/questions/18773598/creating-folders-inside-github-com-repo-without-using-git)

Debugging:
* [Rithmschool Exercises](https://www.rithmschool.com/courses/intermediate-javascript/javascript-debugging-exercises)
* [DevMountain Exercises](https://github.com/DevMountain/debugging-exercises)

[TOP](#index)



___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>

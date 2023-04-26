# GitHub_HW_2

1. Make branches on the local repository:
+ `git branch Postman`
+ `git branch Jmeter`
+ `git branch CheckLists`
+ `git branch Bag_Reports`
+ `git branch SQL`
+ `git branch Charles`
+ `git branch Mobile_testing`
2. Push all branches to an external repository
+ `git push -u origin --all`
3. In the Bag Reports branch, make a text document with the bug report structure
+ `git checkout Bag_Reports` - go to the branch _Bag_Reports_
+ `cat > BagReport_structure.txt`
+ Enter data:
```
Summary
Priority
Severity
Status
Environment
Descriprion
  Precondition
   Steps to Reproduce
   Actual Result
   Expected Result
 Attachment
 Assignee
 Reporter
```
+ `ctrl+c` - get out of editing
4. Push the bug report structure to an external repository
+ `git add .; git commit -m "new file"; git push`
5. Merge branch _Bag Reports_ to _Main_
+ `git checkout main` - go to branch _main_
+ `git merge Bag_Reports` - merge a branch _Bag_Reports_ to _main_

or one line

+ `git checkout main; git merge Bag_Reports`
6. Push _main_ to the external repository.
+ `git push -u origin main`
7. In the branch _CheckLists_ outline the structure of the checklist.
+ `git checkout CheckLists` - go to the branch _CheckLists_
+ `cat > CheckList_structure.txt`
+ Enter data:
```
ID
Title
Precondition
Module
Steps_to_reproduce
Expected_result
Status
```
+ `ctrl+c` - get out of editing
8. Push structure to external repository
+ `git add .; git commit -m "new file"; git push`
9. On an external repository do Pull Request branche _CheckLists_ to _main_
+ Go to https://github.com/ to the repository
+ Go to tab _Pull Request_
+ Press the button _`New pull request`_
+ base branch _`main`_ <-- compare branch _`CheckLists`_
+ Press _`Create pull request`_
10. Synchronize External and Local branches _Main_
+ `git checkout main; git pull`

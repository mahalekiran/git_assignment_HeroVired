# git_assignment_HeroVired
Q1. Steps Performed
1. Created a repository name: git_assignment_HeroVired in github.com
2. cloned the project in local. and open in VS code.
3. created dev branch using git branch dev
4. Created CalculatorPlus.py file and added the code
5. Commit and push code in dev
git add .
git commit -m "adding dev files calculatorplus code"
git push origin dev
6. merge code from dev to main. Here a relase to b e reated. but forgot to do it.I have created release 1 after bug fixation.
git checkout main
git pull origin dev
git merge dev
git push origin main
7. Added Prem Kumar as collaborator
8. created feature branch 
git branch feature/sqrt
9. Switched to this branch
git switch feature/sqrt
10. Added sqrt code.
11. Before switching to dev to fix bug. Commit feature changes tht has been modified by git add and git commit.
12. then switch to dev branch using git switch dev.
13. Modify divide function by adding fix. commt and push code on dev. 
14. switch to main branch.merge dev changes for bug fixation.
15. again come to feature branch and work on it. push the code.
16. Ceate pull request. Add Reviewer. ask them to review. Merge feature branch to dev branch.
17. Testing on dev branch after puling the code.
18. Merge dev to main branch. and make a release 2.
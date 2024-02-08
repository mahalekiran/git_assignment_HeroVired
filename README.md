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


Q2. Git LFS
1. Create a branch lfs using 
git banch lfs
git switch lfs
2. Add large file. zip file here
3. install git lfs
git lfs install
4. track lfs
git lfs track "*.zip"
git lfs track "*.iso"
5. Add commit push large files
git add .\bluetooth_applications-22.zip
git commit -m "Add files using Git LFS"
git push origin lfs
6. On Second Machine, cloned the project. 
git switch lfs
git lfs pull

Q3. Stash usage
1. First created geometry-calculator branch and added the code
git checkout -b geometry-calculator
add python file GeometryCalculator.py and write the code
2. Commit the code in this branch
 git commit -m "Created file with Geo calculator code"
3. Create a new branch named "feature/circle-area" to work on the circle area feature
git checkout -b feature/circle-area
python .\GeometryCalculator.py 
4. Stash Changes for Circle Area Feature and Verify working directory
git stash save "Circle Area Feture Implementation"
git status
5. Create a New Branch for Rectangle Area Feature:
git checkout -b feature/rectangle-area
python .\GeometryCalculator.py
6. Stash Changes for Rectangle Area Feature and verify working directory
git stash save "RectangleArea Feature Implementation"
git status
7. Switch Back to Circle Area Branch:
git checkout feature/circle-area
8. Retrieve stashed changes
git stash list
git stash apply stash@{1}
9. make implementation and commit and push changes to this feature: circle
git add GeometryCalculator.py
git commit m "Completed Circle feature"
git push origin feature/circle-area
10.  Switch Back to Rectangle Area Branch:
git checkout feature/rectangle-area
11. Retrieve stashed changes
git stash list
git stash apply stash@{0}
12. make implementation and commit and push changes to this feature: rectangle
git add GeometryCalculator.py 
git commit -m "Completed Rectangle feature"
git push origin feature/rectangle-area
13. Created Pull Requests for both features to dev branch.
Added reviewer Prem Kumar.
After approval. Merged the code to dev branch.
14. Created another pull request to merge code from dev to main branch without reviewer.
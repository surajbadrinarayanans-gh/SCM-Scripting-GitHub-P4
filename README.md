# SCM (GitHub) Project:

---



![1773651537299](image/README/1773651537299.png)

#### Step 1 - Creating Project Folder Structure:

![1773639887297](image/README/1773639887297.png)

Adding sample contents to all the files.

![1773640313770](image/README/1773640313770.png)

Adding all the files to staging area, committing them and pushing it to GitHub for the inital project folder setup.

![1773640381475](image/README/1773640381475.png)

Pushing the contents to the GitHub repository.

![1773640464865](image/README/1773640464865.png)

---

#### Step 2 - Creating Development Workflow:

- main → production
- dev  → integration branch
- feature branches → development work

![1773640992750](image/README/1773640992750.png)

Creating a dev branch and pushing the code contents and folders to the dev branch.

![1773641036135](image/README/1773641036135.png)

---

#### Step 3 - Simulating the Feature Development:

Situation:

There are 2 developers A and B. they will be working on separate feature branches.

For developer A:

![1773641461253](image/README/1773641461253.png)

![1773641511537](image/README/1773641511537.png)

Modifying the configuration file.

![1773641718911](image/README/1773641718911.png)

Adding, commiting and pushing only that configuration file.

Even though the entire folder structure appears in the feature branch (because of the initial git add. for the project folder structure initialisation) the feature-branch only containes the config file commit snapshot.

![1773641926780](image/README/1773641926780.png)

Checking out to a new feature branch to Developer B.

![1773642783114](image/README/1773642783114.png)

Adding, committing and pushing changes to the main folder feature branch.

![1773642749856](image/README/1773642749856.png)

![1773642717128](image/README/1773642717128.png)

After merging the changes of the configuration feature branch the dev branch is now updated with that feature.

---

#### Step 4 - Second Feature Development (Merge Conflict):

![1773645226527](image/README/1773645226527.png)

![1773645776777](image/README/1773645776777.png)

Creating a feature branch to demonstrate merge conflicts.

- A new feature branch modified the main.txt file.
- A developer in the dev branch also modified the same file.
- Both tried to modify the same file before merging so the conflict occured.

What should have done actually?

- A new feature must be merged to the dev branch first.
- The dev branch must be pulled and should be made upto date.
- Then the other developer should enhance the file again, push it and merge it so that the conflict does not happen.

![1773646139368](image/README/1773646139368.png)

---

#### Step 5 - Cherry Picking:

![1773646734225](image/README/1773646734225.png)

Consider the test feature branch with 3 experimental commits.

![1773646886349](image/README/1773646886349.png)

![1773646873075](image/README/1773646873075.png)

Switching to the config branch and seeing the contents of the main.txt file.

![1773646973599](image/README/1773646973599.png)

![1773646986997](image/README/1773646986997.png)

---

#### Step 6 - Hotfix:

![1773650734504](image/README/1773650734504.png)

Creating a hotfix branch and pushing the hotfix to the hotfix branch.

![1773650909160](image/README/1773650909160.png)

Merging the branch again to main so that the hotfix feature is reflected in the main branch.

Now the main branch only contains the changes of the hotfix branch and not the dev branch so we need to sync the hotfix to dev branch also.

![1773651124199](image/README/1773651124199.png)

Once the production is stable, we delete the hotfix branch locally and remotely.

![1773651185636](image/README/1773651185636.png)

---

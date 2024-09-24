# Explore NetBox Branching

Follow these steps to get familiar with Branching in NetBox

1. In the Web UI main menu, navigate to **Branching** > **Branches** and click on the plus sign to add a new branch.
2. Name the new branch `New Site - Lisbon`, and give it a description of `New site deployment - Lisbon, Portugal`, and then click **Create**.
3. Note that the **Status** is `Provisioning` and then if you refresh, you will see it change to `Ready`.
4. Make the new branch active, by clicking **Activate** and note that the active branch name in the top-right corner has now been updated.
5. Make changes in the branch - add a new `Site` called `Lisbon` and a new rack called `POLIS01-RK-01`
6. Navigate to **Branching** > **Branches** and click on the name of the new branch. Explore the **Diff** and **Changes Ahead** tabs
7. When you are happy with your changes, click on **Merge** tick the box to commit the changes to the database click **Merge Branch**.
8. Refresh and note that the **Status** is now `Merged` and the branch is no longer active, but you can still view the branch under the **Branching** menu.
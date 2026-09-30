1. Why did merging update-message-b cause a conflict, but merging update-message-a did not?

Because update-message-a preserved the print and the variables, so the reference of original print vs update-message-a didn't raise any conflicts whereas in update-message-b we're rewording already existing version of the print message. 

2. In the conflict markers, what does the section under HEAD represent? What does the section under the branch name represent?

HEAD shows what's in the branch we're trying to merge the update-message-b with and the section under branch name is what the upcoming changes want to write in the given lines.

3. What command would abort a merge in progress if you decided not to resolve it? (Look up git merge --abort.)

git merge --abort aborts the merge in progress, keeping the pre-merged state of the last commit/merge in the HEAD

4. How does the git log --graph shape from Part C differ from the one in Part B? Why?

part B had a single line while part C had two have two lines rejoined because of the merging conflicts caused by update-message-b
What is this project ?
----------------------

This project is **NOT** the official BRAINSTools repository.

It is a fork of BRAINSTools sources hosted at https://github.com/BRAINSia/BRAINSTools.

It is used as staging area to maintain and test patches that will be contributed back to the
official repository.


What is the branch naming convention ?
--------------------------------------

Each branch is named following the pattern `slicer-vY.Y.Z-YYYY-MM-DD-SHA{7}`

where:

* `vX.Y.Z` is the version of the forked project
* `YYYY-MM-DD` is the date of the last official commit associated with the branch.
* `SHA{7}` are the first seven characters of the last official commit associated with the branch.

For more details, see https://www.slicer.org/wiki/Documentation/Nightly/Developers/ProjectForks


How to update the version of BRAINSTools ?
------------------------------------------

1. Clone this repository and add a remote to the official project

```
git clone git://github.com/Slicer/BRAINSTools
cd BRAINSTools
git remote add upstream git://github.com/BRAINSia/BRAINSTools
git fetch upstream
```

2. Create a new branch following the convention `slicer-vY.Y.Z-YYYY-MM-DD-SHA{7}`

3. Cherry-pick the Slicer specific commits from last branch. Resolve conflict as needed.

4. To **test the changes**, locally rebuild Slicer.

5. Publish the branch. (directly in this repo if you have push rights, or on a fork)

6. Update Slicer BRAINSTools external project and submit a pull request.


How to be granted push rights ?
-------------------------------

Ask on https://discourse.slicer.org/


Questions
---------

If you have questions, see https://discourse.slicer.org/


Alright guys. There it is:
1. Install this https://www.git-scm.com
2. Instal that https://tortoisegit.org
3. Go to /CRYENGINE Launcher/Crytek/
4. Right-click and choose Git Clone...
5. In URL field paste this address:
https://github.com/fury22pl/WW2-MMO-Public
6. Press OK and wait until it downloads all the files

Your repository is equal with our mutual repository in github now.

Open Cryengine Launcher now and go to Library -> My Projects and in right up corner you hit "Import", find your repository (/Crytek/WW2-MMO-Public), highlight it and press Ok
That's it. Your project is ready now!

Now... What do you do if you have made any changes, or you have created new files to the project (3d models etc, whatever).
Once your changes are ready to public for the rest of the team, there are two ways.

1.If you have changed already existing files:
   - Inside Crytek/WW2-MMO-Public/ right-click
   - Git Sync...
   - Remote Branch must be set to "test" (without quote marks)
   - Press "Push", it should load your files into github repository.

2. If you add any new files:
   - /Crytek/WW2-MMO-Public/ right-click
   - Git Sync...
   - Remote Branch : test
   - Commit 
   - On the list you'll see new files. Check the box next to each file you want to push to github. 
   - On the top you have texfield "Message". Add some short comment about what files you upload and why. It will make our cooperation much easier.
   - Hit "Commit" and wait until it loads your files
   - This will update only your repository, to push it to our mutual github repository, go to step 1 - already existing files.

Now... What to do if someone else updated our repository on github, and you want to be up-to-date?

1. If you want to completely replace your repository by our github repository:
   - /Crytek/WW2-MMO-Public/ right-click
   - Git Sync...
   - Remote Branch : master (we are going to use master to update our repositories. I will keep merging test branch with master branch, just to keep it tidy. Master branch will be used as a working project)
   - Hit "Pull"
   !!! Note that this will REMOVE all your new files, that are not the same as in repository!!!

2. If you want to merge repository with github repository (this will be something we'll use the most of time)
   - /Crytek/WW2-MMO-Public/ right-click
   - Git Sync...
   - Remote Branch : master
   - On the "Pull" button you'll see an arrow. Hit it and choose "Fetch"
   !!!This will replace existing files with the files from github without deleting your new files!!!



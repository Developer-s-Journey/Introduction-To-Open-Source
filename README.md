## Introduction-To-Open-Source :octocat:

Our open source community is focused on helping everyone get started with Open Source.

## Steps to follow :scroll:

### 1. Fork it :fork_and_knife:

You can get your own fork/copy of [Introduction-To-Open-Source](https://github.com/HeroicHitesh/Introduction-To-Open-Source) by using the <a href="https://github.com/HeroicHitesh/Introduction-To-Open-Source/new/master?readme=1#fork-destination-box"><kbd><b>Fork</b></kbd></a> button.

 [![Fork Button](https://help.github.com/assets/images/help/repository/fork_button.jpg)](https://github.com/HeroicHitesh/Introduction-To-Open-Source)

### 2. Clone it :busts_in_silhouette:

Now that you forked `Introduction-To-Open-Source` repository, you need to clone (download) it to your local machine using

```sh
$ git clone https://github.com/Your_Username/Introduction-To-Open-Source.git
```

> This makes a copy of repository on your local machine(simply saying, your PC).

Once you have cloned the `Introduction-To-Open-Source` repository to your local machine, move to the folder created using change directory command on linux / Windows / Mac.

```sh
# This will change directory to a folder Introduction-To-Open-Source
$ cd Introduction-To-Open-Source
```

Move to this folder to perform all future commands.

### 3. Set it :up:

Run the following commands to confirm that *your local copy* has a reference to *your forked remote repository* in Github 

```sh
$ git remote -v
origin  https://github.com/Your_Username/Introduction-To-Open-Source.git (fetch)
origin  https://github.com/Your_Username/Introduction-To-Open-Source.git (push)
```

Now, lets add a reference to the original [Introduction-To-Open-Source](https://github.com/HeroicHitesh/Introduction-To-Open-Source) repository using

```sh
$ git remote add upstream https://github.com/HeroicHitesh/Introduction-To-Open-Source.git
```

> This adds a new remote named ***upstream***.

View the changes using

```sh
$ git remote -v
origin    https://github.com/Your_Username/Introduction-To-Open-Source.git (fetch)
origin    https://github.com/Your_Username/Introduction-To-Open-Source.git (push)
upstream  https://github.com/HeroicHitesh/Introduction-To-Open-Source.git (fetch)
upstream  https://github.com/HeroicHitesh/Introduction-To-Open-Source.git (push)
```

### 4. Sync it :arrows_counterclockwise:

Always keep your local copy of repository updated with the original repository.
Before making any changes and/or in an appropriate interval, run the following commands **carefully** to update your local repository.

```sh
# Fetch all remote repositories and delete any deleted remote branches
$ git fetch --all --prune

# Switch to `master` branch
$ git checkout master

# Reset local `master` branch to match `upstream` repository's `master` branch
$ git reset --hard upstream/master

# Push changes to your forked `Introduction-To-Open-Source` repo
$ git push origin master
```

### 5. *Git* Set Go... :racehorse: :loudspeaker:

Once you have completed above steps, you are ready to start contributing to open source by checking Issues with `Help Wanted` tag and creating PRs.

Whenever you are going **to make contribution**. Please, create a *new branch* using following command and keep your `master` branch clean (i.e. synced with remote branch).

```sh
# It will create a new branch with name Branch_Name and switch to branch Folder_Name
$ git checkout -b Folder_Name
```

Create a separate branch for contibution and try to use same name of branch as of folder.

To switch to desired branch

```sh
# To switch from one folder to other
$ git checkout Folder_Name
```

To add the changes to the branch. Use

```sh
# To add all files to branch Folder_Name
$ git add .
```

Type in a message relevant for the code reveiwer using

```sh
# This message get associated with all files you have changed
$ git commit -m 'relevant message'
```

Now, Push your awesome work to your remote repository using

```sh
# To push your work to your remote repository
$ git push -u origin Folder_Name
```

Finally, go to your repository in browser and click on `compare and pull requests`.
Then add a title and description to your pull request that explains your precious effort.

## Help us IMPROVE :crown:

We love to have `articles` and `codes` in different languages to `improve` existing ones.

Please discuss it with us first by creating new issue.

:tada: :sparkles: :smile: _**Happy Contributing**_ :smile: :sparkles: :tada:

Hello. I'm Wilson Mar.
I've struggled to create an <a href="#MyMap">animated illustration</a> 
so you can quickly grasp Git's basic workflow and commands.

I call my diagram the "fearless" approach 
because I introduce Git in more depth and in a different sequence 
than other tutorials that have come before me.

I thank <a target="_blank" href="http://zeroturnaround.com/rebellabs/git-commands-and-best-practices-cheat-sheet/">
ZeroTurnaround</a> for this diagram.


<a name="MyMap"></a>

## My map #

I use a <strong>map</strong> of how key files and commands relate to each other.
It's the only one of its kind I've seen.

   PROTIP: You are encouraged to pull out a paper and hand-draw 
   the diagram as we go along.

> Please let me know if you can see a tweak to this sequence for better introduction of concepts.

Let's begin with repositories in a cloud service, GitHub.com.
A repo that belongs to another organization is called an <strong>"upstream"</strong> location.
If we <strong>edit</strong> that repo, 
GitHub automatically <strong>forks</strong> it under our own account.
If we want to make changes, we would need to file a 
<strong>Pull Request</strong> from the repo under our account.

One to the main advantages of GitHub is it makes use of <strong>branches</strong>.
The default branch is named "master".
But many organizations use it for production 
and create a <strong>"developer"</strong> and other branchs to do work.

I can click the <strong>Download</strong> button to 
bring a zip file to my local Downloads folder,
which I then <strong>unzip</strong> to folder I created.

But that folder alone does not keep back versions.
For that we need a <strong>.git</strong> folder among the files,
which is done by a <strong>Git client</strong> 
installed on my local machine.

The git <strong>init</strong> command processed by the Git client
creates the git folder to hold the history of changes it recognizes.
The git <strong>clone</strong> command which creates a new folder
to download files from GitHub and in that new folder
also creates the .git folder to hold historical references.

If we run the SSH or Putty command to create keys,
the Git client can communicate securely with the cloud service.

We need to run <strong>config</strong> commands to 
configure the <strong>.gitconfig</strong> file
referenced by all Git repositories on our machine
to provide our default name and email address to repos.

We can clone from an upstream repo, 
but it's preferable that we first fork any repo if we ever want to
send a Pull Request.

If we do a <strong>remote -v</strong> command on a repo we cloned,
we see that <strong>origin</strong> is the location.
If we need to update our local repo with changes in the upstream repo,
we would <strong>remote add</strong> the upstream.

Git only tracks files involved in a git <strong>commit</strong> 
command. Git stores what has changed in the .git folder
and calculates a reference to each particular change.

The git <strong>tag</strong> command allows a 
custom name of your choosing to be assigned to a commit.
Teams use this to specify release numbers and
specifications which Jenkins recognizes to invoke integration builds.

The git <strong>shortlog</strong> summarizes the history of commits made.

The git <strong>log</strong> command lists a 
<em>detailed</em> history of all commits made.
Most consider its default format takes up too many lines,
so many configure in the .gitconfig file an alias 
such as <strong>lol</strong> to format what gets displayed.

BTW, <strong>"HEAD"</strong> refers to the most current commit,
listed at the top of a chain of its <em>descendants</em> prior commits.

The git <strong>reflog</strong> command lists the history of 
<em>all</em> changes made in the sequence they occurred,
like an undo history of the repo. 
It's stored separately from the commits themselves
and isn't included in pushes, fetches or clones
because it's purely for local use. 

PROTIP: understanding the reflog means you can't really lose data from what has been committed. 
If you accidentally reset to an older commit, or rebase wrongly, or any other operation that visually "removes" commits, you can use the reflog to see where you were before and git reset --hard 
back to that ref to restore your previous state. 

git <strong>log</strong> shows the current HEAD and its ancestry. 
That is, it prints the commit HEAD points to, then its parent, its parent, and so on. 
It traverses back through the repo's ancestry, by recursively looking up each commit's parent.


The git <strong>show</strong> command lists fine-grained individual
<em>objects</em> in the repository, such as blobs and trees
as well as tags and commits.

<hr />

The git <strong>branch</strong> command lists what branches 
are in the local repository because only a specific branch
may be cloned locally.

A git <strong>checkout</strong> command can specify a
specific branch or commit version to be brought into the working folder.

A parameter in the checkout command can also specify the creation of a new branch
based on a previous branch.

This will put you in what Git calls a "detached HEAD" state.

<hr />

Bash command <strong>touch</strong> and <strong>echo</strong> 
can create and change files,
but in order for them to be committed for tracking by git,
they first must be specified in a git <strong>add</strong> 
command which puts changes in a sort of "shopping cart" called the 
<strong>staging</strong>, which is also called <strong>Index</strong>
because it holds an index of files which the
next git commit command would track.

The git <strong>status</strong> command shows
which files have been <strong>staged</strong>
or remain <strong>untracked</strong>.

When Git detects a staged file has been 
<strong>edited</strong> by a text editor,
Git automatically takes that file out of staging
and assigns it the status of <strong>modified</strong>.

<hr />

Git provides a way to stash the state of files in the working directory and index
so they are not lost forever when you have to 
suddenly switch back to the state in the HEAD commit.

The <a target="_blank" href="https://git-scm.com/docs/git-stash">
git <strong>stash</strong></a> command (with implicit save)
puts all files from the working directory
into a local stash area separate from Staging or the Git repository.

The modifications stashed can be listed with git <strong>stash list</strong>, 
inspected with git <strong>stash show</strong>, 
and restored (potentially on top of a different commit) 
with git <strong>stash apply</strong>. 

To get rid of what's in the stash, do a git <strong>stash drop</strong>.

<hr />

To remove files from staging,
Git command <strong>reset HEAD --</strong> can be used 
followed by a file specification, which can be a dot to specify all files.

To remove all files in the <em>working directory</em>
which are NOT under version control, using the
git <strong>clean</strong> command, which works 
<em>recursively</em> down the various sub-folders.

To wipe out all uncommitted changes in staging and 
replace the working tree with the commit HEAD specified, use
Git command <strong>reset --hard HEAD^</strong>.

<hr />

After a commit, the status command would show no files, except
files <strong>deleted</strong> after being committed would 
appear as status deleted.
Such a file can be retrieved using the
git <strong>checkout</strong> from repository history.

If the <em>description</em> of the <em>most recent</em> 
local commit needs to be changed,
<a target="_blank" href="https://help.github.com/articles/changing-a-commit-message/">
it can be done</a> using a <strong>commit --amend</strong> parameter.

To change the content of the most recent commit,
a <strong>revert</strong> command can be used to
create another commit which does the opposite of what is being reverted.

Changing previous commits would require a git "push --force" command,
which is not allowed in most organizations because it requires
others who have cloned the repo to make manual changes.

But while you're still working on a local branch, you can use
git <strong>rebase</strong> to reword commit messages or
<em>squash</em> several commits into one.
This is desirable especially for commits that only fix typos in the local repo
which other do not really want to know about.

<hr />

When working in a team, changes may have occcurred while you're 
working with an older version.

Many tutorials talk about using the <strong>pull</strong> command
to obtain updates from the origin or upstream location.

But we prefer using the <strong>fetch</strong> command which,
unlike pull, does not automatically do a 
<strong>merge</strong>.

The <strong>diff-tree</strong> has a similar command set
as the git show command.

We want to use a git <strong>diff</strong> command or use a 
<strong>diff-tool</strong> to examine what has changed,
then run merge manually or using a
<strong>merge-tool</strong>.

We want to check whether changes have occured before doing a
git <strong>push</strong> of local commits to the team repository in the cloud.





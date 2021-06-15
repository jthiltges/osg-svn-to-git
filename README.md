svn-to-git
==========

Mirror a repo from Subversion to Git using `git svn`

# Environment variables

## Required

* `SVN_BASE` - Subversion base URL. Ex. `https://example.edu/svn`
* `SVN_PATH` - Subversion path. Ex. `native/redhat`
* `GIT_DEST` - Destination git URL. Ex. `git@github.com:opensciencegrid/mirror.git`
* `AUTHORS_URL` - URL to retrieve the git-svn authors-file. Ex. `https://example.edu/authors.txt`
* `WORK_DIR` - Persistent working volume. Ex. `/data/mirror`

## Optional

* `GIT_SSH_COMMAND` - Allow SSH key path to be specified. Ex. `ssh -i /secrets/id_rsa`
* `SLEEP_ERR` - Sleep on error for easier CronJob debugging. Ex. `15m`

### Connections
$ ssh-agent
$ ssh -T git@github.com
$ ssh wkchung@abigail.iis.sinica.edu.tw
$ git status:                   check current tracked/untracked files
$ git add <file>:                 add a file to git for tracking. (status become: "Changes to be committed")
          -A (-all):            add all files under the current path to git for tracking.(status become: "Changes to be committed")
$ git reset                     reset git status.
# Note: if you remove a file and hope to syncrinize to GitHub, use 'rm' or 'add -u' instead of 'add'. #
$ git rm <file>:              Tells git that the file will be removed and waited to be committed. 
$ git add -u (--update):        add all modified & deleted files and waited to be committed.
$ mkdir <directory_name>:     create a new directory under the current path
$ mkdir <D1/D2/D3>:               Assuming that the path ~/D1/D2 already exists. create a new directory D3 under that path.
$ mkdir -p <D1/D2/D3>:            Checking existing path and create path if no such directory.
$ (git) mv <file> <directory>:  (tells git that we) move a file into the target directory.
$ (git) mv <file> <new_name>:   (tells git that we) rename a file.
$ git clone <ssh/https web>       clone remote repository to the local.
$ git commit:                   commit a patch. (enter into vim mode to edit commit message.)
$ git commit -m <title>:      commit only with title without entering vim.
$ git commit -m <title> -m <msg1> (-m <msg2>...): commit with title and message without entering vim.             
$ git log:                      show all commit histroy.
$ git show:                     show last submittied patch.
$ git show <commit id>:           show corresponding submittied patch. 
$ git diff <file>:                show revised content of the file. (can only show contents with status "Changes not staged for commit ")
$ git diff --cached (--staged): show revised content fo the file. (also include contents with status "Changes to be committed")
$ wget <http://...>               clone data into current directory.
$ tar -zvxf <file.zip (file.gz)>  ucompress file.
$ jobs                          list all jobs.
$ jobs -r                       list running jobs.
$ jobs -s                       list suspended jobs.
Branch command
$ git status                    list all tracked files and untracked and committed-not-push files under CURRENT directory.
$ git branch:                   show all branches
$ gitk --all &:                 show all branches using gitk graphical interface. '&' means run gitk at background.
$ git branch <new_branch>:        construct a new branch.
$ git checkout <branch>:      switch from current branch to target branch.
$ git pull
$ git push
### Tmux command
prefix key for tmux: Ctrl + a 
$ tmux                                              start new session
$ tmux new -s <name>                                  the current screen starts to be supervised by tmux (new tmux session with a name)
$ tmux ls                                           show all tmux sessions
$ tmux a (or at, or attach)                         attach to a tmux window.
$ tmux attach -t <no.>(<name>)                      attach to tmux session by number <no.> or by name <name>
$ tmux rename-session -t <target w> <changed_name/no.>  rename target session by a new number or new name.
$ tmux display-message -p                           show current active window number or name.
$ tmux kill-session -t <name>                     kill tmux session.
$ prefix + d                                        Detach current session. Use tmux attach if you want to attach back to the session.
$ prefix + s                                        switch to other session
$ prefix + %                                        open new pane horizontally on the same window.
$ prefix + \" (only quote)                         open new pane vertically on the same window.
$ prefix + Arrowkey (↑ ↓ ← →)                       move to other pane.
$ prefix + x                                        close current pane under current window.
$ prefix + c                                        open new window.
$ prefix + &                                        close current window.
$ prefix + p                                        switch to previous window.
$ prefix + n                                        switch to next window.
$ prefix + :                                        tmux command prompt mode.
: move-window -s <src w no.> -t <tar w no.>         move window from a number to another number.
### Pip (or Pip3 for Python3.x) command
$ pip3 -v                                           show the current version of pip
$ pip3 -h (help)                                    show pip commands
$ pip3 install [options] <package>                    install package
$ pip3 install [options] <package> -i httP://...  Specify particular package source to be installed
$ pip3 uninstall [options] <package>              uninstall package
$ pip3 install -U (--upgrade) [options] <package> update package
$ pip3 install -U pip                               update pip
$ pip3 list                                         list installed packages
$ pip3 freeze                                       list all installed packages
$ pip3 freeze | grep [options] <package>          list the version of target package
$ pip3 list --outdated                              list all oudated packages
$ pip3 show [options] <package>                       show datail information of the package
$ pip3 show --files [options] <package>               show the installation directory of the package
$ pip3 search [options] <package>                 search target package
# Python site-packages are here: C:\Users\rreal\AppData\Local\Programs\Python\Python36\Lib\site-packages #
### Other useful command
$ unzip <file.zip> (-d <target_directory> )         extract .zip file under current directory, or target directory is specified
$ nvidia-smi                                        supervice GPU status statically.
$ watch nvidia-smi                                  supervice GPU status dynamically.
$ CUDA_VISIBLE_DEVICE=<1,2>   <python3.6> <filename>  use particular GPU device to run the programm
$ Ctrl + b + d                                      close current window and ternimate tasks
$ Ctrl + q + c                                      exit current running command 

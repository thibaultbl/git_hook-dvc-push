# git_hook-dvc-push

1 - in /shared/folder/hooks, copy the hooks folder

2 - Then on all VMs (based on https://stackoverflow.com/questions/21873326/how-specify-new-path-for-git-hooks-directory)

a - git config --global core.hooksPath /path/to/shared/hooks
b - chown -R root:root /path/to/shared/hooks
c - chmod -R 755 /path/to/shared/hooks


then the hook pre-push-dvc may be modified to push only some files

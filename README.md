# git_hook-dvc-push

in ./.git/hooks/pre-push

add 

```sh
#!/usr/bin/sh
echo "push evaluate"
exec dvc push evaluate
```

then 

configure on all VMs

git config core.hooksPath hooks

```
go mod init github.com/d-selifanov/less3mod
touch less3mod.go
```
copy code to less3mod

```
git add -A
git commit -a
git push
git tag -a v0.0.1 -m "module ver 0.0.1"
git push origin --tags
```

create v2 version

```
mkdir v2
cp less3mod.go v2/
git add -A
git commit -a
```

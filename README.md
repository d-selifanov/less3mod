```
go mod init github.com/d-selifanov/less3mod
touch less3mod.go
```
copy code to less3mod from lesson2

commit, push and add tag v0.0.1

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
cp go.mod v2/
sed -i 's/less3mod/less3mod\/v2/g' v2/go.mod
git add -A
git commit -a -m "add module v2"
git push
git tag -a v2.0.0 -m "module ver 2.0.0"
git push origin --tags
```

check versions

```
go get github.com/d-selifanov/less3mod
go: downloading github.com/d-selifanov/less3mod v0.0.1

go get github.com/d-selifanov/less3mod/v2
go: downloading github.com/d-selifanov/less3mod/v2 v2.0.0
```


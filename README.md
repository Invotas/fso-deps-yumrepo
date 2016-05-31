# Yum repository for XXO dependencies

## Usage

```
# cat /etc/yum.repos.d/xxodeps.repo
[xxodeps]
name=XXO Dependencies
baseurl=https://raw.githubusercontent.com/martin-langhoff/xxo-deps/master/
failovermethod=priority
enabled=1
gpgcheck=0

```

## Update

After adding/removing/changing a package, remember to run
`createrepo ./` and to commit additions, removals and all changes
in `repodata`.


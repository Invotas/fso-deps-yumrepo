# Yum repository for FSO dependencies

## Usage

```
# cat /etc/yum.repos.d/fsodeps.repo
[fsodeps]
name=FSO Dependencies
baseurl=https://raw.githubusercontent.com/Invotas/fso-deps-yumrepo/master/
failovermethod=priority
enabled=1
gpgcheck=0

```

## Update

After adding/removing/changing a package, remember to run
`createrepo ./` and to commit additions, removals and all changes
in `repodata`.


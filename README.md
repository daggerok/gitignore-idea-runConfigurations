# exclude idea files except runConfigurations
IntelliJ IDEA .gitignore file configuration include (exclude fron git ignore) all runConfigurations

## exclude .idea except .idea/runConfigurations/\*

```.gitignore
.idea
!.idea/
.idea/*
!.idea/runConfigurations/
```

explain pattern is very simple: start from project root and move deeply to folder you want keep track

```.gitignore
# let's assume we have ignored folder a
# but we want keep track in a repo only folders: a/b/c and a/b/d
a
!a/
a/*
!a/b/
a/b/*
!a/b/c/
!a/b/d/
```

## exclude legacy project / workspace idea files

```.gitignore
*.iml
*.ipr
*.iws
```

## exclude idea compile output directory

```.gitignore
/out/
```

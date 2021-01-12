# JenkinsPracticePipeline

How to make shell file on Git executalbe:
1. clone git
```
git clone <Git repo URL>
```

2. List files in git
```
cd <Repo diractory>
git ls-files -sc
```

3. Add execute permission
```
git update-index --chmod=+x <shell file>
```

4. Commit back to git
```
git add .
git commit -m "add execute"
```

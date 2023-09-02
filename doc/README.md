# Documentation

## Git flow
### Branches
Branches:
- Main
- Hotfix/A2
- Release/R1
- Develop
- Feature/A1

### Add new feature
1. Check for issues
2. Git command: git checkout -b feature_name development
3. Git command: git commit -m "Added feature_name"
4. GitHub: Create pull request (subject: feature_name, body: Resolve #337 ...)
5. Review
6. Review approved with deleting feature_name branch

## Commands
```shell
git status
git branch -v
git checkout main
git checkout development
git checkout -b development main
git checkout -b feature_name development
git commit -m "Added feature_name"
git push
```

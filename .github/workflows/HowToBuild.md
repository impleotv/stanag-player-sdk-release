The workflow will run automatically on push (with tag) from the STANAG Player SDK.NET setup

To manually run this, add, commit, add tag and push (git tag -a v3.8.9.2 -m "version 3.8.9.2")

```
git add .
git commit -m "ver 3.8.9.2"
git tag -a v3.8.9.2 -m "ver 3.8.9.2"
git push --follow-tags
```
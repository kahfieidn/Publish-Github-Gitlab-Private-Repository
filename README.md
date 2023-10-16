# Generate SSH Keys
```
ssh-keygen -o -t rsa -C "email@email.com"
```

# Publish Github or Gitlab
```
git init
git add .
git commit -m "message"
git remote add origin git@github.com:repo.git
git branch -M main
git push -uf origin main
```

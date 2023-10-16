# Generate SSH Keys

Buka cmd
Lalu jalankan command berikut:
```
ssh-keygen -o -t rsa -C "email@email.com"
```

Copy isi dari file "id_rsa" pada direktori output ssh di : C:\Users\nama_user_komputer\.ssh

Atur SSH Keys pada akun github anda pada menu "Setting"
Masuk ke menu "SSH keys and GPG Keys"
Pilih "New SSH Keys"

# Publish Github or Gitlab
```
git init
git add .
git commit -m "message"
git remote add origin git@github.com:repo.git
git branch -M main
git push -uf origin main
```

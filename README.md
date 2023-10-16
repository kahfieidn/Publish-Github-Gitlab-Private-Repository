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
=================================================================================================

# Khusus Untuk cPanel

Buka terminal,
Lalu generate ssh key

```
ssh-keygen -t rsa -b 2048 -C "username@srv2.jagoankodecloud.com"

touch ~/.ssh/config
chmod 0600 ~/.ssh/config
chown username:username ~/.ssh/config
```

Lalu, setelah key berhasil dibuat:
Buka cPanel
Masuk ke menu "SSH Access"
Dan pilih "Manage SSH Keys"
Lakukan otoriasasi keynya yang sebelumnya unauthorized menjadi authorized
Copy SSH Keysnya

Sekarang kita integrasikan ke github

Atur SSH Keys pada akun github anda pada menu "Setting"
Masuk ke menu "SSH keys and GPG Keys"
Pilih "New SSH Keys"

Paste key yang didapat sebelumnya.

Selesai

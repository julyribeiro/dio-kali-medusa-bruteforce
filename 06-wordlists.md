# 6. Criação de Wordlists

## 6.1 Wordlists simples criadas manualmente
Exemplos:
`echo -e "admin\nuser\nmsfadmin\ntest" > users.txt`
`echo -e "123456\npassword\nadmin\nmsfadmin" > passwords.txt`

## 6.2 Gerando com ferramentas do Kali
`crunch 4 6 abc123 -o wordlist.txt`
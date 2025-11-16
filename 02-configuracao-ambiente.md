# 2. Configuração do Ambiente

## 2.1 Máquinas utilizadas

✔ Kali Linux (bootável ou VM)  
✔ Metasploitable 2 (VM vulnerável)  
✔ DVWA (na própria Metasploitable ou máquina separada)

## 2.2 Configuração de rede no VirtualBox
Ambas as VMs foram configuradas em:

- **Adaptador 1:** Host-Only Adapter  
Garantindo comunicação interna sem acesso externo.

## 2.3 Descobrindo os IPs

No Kali:

`ip a`


Na Metasploitable:

`ifconfig`


Exemplo utilizado:

- Kali: `192.168.56.10`
- Metasploitable: `192.168.56.5`
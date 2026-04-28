# Auditoria de Segurança: Ataques de Força Bruta com Medusa e Kali Linux

## Sobre o Projeto
Este projeto apresenta um estudo técnico sobre a execução e mitigação de ataques de força bruta em ambientes controlados. Utilizando o **Kali Linux** como plataforma de ataque e o **Metasploitable 2** como alvo, simulamos vulnerabilidades em serviços críticos como FTP, SSH e aplicações Web (DVWA).

---

## Configuração do Ambiente.
Para garantir a segurança, o ambiente foi planejado sob uma rede isolada:
* **Rede:** VirtualBox Host-Only Adapter (IP: 192.168.56.0/24).
* **Máquina Atacante:** Kali Linux (IP 192.168.56.101).
* **Máquina Alvo:** Metasploitable 2 (IP 192.168.56.102).

---

## Execução Técnica.

### 1. Reconhecimento com Nmap
O primeiro passo é identificar as portas abertas no alvo:
```bash
# Comando para identificar serviços e versões
nmap -sV -Pn 192.168.56.102

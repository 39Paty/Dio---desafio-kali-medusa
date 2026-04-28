# Auditoria de Segurança: Ataques de Força Bruta com Medusa 🛡️

## Sobre o Projeto
Este projeto documenta a implementação de um laboratório de segurança ofensiva focado em ataques de força bruta (Brute Force). O objetivo é demonstrar como vulnerabilidades de autenticação podem ser exploradas e, principalmente, como implementar medidas de defesa eficazes para proteger serviços de rede e aplicações web.

---

## Metodologia e Infraestrutura
Para otimização de hardware e eficiência técnica, o ambiente foi estruturado utilizando **Containers Docker** em um host **Linux Mint**, em vez de virtualização pesada. Esta abordagem permitiu um consumo reduzido de RAM e maior estabilidade nos testes.

* **Ferramenta de Ataque:** Medusa v2.2 (Execução nativa/Docker).
* **Alvo Vulnerável:** DVWA (Damn Vulnerable Web Application) hospedado via Docker.
* **Protocolos Auditados:** HTTP (Formulário Web) e planejamento para FTP.
* **Rede:** Loopback (127.0.0.1) com mapeamento de portas (8080:80).

---

## Execução Técnica (Cenários Reais)

### 1. Reconhecimento
Antes de iniciar o ataque, validei se o serviço alvo estava ativo:
```bash
# Verificando se o container do alvo está rodando
sudo docker ps

# Laboratório de Infraestrutura Ágil: Ansible, Docker, SQL & Zabbix

Este repositório contém a automação completa para o provisionamento de um ambiente de sistemas distribuídos, focado em alta disponibilidade, monitoramento e persistência de dados. O projeto demonstra a capacidade de orquestrar múltiplos serviços garantindo isolamento de rede e segurança.

##  Tecnologias e Implementações

* **Ansible:** Automação da configuração do host (IaC) e garantia de idempotência.
* **Docker:** Conteinerização de serviços para portabilidade e isolamento de dependências.
* **Nginx:** Configurado como Proxy Reverso, atuando como camada de segurança e gerenciamento de tráfego na porta 80.
* **MySQL 8.0 (SQL):** Gerenciamento de banco de dados relacional com implementação de persistência via volumes.
* **Adminer:** Interface web para administração de banco de dados, facilitando a execução de comandos SQL.
* **Zabbix Agent:** Monitoramento de ativos implementado via container para evitar conflitos de bibliotecas no S.O. Host.

##  Arquitetura de Rede e Sistemas Distribuídos

O projeto utiliza uma **Bridge Network** customizada no Docker (`rede_infra`), permitindo que os serviços se comuniquem via DNS interno pelo nome do container. Isso garante que o banco de dados MySQL não precise expor portas diretamente para a internet, sendo acessível apenas pelos serviços autorizados dentro da rede.

##  Noções de SQL Aplicadas

Como parte do laboratório, foram validadas operações essenciais de banco de dados:
- **DDL:** Criação de tabelas para armazenamento de dados de candidatos e logs.
- **DML:** Inserção de registros e consultas estruturadas (SELECT) para validação de integridade.

##  Como Executar

1. **Clonar o repositório:**
   ```bash
   git clone [https://github.com/arlomends/projeto-devops.git](https://github.com/arlomends/projeto-devops.git)
   cd projeto-devops

##  Contato
Arlon Montes - https://www.linkedin.com/in/arlon-montes-05745b1a1/

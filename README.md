# Automação de Infraestrutura: Proxy Reverso com Ansible & Docker

Este projeto demonstra a automação completa do provisionamento de um servidor web utilizando cultura **IaC (Infrastructure as Code)**.

##  Tecnologias Utilizadas
* **Ansible**: Orquestração e configuração do servidor.
* **Docker**: Conteinerização da aplicação (Nginx Hello World).
* **Nginx**: Configurado como Proxy Reverso.
* **Linux (Ubuntu)**: Sistema operacional base.

##  O que este projeto faz?
1. Atualiza os repositórios do sistema.
2. Instala o motor do Docker e o servidor Nginx.
3. Sobe um container Docker na porta 8080.
4. Configura o Nginx para escutar na porta 80 e redirecionar (Proxy) para o container.

##  Como executar
1. Certifique-se de ter o Ansible instalado.
2. Clone o repositório:
   `git clone https://github.com/SEU_USUARIO/projeto-devops.git`
3. Execute o Playbook:
   `ansible-playbook -i ansible/inventory.ini ansible/playbook.yml --ask-become-pass`

##  Contato
Arlon Montes - https://www.linkedin.com/in/arlon-montes-05745b1a1/

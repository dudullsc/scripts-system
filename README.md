# 🚀 Meus Scripts de Automação (Shell)

Este repositório é uma coleção de scripts shell (`.sh`) que criei para automatizar tarefas de administração de sistemas, instalações de software e configurações gerais em servidores Linux (principalmente Ubuntu).

## 🎯 Sobre o Projeto

O objetivo é simples: **fazer mais, digitando menos**.

Cada script aqui foi projetado para resolver um problema específico, economizar tempo e garantir que as instalações e configurações sejam consistentes e livres de erros.

## 🗂️ Scripts Disponíveis

Abaixo está uma lista de todos os scripts disponíveis e o que eles fazem.

| Script | Sistema(s) Suportado(s) | Descrição |
| :--- | :--- | :--- |
| `instalar_zabbix_server.sh` | Ubuntu 24.04 | Instala o **Zabbix Server 7.4** completo (Server, Frontend, Apache, MariaDB) de forma automatizada. |
| `instalar_zabbix_agent.sh` | Ubuntu 24.04, 22.04 | Instala e configura o **Zabbix Agent 7.4**. Detecta a versão do Ubuntu e pergunta o IP do Server e o Hostname. |
| `instalar_agent_proxmox.sh` | Ubuntu (Qualquer), Debian | Instala o **QEMU Guest Agent** para comunicação correta entre a VM e o host Proxmox. |

---

## 🏁 Como Usar

O uso geral para qualquer script neste repositório é simples:

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
    cd seu-repositorio
    ```

2.  **Dê permissão de execução** ao script desejado:
    ```bash
    chmod +x nome_do_script.sh
    ```

3.  **Execute o script** (a maioria requer `sudo` para instalar pacotes):
    ```bash
    sudo ./nome_do_script.sh
    ```

Siga as instruções que cada script apresentar no terminal.

## 🤝 Contribuição

Contribuições são bem-vindas! Se você tem uma melhoria para um script existente ou quer adicionar um novo:

1.  Faça um "Fork" do projeto.
2.  Crie uma nova "Branch" (`git checkout -b feature/MeuScriptIncrivel`).
3.  Faça o "Commit" das suas mudanças (`git commit -m 'Adiciona script para XYZ'`).
4.  Faça o "Push" para a Branch (`git push origin feature/MeuScriptIncrivel`).
5.  Abra um "Pull Request".

## 📝 Licença

Este projeto é licenciado sob a Licença MIT.

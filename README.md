# Scripts de Instalação Automatizada

Este repositório contém uma coleção de scripts shell (`.sh`) para automatizar a instalação e configuração de diversos softwares em sistemas Linux, com foco principal em distribuições baseadas em Debian (como Ubuntu).

## 🚀 Sobre o Projeto

O objetivo deste projeto é economizar tempo e garantir instalações consistentes e livres de erros. Cansado de digitar os mesmos 50 comandos toda vez que sobe um servidor novo? Este repositório é a solução.

## ✨ Funcionalidades Principais

* **Automatização Completa:** Execute um único arquivo para ter um serviço complexo instalado e configurado.
* **Interatividade:** Os scripts solicitam informações essenciais (como senhas) de forma segura.
* **Limpeza Inteligente:** Opção de remover (purgar) instalações anteriores antes de começar.
* **Verificação de Erros:** Os scripts param se um passo crítico falhar, informando o problema.
* **Logs Claros:** Saída formatada com [INFO], [AVISO] e [ERRO] para fácil acompanhamento.

---

## Scripts Disponíveis

Aqui está a lista dos scripts atualmente disponíveis no projeto:

### 1. Instalador do Zabbix 7.4 (Ubuntu 24.04)

* **Arquivo:** `instalar_zabbix_ubuntu_24.04.sh`
* **Descrição:** Automatiza a instalação completa do Zabbix Server 7.4 no Ubuntu 24.04.
* **Componentes Instalados:**
    * Zabbix Server
    * Zabbix Frontend
    * Zabbix Agent
    * Apache2 (Servidor Web)
    * MariaDB (MySQL) (Banco de Dados)
* **Funcionalidades Específicas:**
    * Instala todas as dependências (PHP, `pv`, etc.).
    * Solicita uma senha para o banco de dados de forma segura.
    * Cria o banco de dados e o usuário automaticamente.
    * Importa o schema do Zabbix com uma barra de progresso.
    * Configura o `zabbix_server.conf` com a senha do DB.
    * Corrige o erro 404 do Apache ativando o `a2enconf zabbix`.
    * Inicia e habilita todos os serviços.

### 2. (Seu Próximo Script Aqui)

* **Arquivo:** `nome-do-script.sh`
* **Descrição:** O que este script faz?
* **Componentes Instalados:** ...

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
    chmod +x instalar_zabbix_ubuntu_24.04.sh
    ```

3.  **Execute o script** (a maioria requer `sudo` para instalar pacotes):
    ```bash
    sudo ./instalar_zabbix_ubuntu_24.04.sh
    ```

Siga as instruções que o script apresentar no terminal.

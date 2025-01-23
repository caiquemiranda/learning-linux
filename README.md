# Linux Basics Learning Repository

Bem-vindo ao **Repositório de Aprendizado de Linux Básico**! Este documento fornece uma visão geral dos comandos essenciais do Linux para iniciantes, com explicações claras em português.

## Sumário

- [Linux Basics Learning Repository](#linux-basics-learning-repository)
  - [Sumário](#sumário)
  - [Introdução](#introdução)
  - [Comandos de Arquivos e Diretórios](#comandos-de-arquivos-e-diretórios)
  - [Permissões e Propriedades](#permissões-e-propriedades)
  - [Monitoramento de Processos e Sistema](#monitoramento-de-processos-e-sistema)
  - [Manipulação e Pesquisa de Arquivos](#manipulação-e-pesquisa-de-arquivos)
  - [Processamento de Texto](#processamento-de-texto)
  - [Gerenciamento de Pacotes](#gerenciamento-de-pacotes)
    - [Sistemas Baseados em Debian (ex.: Ubuntu):](#sistemas-baseados-em-debian-ex-ubuntu)
    - [Sistemas Baseados em Red Hat (ex.: CentOS):](#sistemas-baseados-em-red-hat-ex-centos)
  - [Obtendo Ajuda](#obtendo-ajuda)

---

## Introdução
O Linux é um sistema operacional poderoso e flexível, amplamente utilizado em servidores, desktops e sistemas embarcados. Dominar os comandos básicos do Linux é essencial para uma gestão eficaz do sistema e navegação.

---

## Comandos de Arquivos e Diretórios

- **`pwd`**: Mostra o diretório de trabalho atual.
  ```bash
  pwd
  ```
- **`ls`**: Lista arquivos e diretórios.
  ```bash
  ls -a       # Inclui arquivos ocultos
  ls -l       # Listagem detalhada dos arquivos
  ```
- **`cd`**: Altera o diretório atual.
  ```bash
  cd /path/to/directory
  cd ~        # Vai para o diretório home
  cd -        # Retorna ao diretório anterior
  ```
- **`mkdir`**: Cria um novo diretório.
  ```bash
  mkdir new_directory
  ```
- **`rmdir`**: Remove um diretório vazio.
  ```bash
  rmdir directory_name
  ```
- **`touch`**: Cria um arquivo vazio ou atualiza o timestamp de um arquivo existente.
  ```bash
  touch file_name
  ```
- **`rm`**: Remove arquivos ou diretórios.
  ```bash
  rm file_name        # Remove um arquivo
  rm -r directory     # Remove um diretório e seu conteúdo
  ```
- **`cp`**: Copia arquivos ou diretórios.
  ```bash
  cp source_file destination
  cp -R source_directory destination_directory
  ```
- **`mv`**: Move ou renomeia arquivos e diretórios.
  ```bash
  mv old_name new_name
  mv file_name /new/path
  ```

---

## Permissões e Propriedades

- **`chmod`**: Altera permissões de arquivos ou diretórios.
  ```bash
  chmod u+x file_name  # Adiciona permissão de execução para o dono
  chmod 755 file_name  # Define rwx para o dono, rx para grupo e outros
  ```
- **`chown`**: Altera a propriedade de arquivos.
  ```bash
  chown user:group file_name
  ```

---

## Monitoramento de Processos e Sistema

- **`ps`**: Mostra informações sobre os processos em execução.
  ```bash
  ps aux
  ```
- **`top`**: Monitora processos do sistema em tempo real.
  ```bash
  top
  ```
- **`kill`**: Finaliza um processo pelo seu PID.
  ```bash
  kill PID
  ```

---

## Manipulação e Pesquisa de Arquivos

- **`cat`**: Exibe o conteúdo de um arquivo.
  ```bash
  cat file_name
  ```
- **`find`**: Procura por arquivos e diretórios.
  ```bash
  find /path -name "file_name"
  ```
- **`grep`**: Busca texto dentro de arquivos.
  ```bash
  grep "pattern" file_name
  ```

---

## Processamento de Texto

- **`echo`**: Exibe uma string no terminal.
  ```bash
  echo "Olá, Mundo!"
  ```
- **`wc`**: Conta palavras, linhas e caracteres em um arquivo.
  ```bash
  wc file_name
  ```

---

## Gerenciamento de Pacotes

### Sistemas Baseados em Debian (ex.: Ubuntu):
- **`apt`**: Ferramenta de gerenciamento de pacotes.
  ```bash
  sudo apt update       # Atualiza a lista de pacotes
  sudo apt install pkg  # Instala um pacote
  sudo apt remove pkg   # Remove um pacote
  ```

### Sistemas Baseados em Red Hat (ex.: CentOS):
- **`yum`**: Gerenciador de pacotes para sistemas Red Hat.
  ```bash
  sudo yum install pkg
  sudo yum remove pkg
  ```

---

## Obtendo Ajuda

- **`man`**: Exibe o manual de um comando.
  ```bash
  man command_name
  ```
- **`--help`**: Mostra informações de uso para um comando.
  ```bash
  command_name --help
  ```
  

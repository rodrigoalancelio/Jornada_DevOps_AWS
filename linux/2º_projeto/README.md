# Projeto: Infraestrutura como Código - Criação de Estrutura de Usuários, Diretórios e Permissões

## Visão Geral
Este projeto faz parte da Jornada DevOps e tem como objetivo a criação automatizada de uma estrutura de usuários, grupos de usuários, diretórios e permissões utilizando um script shell. O objetivo é provisionar essa infraestrutura de forma rápida e eficiente, garantindo padronização e facilidade de reutilização.

## Objetivos do Projeto
- Criar um ambiente estruturado de usuários e grupos.
- Configurar permissões automaticamente.
- Automatizar a implantação via script.
- Utilizar um ambiente virtualizado com Vagrant.

## Tecnologias Utilizadas
- **Linux (Ubuntu 24.04)**
- **Shell Script**
- **Vagrant**
- **VirtualBox**
- **Apache**

## Estrutura do Projeto
```
projetos/
  ├── 2º_projeto/
      ├── site/
          ├── linux-site-dio/
              ├── css/
              ├── img/
              ├── js/
              ├── scss/
              ├── vendor/
              ├── about.html
              ├── blog.html
              ├── contact.html
              ├── elements.html
              ├── index.html
              ├── projects.html
              ├── service.html
      ├── vm/
          ├── script.sh
          ├── Vagrantfile
          ├── README.md
```

## Configuração e Uso
### 1. Clonar o repositório
```sh
 git clone https://github.com/rodrigoalancelio/Jornada_DevOps_AWS.git
 cd Jornada_DevOps_AWS/projetos/2º_projeto
```

### 2. Configurar a VM com Vagrant
O arquivo `Vagrantfile` está configurado para iniciar uma VM Ubuntu 24.04 com IP privado `192.168.56.10`.

```sh
 vagrant up
 vagrant ssh
```

### 3. Instalação do Apache e Configuração do Servidor
Dentro da VM:
```sh
 sudo apt update && sudo apt install apache2 -y
 sudo systemctl start apache2
 sudo systemctl enable apache2
```

### 4. Copiar os arquivos do site para o diretório do Apache
```sh
 cp -R linux-site-dio/* /var/www/html/
```

### 5. Executar o Script de Infraestrutura
```sh
 chmod +x script-iac.sh
 ./script-iac.sh
```
Esse script criará automaticamente a estrutura de usuários e permissões.

## Recursos Adicionais
- [Infraestrutura como Código - Script de Criação de Estrutura de Usuários, Diretórios e Permissões](https://github.com/denilsonbonatti/linux-site-dio)
- [Comandos Linux](https://www.linux.ime.usp.br/~albasalo/Apostila/apostila.pdf)

## Conclusão
Este projeto exemplifica como utilizar Infraestrutura como Código para automatizar a criação de ambientes Linux. Com um Vagrantfile e scripts shell, é possível configurar um servidor web e implementar estrutura de usuários de forma automatizada.


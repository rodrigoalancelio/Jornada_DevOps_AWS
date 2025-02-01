# 📌 Infraestrutura como Código: Script de Criação de Estrutura de Usuários, Diretórios e Permissões

## 🏗️ Sobre o Projeto

Este projeto faz parte do bootcamp **Jornada DevOps com AWS - Impulso**, oferecido pela DIO. O objetivo é criar um **script Bash** que automatiza a configuração da infraestrutura inicial de um ambiente Linux, garantindo que:

- **Usuários** sejam criados;
- **Grupos de usuários** sejam configurados;
- **Diretórios específicos** sejam estruturados;
- **Permissões de acesso** sejam corretamente definidas.

Dessa forma, toda nova máquina virtual que executar o script já estará configurada e pronta para uso.

---

## 🔧 Tecnologias Utilizadas

- 🐧 **Linux**
- 📝 **Bash Script**
- ☁️ **GitHub**

---

## 📜 Estrutura do Script

O script executa os seguintes passos:

1. **Criação de diretórios**:
   - `/publico`
   - `/adm`
   - `/ven`
   - `/sec`
2. **Criação de grupos de usuários**:
   - `GRP_ADM`
   - `GRP_VEN`
   - `GRP_SEC`
3. **Criação de usuários e atribuição aos grupos**
4. **Configuração das permissões de diretório**
5. **Upload do script no GitHub para reutilização futura**

---

## 📥 Como Executar o Script

1. Clone este repositório:
   ```sh
   git clone https://github.com/seu-usuario/linux-projeto1-iac.git
   ```
2. Acesse o diretório do projeto:
   ```sh
   cd linux-projeto1-iac
   ```
3. Dê permissão de execução ao script:
   ```sh
   chmod +x criar_estrutura.sh
   ```
4. Execute o script como **root**:
   ```sh
   sudo ./criar_estrutura.sh
   ```

---

## 📎 Recursos Úteis

- [Principais comandos do Linux](https://www.linux.ime.usp.br/~albasalo/Apostila/apostila.pdf)
- [Mais informações sobre usuários no Linux](https://www.infowester.com/usuarioslinux.php)

---

## 🛠️ Contribuição

Se desejar contribuir com melhorias, siga os passos abaixo:
1. **Fork** este repositório.
2. Crie uma **branch** para suas alterações.
3. Submeta um **Pull Request**.

---

## 📌 Contato

Caso tenha dúvidas ou sugestões, fique à vontade para entrar em contato ou contribuir para o repositório!

🚀 **Bons estudos e boas práticas DevOps!**

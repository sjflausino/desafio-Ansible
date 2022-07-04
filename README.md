# desafio-Ansible

## É necessario Vagrant e Ansible instalados em sua maquina local.

Primeiro faremos download do repositório com nossos arquivos de configuração do vagrant e provisionamento do Ansible:
```
https://github.com/sjflausino/desafio-Ansible.git
```
Após entraremos no diretório criado:
```
cd desafio-Ansible
```
Neste momento executaremos o ```vagrant up``` para provisionarmos nossa maquina virtual para executar nosso playbook;

Assim que a vm for criada podemos executar o comando de provisionamento do ansible:

```
ansible-playbook provisioning.yml -i host
```
Nesse momento o ansible irá provisionar um ambiente docker dentro de nossa vm, esse ambiente sera responsável por clonar este repositório ```https://github.com/sjflausino/desafio-Docker.git ```

Conseguiremos ver a aplicação em funcionamento acessando http://localhost:8080/

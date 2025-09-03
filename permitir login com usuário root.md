## Permitir login com usuário root  

01 - Acesse o servidor com seu usuário padrão e execute: <code>sudo su</code> para liberar acesso root

02 - edite o arquivo <code>sshd_config</code> com o comando nano <code> /etc/ssh/sshd_config</code> 

03 - Procure a linha que contém: <code> #PermitRootLogin prohibit-password</code> altere para <code> PermitRootLogin yes</code> removendo # no início!

04 - Salve o arquivo e execute o comando: <code> systemctl restart ssh</code> 
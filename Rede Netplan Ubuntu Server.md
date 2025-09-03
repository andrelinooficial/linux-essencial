## Configuração de Rede via Netplan

#### Procedimento para configuração de IP Fixo no Ubuntu Server:

01 - Acesse o servidor Linux com privilégio root

02 - Vá para /etc/netplan/

03 - Faça uma cópia de segurança do arquivo <code>50-cloud-init.yaml</code>

04 - Configure o arquivo conforme o exemplo abaixo:

```
network:
  version: 2
  ethernets:
    enp0s18:
      dhcp4: no
      addresses:
        - 192.168.1.200/24
      gateway4: 192.168.1.254
      nameservers:
        addresses:
          - 1.1.1.1
          - 8.8.8.8

```

OBS: 
- Respeite os espaços, pois arquivos YAML devem respeitar ierarquia ! Caso esteja diferente do exemplo acima pode não funcionar!
- Troque as Informações de acordo com a sua Rede e o nome da placa de rede da VM 
- Após salvar o arquivo execute o comando <code>sudo netplan apply</code>

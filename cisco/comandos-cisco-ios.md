**Trocar nome do equipamento**
```
>enable
#configure terminal
(config)#hostname <nome>
```

**Configurar um banner**
```
>enable
#configure terminal
(config)#banner motd "<texto>"

M.O.T.D - Message Of The Day
```

**Configurar senha na Console**
```
>enable
#configure terminal
(config)#line console 0
(config-line)#password <senha>
(config-line)#login
```

**Configurar senha na enable**
```
>enable
#configure terminal
(config)#enable secret <senha>
```

**Verificar as configurações que estão rodando no equipamento**
```
>enable
#show running-config
```

**Ativar o serviço de criptografia**
```
>enable
#configure terminal
(config)#service password-encryption
```

**Desfazer configurações no IOS**
```
Colocar "no" na frete do comando
```

**Desativar uma interface**
```
>enable
#configure terminal
(config)#interface <nome>
(config-if)#shutdown

        Exemplo:
            interface FastEthernet 0/2
```

**Desativar várias interfaces de uma vez**
```
>enable
#configure terminal
(config)#interface range <intervalo>
(config-if-range)#shutdown

    Exemplo:
    (config)#interface range f0/1-3
    (config-if-range)#shutdown
```

**Ver o resumo das interfaces**
```
>enable
#show ip interface brief
```

**Salvar as configurações**
```
>enable
#wr

>enable
#copy running-config startup-config
```

**Resetar o equipamento**
```
>enable
#write erase
```

**Colocar IP em uma Interface**
```
>enable
#configure terminal
(config)#interface <nome>
(config-if)#ip address <ip> <mascara>
(config-if)#no shutdown
```

**Colocar descrição em uma interface
```
>enable
#configure terminal
(config)#interface <nome>
(config)#description <descricao>
```

**Visualizar tabela de roteamento [ROTEADOR]**
```
>enable
#show ip route
```

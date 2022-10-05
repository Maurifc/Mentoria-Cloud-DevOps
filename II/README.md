# Aprentação
[Linux - Usuários, grupos, permissões, pacotes e variáveis de ambiente](https://docs.google.com/presentation/d/1UMFF6ro10n-hzED5k-7-COSYuz27dbHBD6SgdvNJG6c/edit?usp=sharing)


# Demos

## Usuários, grupos e permissões

```bash
# create user and group
adduser joao
addgroup bonde

# show userid
id joao

# create dir
mkdir /tmp/pasta10

# list permission
ls -l /tmp/pasta10

# change owner and group
chown joao:bonde /tmp/pasta10

# change permissions
chmod 624 /tmp/pasta10
```

## Instalação de pacotes

### Instalando via gerenciador de pacote (APT)
```bash
apt install nano
```

### Instalando via script (Docker)
https://docs.docker.com/engine/install/ubuntu/#install-using-the-convenience-script

### Download direto do executável (Helm)
https://helm.sh/docs/intro/install/

## Variáveis de ambiente

1. Define uma variável sem exportá-la
```bash
# set a variable
DATA_ATUAL="05-10-2022"

# print a variable
echo $DATA_ATUAL
```

2. Roda o script antes de exportar `DATA_ATUAL`
```bash
./imprime_envs.sh
```

3. Exporta a variável `DATA_ATUAL`
```bash
export DATA_ATUAL="05-10-2022"
```

4. Roda o script antes de exportar `DATA_ATUAL`
```bash
./imprime_envs.sh
```
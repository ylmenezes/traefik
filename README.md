# Traefik

## Instruções de instalação

### 1 - Criando os volumes para o container

```
create volume traefik_certificates
```
### 2 - Criando a rede (network)
```
docker network create -d overlay traefik_net
```
### 3 - Executando o container
```
docker-compose -f traefik.yml up -d
```
## Exemplo de container

Para você criar um apontamento de dominio para o contaier, siga o exemplo do arquivo service-stack.yml
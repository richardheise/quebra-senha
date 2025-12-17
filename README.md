# Quebra Senha

Este repositório contém scripts para quebrar senhas usando diferentes métodos.

## Estrutura de Arquivos

O repositório está organizado da seguinte forma:

-   `scripts/`: Contém os scripts Python para quebrar as senhas.
-   `dictionaries/`: Contém os dicionários de senhas usados pelos scripts.
-   `hashes/`: Contém os arquivos de hash a serem quebrados.
-   `results/`: Contém os resultados da execução dos scripts.

## Como Usar

Para usar os scripts, você precisa ter o Python 3 instalado.

**Importante:** Os scripts devem ser executados a partir do diretório raiz do projeto.

1.  Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/quebra-senha.git
    ```
2.  Navegue até o diretório do projeto:
    ```bash
    cd quebra-senha
    ```
3.  Execute o script desejado, passando o hash como entrada.

### Exemplo com `busca_md5.py`

Para quebrar um hash MD5, execute o seguinte comando:

```bash
echo "SEU_HASH_MD5" | python3 scripts/busca_md5.py
```

O script tentará quebrar o hash usando os dicionários e, em seguida, por força bruta.

### Exemplo com `busca_yescript.py`

Para quebrar um hash yescrypt, execute o seguinte comando:

```bash
echo "SEU_HASH_YESCRYPT" | python3 scripts/busca_yescript.py
```

**Aviso:** A busca por força bruta no `busca_yescript.py` pode demorar vários dias.

## Scripts

-   `busca_md5.py`: Tenta quebrar um hash MD5 usando ataques de dicionário e força bruta.
-   `busca_yescript.py`: Tenta quebrar um hash yescrypt usando ataques de dicionário e força bruta.

## Dicionários

-   `dicionario_completo.txt`: Um dicionário completo de senhas.
-   `1MillionPasswords.txt`: Uma lista com 1 milhão de senhas comuns.
-   `pimpolho.txt` e `testeadm.txt`: Outras listas de senhas.

## Hashes

-   `md5.txt`: Um arquivo de exemplo com hashes MD5 a serem quebrados.

## Resultados

-   `results/`: Este diretório armazena os resultados das tentativas de quebra de senha.
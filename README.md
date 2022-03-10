## Bombcrypto-bot
## Utilizei Fork de duas Pessoas
https://github.com/mpcabete/bombcrypto-bot
https://github.com/MatheusHAS/bombcrypto-bot

# Bombcrypto-bot

## Funções extras adicionadas

- Usar browser com zoom diferente (scale)
- Suporte a multiplas contas no mesmo monitor (usar URL do IFRAME para acessar)
- Debug por funções do game
- Suporte a monitores retina
- Adicionado sistema de login novo após o connect

# Instalação:

### Baixe e instale Python na versão maior que 3 no [site oficial](https://www.python.org/downloads/) ou através da [windows store](https://www.microsoft.com/p/python-37/9nj46sx7x90p?activetab=pivot:overviewtab).

Se você baixar pelo site é importante marcar a opção para adicionar o
python ao PATH:
![Check Add python to PATH](https://github.com/mpcabete/bombcrypto-bot/raw/ee1b3890e67bc30e372359db9ae3feebc9c928d8/readme-images/path.png)

### Realize o download do codigo no formato zip, e extraia o arquivo.

### Copie o caminho até a pasta do bot:

![caminho](https://github.com/mpcabete/bombcrypto-bot/raw/main/readme-images/address.png)

### Abra o terminal.

Aperte a tecla do windows + r e digite "cmd":

![launch terminal](https://github.com/mpcabete/bombcrypto-bot/raw/main/readme-images/cmd.png)

### Navegue até a pasta do bot:
Digite o comando "cd" + caminho que você copiou:

![cd](https://github.com/mpcabete/bombcrypto-bot/raw/main/readme-images/cd.png)

### Instale as dependências:

```
pip install -r requirements.txt
```

  
![pip](https://github.com/mpcabete/bombcrypto-bot/raw/main/readme-images/pip.png)

### Pronto! Agora é só iniciar o bot com o comando

```
python3 index.py
```

![run](https://github.com/mpcabete/bombcrypto-bot/raw/main/readme-images/run.png)


# Como usar?

Abra o terminal, se ainda não tiver navegado para a pasta do bot dê novamente o comando

```
"cd" + caminho que você copiou
```

Para iniciar use o comando 

```
python3 index.py
```


2 - Após instalado python:

- Para `windows` _execute como administrador_ o arquivo `run.bat` na pasta principal.
- Ou se preferir no `windows` tecla Windows+r digitar cmd, digitar o local onde está a pasta do bot exemplo: cd c:\bomb dar entre, após isso é só usar python index.py
- Para `linux` o arquivo `run.sh` na pasta principal.

# Configurações:

Você pode configurar algumas opções alterando o arquivo `config.yaml` na pasta principal do bot.

## `scale_image`

- Você agora tem suporte de colocar quantos % de zoom está usando em seu navegador.

  > Se atente também ao ZOOM da janela de notificação do _Metamask_, ela deve ser a mesma usada no navegador.

  - ### `enable`

    Quando `True`, ativa a funcionalidade de usar um scale diferente. Caso contrário, deixe o valor como `False`

    > O valor deve ser: `True` ou `False`

  - ### `percent`
    A porcentagem de zoom do seu navegador e da janela de notificação do metamask.
    > O Valor deve ser de: `50` a `100`. Quanto menor o valor, mais impreciso serão as detecções do bot.

## `is_retina_screen`

- Caso seu computador seja um dispositivo mac com tela retina, será necessário ativar essa opção para que o bot realize clicks com precisão. Se seu bot move o mouse para lugares aleatórios, talvez essa opção te ajude.
  > O valor deve ser: `True` para ativar, ou `False` para desativar

## `mouse_move_speed`

- Você pode configurar a velocidade com que o mouse se move na tela antes da realização do click.
  > O valor deve ser de: `0.1` a `1`

## `multiples_accounts_same_monitor`

- Essa opção habilita o uso de multiplas contas no mesmo monitor, sendo as ações feitas de forma sincrona, ou seja, uma janela por vez. Para usar essa funcionalidade sugiro utilizar a URL do IFRAME do jogo.

  - ### `enable`

    > O Valor deve ser: `True` para habilitar ou `False` para desabilitar

  - ### `window_contains_title`
    Essa opção te fornece a possibilidade de alterar qual o texto que será utilizado para detectar as janelas. Esse texto deve estar no título da janela do nevegador.

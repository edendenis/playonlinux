# Como instalar/configurar/usar o `PlayOnLinux (POL)` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para instalar/configurar/usar o `PlayOnLinux (POL)` no `Linux Ubuntu`.

## _Abstract_

_This document contains the main commands and settings for installing/configuring/use `PlayOnLinux (POL)` on `Linux Ubuntu`._


## Descrição [2]

### `PlayOnLinux (POL)`

O `PlayOnLinux (POL)` é uma aplicação de código aberto projetada para simplificar a instalação e execução de jogos e aplicativos do `Windows` em sistemas Linux. Ele utiliza o Wine, uma camada de compatibilidade que permite a execução de programas `Windows` em ambientes Linux, e oferece uma interface gráfica amigável que facilita o processo de configuração e instalação. O PlayOnLinux possui um vasto repositório de scripts e configurações pré-definidas para uma ampla variedade de jogos e programas, tornando mais fácil para os usuários encontrar e instalar suas aplicações `Windows` favoritas. Isso o torna uma escolha popular para jogadores e usuários que precisam de aplicativos específicos do `Windows` em seus sistemas `Linux`, proporcionando uma experiência mais acessível e otimizada.


## 1. Configurar/Instalar/Usar o `PlayOnLinux (POL)` no `Linux Ubuntu` [1]

Para configurar/instalar/usar o `PlayOnLinux (POL)` no `Linux Ubuntu`, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`


2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
    

3. Para configurar/instalar/usar o `PlayOnLinux (POL)` execute o comando: `sudo apt install playonlinux -y`

    **OBSERVAÇÂO(ÕES)**: O diretório para a(s) pasta(s) ou arquivo(s) é indicado a seguir, conferir se no diretório se a(s) pasta(s) e/ou o(s) arquivo(s) existe(m), se não, copiar da pasta `docs` para o diretório:
    
    ```
    whereis playonlinux
    /usr/bin/playonlinux /usr/share/playonlinux /usr/share/man/man1/playonlinux.1.gz
    ```

    Você pode usar o código a seguir para copiar a pasta ou o arquivo para o diretório:
    
    ```
    sudo cp /home/edenedfsls/Documents/Downloads/unix/ubuntu/playonlinux/docs/usr/bin/playonlinux /usr/bin/ 
    sudo cp -r /home/edenedfsls/Documents/Downloads/unix/ubuntu/playonlinux/docs/share/playonlinux /usr/share/ 
    sudo cp /home/edenedfsls/Documents/Downloads/unix/ubuntu/playonlinux/docs/usr/share/man/man1/playonlinux.1.gz /usr/share/man/man1/ 
    ```


## 2. Código completo para configurar/instalar/usar o `PlayOnLinux (POL)`

Para configurar/instalar/usar o `PlayOnLinux (POL)` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    sudo apt autoclean
    sudo apt autoremove -y
    sudo apt update
    sudo apt --fix-broken install
    sudo apt clean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install playonlinux -y
    playonlinux
    ```

## Referências

[1] OPENAI. ***Instalação do playonlinux no xubuntu.*** Disponível em: <https://chat.openai.com/c/74f27d86-e06e-4724-8c5a-e8fe2aed3754> (texto adaptado). Acessado em: 20/10/2023 22:16.

[2] OPENAI. ***Vs code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). Acessado em: 14/11/2023 09:33.


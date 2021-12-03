# Game Of Life
Neste repositório você irá encontrar um protótipo do jogo da vida de Conway desenvolvido para a disciplina de Lógica (2021.2) da UFRJ.

## Sobre o jogo da vida:
O jogo da vida é um autómato celular desenvolvido pelo matemático John Horton Conway. Esse autômato foi criado de modo a reproduzir, através de regras simples, as alterações e mudanças em grupos de seres vivos, tendo aplicações em diversas áreas da ciência. As regras definidas são aplicadas a cada nova "geração"; assim, a partir de uma imagem em um tabuleiro bi-dimensional definida pelo jogador, percebem-se mudanças muitas vezes inesperadas e belas a cada nova geração, variando de padrões fixos a caóticos.

## As regras do Game of Life são as seguintes:
Qualquer célula viva com menos de dois vizinhos vivos morre de solidão;
Qualquer célula viva com mais de três vizinhos vivos morre de superpopulação;
Qualquer célula morta com exatamente três vizinhos vivos se torna uma célula viva;
Qualquer célula viva com dois ou três vizinhos vivos continua no mesmo estado para a próxima geração.
 

## Setup (Windows):
### 1-) Instando o Ruby:
Para realizar a instalação do Ruby, basta você escolher a versão que se adeque ao seu computador e realizar o download. Em seguida, executar o arquivo baixado e configurar seu ambiente. Você pode baixar o arquivo pelo link:  
https://rubyinstaller.org/downloads/
 
### 2-) Instale a biblioteca “ruby2d”:
Para o funcionamento do programa é necessário a instalação da biblioteca “ruby2d”. Para instalar essa biblioteca, você deve executar o seguinte comando no terminal:
gem install ruby2d

## Setup (Linux):
### 1-) Instalando o Ruby:
#### 1.1-) No seu terminal, clone o repositorio rbenv em ~/.rbenv:
        
	git clone https://github.com/rbenv/rbenv.git ~/.rbenv
        

#### 1.2 -) Instale o ruby-build como um plugin do rbenv, no qual vai adicionar o comando “rbenv install”:
        
	git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
        
	
#### 1.3 -) Adicione rbenv ao path e inicialize pelo seu ~/.bashrc ou  ~/.bash_profile:
       
	export PATH="$HOME/.rbenv/bin:$PATH"
	eval "$(rbenv init -)"
         
#### 1.4 -) Obtenha acesso ao rbenv carregando a nova shell utilizando:
         
	source ~/.bashrc  # ou `~/.bash_profile`
        
#### 1.5 -) Instale alguns pacotes (pode não ser necessario):
          
	https://github.com/rbenv/ruby-build/wiki#suggested-build-environment
          
#### 1.6 -) Instale a última versão do Ruby (3.0.1 até agora) e coloque como padrão global

 	rbenv install 3.0.1
	rbenv global 3.0.1
        
#### 1.7 -) Verifique se está tudo funcionando ( $ é o símbolo do prompt):
         
	$ rbenv versions
        system
        * 3.0.1 (set by /home/<me>/.rbenv/version)
        $ ruby -e "puts 'Hello Ruby'"
        Hello Ruby
        
### 2) Instale a biblioteca “ruby2d”
O Ruby 2D precisa de alguns pacotes, que são específicos para cada distribuição do Linux:
##### Ubuntu, Debian, and Mint
        
	sudo apt install libsdl2-dev libsdl2-image-dev libsdl2-mixer-dev libsdl2-ttf-dev
       
##### CentOS and Fedora

        sudo yum install SDL2-devel SDL2_image-devel SDL2_mixer-devel SDL2_ttf-devel
        openSUSE
        sudo zypper install libSDL2-devel libSDL2_image-devel libSDL2_mixer-devel libSDL2_ttf-devel
         
##### Arch
    
        sudo pacman -S sdl2 sdl2_image sdl2_mixer sdl2_ttf
       
 
### IMPORTANTE!
A instalação no Linux não é nada trivial comparada ao windows, para alguns erros, esse link foi util:
	
	https://www.friendlyskies.net/notebook/how-to-install-ruby2d-in-ubuntu-1804


## Rodando o jogo: 
##### 1 -) Clone o repositório
##### 2 -) Executando o game of life
Para abrir o programa basta clicar no executável do jogo

## Funcionamento do nosso protótipo:
##### 1 -) Clicando na tecla 'p' o jogo é iniciado ou pausado
##### 2 -) Clicando na tecla 'c' o grid é limpo

##### Referência:
Vídeo usado com referência para esse trabalho

	https://www.youtube.com/watch?v=Rp7v1f4lpPU


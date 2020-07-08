<p align="center">
    <img width="650" height="200" src="https://practice.uffs.cc/images/logo.png" title="Logo do projeto"><br />
    <img src="https://img.shields.io/maintenance/yes/2020?style=for-the-badge" title="Status do projeto">
    <img src="https://img.shields.io/github/workflow/status/ccuffs/template/ci.uffs.cc?label=Build&logo=github&logoColor=white&style=for-the-badge" title="Status do build">
</p>

# Site do PRACTICE

Esse repositório contém o site do Programa de Ampliação e Consolidação de Tecnologias e Inovação no Contexto Educacional (PRACTICE) da Universidade Federal da Fronteira Sul, disponível em practice.uffs.cc

Link para o site oficial: https://practice.uffs.cc/

> **Dúvidas gerais:** Envie um e-mail para [practice@uffs.edu.br](mailto:practice@uffs.edu.br)

## Começando

Para testar o site localmente na sua máquina, você precisa ter algumas ferramentas instaladas que dependem do sistema operacional em uso. Siga os guias abaixo conforme o seu sistema operacional.

### 1. Windows
#### 1.1 Pré-requisitos

Você precisa ter o [git](https://gitforwindows.org/) instalado e um editor de código qualquer, ex.: [Visual Studio Code](https://code.visualstudio.com), disponíveis. Se você estiver usando Windows 10, é recomendado utilizar o [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/about) para rodar o site.

> **IMPORTANTE:** se você está no _Windows 10_, pule para a seção _[2. Linux (Ubuntu)](#2-Linux-Ubuntu)_ e siga as instruções dessa seção. Se estiver usando Windows 8, 7 ou inferior, continue lendo as seções abaixo.

#### 1.1 Instale o Ruby

Instale a última versão do [Ruby](https://www.ruby-lang.org) através do [RubyInstaller](https://rubyinstaller.org/downloads/). Baixe uma das versões **Ruby+Devkit** disponíveis, como o [rubyinstaller-devkit-2.6.3-1-x64.exe](https://github.com/oneclick/rubyinstaller2/releases/download/RubyInstaller-2.6.3-1/rubyinstaller-devkit-2.6.3-1-x64.exe), rode, e no último passo do instalador, escolha `ridk install` (para instalar gems com extensões nativas).

#### 1.2 Instale o bundler

O site é construído com base no [Jekyll](https://jekyllrb.com) que usa o bundler para gerenciar dependencias. Abra um terminal novo (para garantir que o `PATH` está atualizado depois de instalar o Ruby), e rode:

```
gem install bundler
```

### 2. Linux (Ubuntu)
#### 2.1 Pré-requisitos

Você precisa ter o [git](https://gitforwindows.org/) e um editor de código qualquer, ex.: [Visual Studio Code](https://code.visualstudio.com), disponíveis:

```
sudo apt-get install git code
```

#### 2.2 Instale o Ruby

Instale a última versão do [Ruby](https://www.ruby-lang.org):

```
sudo apt-get install ruby-full build-essential zlib1g-dev
```

A partir desse ponto, não é recomendado a utilização de uma conta _root_. Use a sua própria conta de usuário.

Primeiramente, configure o ambiente para a instalação do Ruby Gems: 

```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
```

Exporte o `GEM_HOME`:

```
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
```

Adicione o `GEM_HOME` ao `PATH`:

```
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
```

Carregue as novas configurações para o terminal:

```
source ~/.bashrc
```

#### 2.3 Instale o bundler

O site é construído com base no [Jekyll](https://jekyllrb.com), que usa o bundler para gerenciar dependencias.

```
gem install bundler
```

## Manuseio do site

Se você seguiu os pré-requisitos de instalação, a partir desse ponto você pode testar o site localmente na sua máquina. Siga os passos abaixo para 

### 1. Faça fork do repositório

Faça ***fork*** do repositório do site pelo Github.

### 2. Clone esse repositório

**Clone o seu fork** em uma pasta qualquer da sua máquina, e.x: `c:\` ou `/tmp/:

```
git clone https://github.com/SEU_USUARIO/website-programa.git && cd website-programa
```

Mude para a branch *`dev`*.
```
git checkout dev
```
> **Cuidado:** Preste atenção em qual das branchs estão sendo feitas as alterações.

Instale todas as dependências:

```
cd src
bundle update
```

Antes de fazer qualquer alteração no site, lembre-se do ***[Guia para a equipe de desenvolvimento](https://github.com/orgs/practice-uffs/teams/dev/discussions/1)***.

### 3. Testando o site

Para testar o site, entre na pasta onde você clonou esse repositório, e rode:

```
bundle exec jekyll serve
```

Após alguns segundos, o site estará disponível através da URL [http://127.0.0.1:4000](http://127.0.0.1:4000).
Depois de rodar o comando, você deve ver algo similar ao seguinte:

```
Configuration file: /mnt/c/website-programa/_config.yml
            Source: /mnt/c/website-programa
       Destination: /mnt/c/website-programa/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 6.255 seconds.
                    Auto-regeneration may not work on some Windows versions.
                    Please see: https://github.com/Microsoft/BashOnWindows/issues/216
                    If it does not work, please upgrade Bash on Windows or run Jekyll with --no-watch.
 Auto-regeneration: enabled for '/mnt/c/website-programa'
    Server address: http://127.0.0.1:4000
  Server running... press ctrl-c to stop.
```


## Licença

Esse projeto é licenciado nos termos da licença open-source [Apache 2.0](https://choosealicense.com/licenses/apache-2.0/) e está disponível de graça.

## Histórico de alterações

Todas as alterações importantes no site são relatadas no arquivo [CHANGELOG.md](CHANGELOG.md).

## Links importantes

* [Página oficial do PRACTICE](https://practice.uffs.cc/)
* [Site da Universidade Federal da Fronteira Sul](https://www.uffs.edu.br)

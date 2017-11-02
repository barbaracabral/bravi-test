# bravi-test
Testing ContaAzul application with Cucumber, Capybara, SitePrism in Ruby language


## Configurando o ambiente ##

### Instalar rbenv ###
Execute os seguintes comandos:
```shell
$ git clone https://github.com/rbenv/rbenv.git ~/.rbenv

$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
$ echo 'eval "$(rbenv init -)"' >> ~/.bashrc
$ source ~/.bashrc
```

Inclua no ~/.bash_profile:
```shell
eval "$(rbenv init -)"
```

Listar as versões disponíveis:
```shell
rbenv install -l
```

Instalar uma versão:
```shell
rbenv install 2.4.2
```

Tornar a versão padrão para todos os projetos
```shell
$ rbenv global 2.4.2
```

Verficar a versão do Ruby instalada
```shell
$ ruby -v
```

### Instalando o bundler ###
Navegar dentro do projeto e instalar o bundler
```shell
cd /bravi-test-rest
gem install bundler
```

### Instalando as gems ###
Execute o seguinte comando dentro da raiz do projeto:
```shell
bundle install
```

### Drivers necessários: ###

* Instalar:
    * [chromedriver](https://christopher.su/2015/selenium-chromedriver-ubuntu/ )


### Executando os testes ###
Execute o seguinte comando dentro da raiz do projeto:
```shell
cucumber features
```

### Executando tags###
Execute o seguinte comando dentro da raiz do projeto:
```shell
cucumber --tags @login_conta_azul @nova_compra
```

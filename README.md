tableless-firefox-os-example
============================

Example application Firefox OS - Tableless


<h2>Introdução</h2>

Firefox OS é novo sistema operacional movel desenvolvido para Mozilla.
Para nos desenvolvedores web ficou fácil criar aplicativos para aparelhos
mobile, pois para desenvolver é utilizado HTML5, CSS e JAVASCRIPT.

Para testar seus aplicativos não precisa ter um smartphone com Firefox OS,
basta baixar a extensão (Firefox OS Simulator) no Firefox disponivel em
Windows, Linux e MAC OS X.

<h2>Colocando em pratica</h2>

Primeiro passo é instalar a extensão Firefox OS Simulator em seu Firefox.

Firefox OS Simulator - links para Download
Windows - https://addons.mozilla.org/firefox/downloads/file/190978/firefox_os_simulator-2.0-fx-windows.xpi
Linux - https://addons.mozilla.org/firefox/downloads/file/190986/firefox_os_simulator-2.0-fx-linux.xpi
Mac OS X - https://addons.mozilla.org/firefox/downloads/file/190998/firefox_os_simulator-2.0-fx-mac.xpi

<h2>Iniciando Firefox OS Simulator</h2>

Para abrir o Firefox OS Simulator procure a aba
Ferramentas > Desenvolvedor web > Firefox OS Simulator. Uma aba sera aberta
com as informações do Firefox OS Simulator. Nesta aba você pode desligar e
ligar o emulador e nela também é adicionado os aplicativos que serão
instalados no emulador assim que iniciado. Para adicionar seus aplicativos
pasta clicar em Add diretory e localizar a pasta em que você desenvolveu seu
aplicativo.

<h2>Criando uma aplicação para Firefox OS</h2>

Para iniciar, crie uma pasta do seu projeto onde ficaram os arquivos da sua aplicação. No meu caso willemallan. Dentro do diretório crie um arquivo manifest.webapp neste arquivo ficam as configurações do projeto, como: nome, autor, versão, icones e outros dados importantes do aplicativo. Veja abaixo o exemplo do arquivo manifest.webapp.

    {
        "version": "0.1",
        "name": "Willem Allan",
        "description": "Willem Allan - Blog posts",
        "launch_path": "/index.html",
        "icons": {
            "16": "/imgs/icons/wi16.png",
            "48": "/imgs/icons/wi48.png",
            "128": "/imgs/icons/wi128.png"
        },
        "developer": {
            "name": "Willem Allan",
            "url": "http://willemallan.com.br"
        },
        "installs_allowed_from": ["*"],
        "locales": {
            "es": {
                "description": "Willem Allan - Blog posts",
                "developer": {
                    "url": "http://willemallan.com.br"
                }
            },
            "it": {
                "description": "Willem Allan - Blog posts",
                "developer": {
                    "url": "http://willemallan.com.br"
                }
            }
        },
        "default_locale": "en"
    }

Analisando o código acima, pode ser visualizado que possuem locais para definir a versão do aplicativo, nome e descrição. Logo após, repare que launch_path aponta para /index.html, que é o primeiro arquivo que irá ser carregado quando o aplicativo for iniciado. Pode ser defino também os icones em diversos tamanhos em icons. Por ultimo temos opções para os dados do desenvolvedor que também pode ser definido em outros idiomas.

<h2>Mão na massa</h2>

Para iniciar crie um diretório da sua aplicação e em seguida crie um arquivo index.html e utilize o arquivo citado acima manifest.webapp alterando as configurações do seu projeto.

Então ficará assim uma pasta nome_projeto e dentro os arquivos index.html e manifest.webapp.

Adicione um texto qualquer no arquivo index.html, pode ser o famoso hello world!!!

    <h1>hello world!!! Primeira aplicação Firefox OS</h1>


Para testar a aplicação é preciso ir na extensão do Firefox OS Simulator, Bashboard e adicionar a pasta do projeto "add directory", depois inicie o emulador a aplicação será instalada e aparecerá nos aplicativos.

github - exemplo de aplicação do Firefox OS: <a href="https://github.com/willemallan/tableless-firefox-os-example"  target="_blank">link</a>
github page - <a href="http://willemallan.github.io/tableless-firefox-os-example/"  target="_blank">link</a>

<h2>Saiba mais</h2>

Firefox OS Quick Start - https://marketplace.firefox.com/developers/docs/quick_start
Desenvolva para Firefox OS sem um smartphone - https://marketplace.firefox.com/developers/docs/firefox_os_simulator
Aplicativos de exemplo - https://marketplace.firefox.com/developers/docs/reference_apps
Disponibilizando um aplicativo no Mozilla Marketplace - https://developer.mozilla.org/pt-BR/docs/Apps/Submitting_an_app

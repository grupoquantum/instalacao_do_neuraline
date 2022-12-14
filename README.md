# Instalador
1.0.0

## Para desbloquear todos os recursos, siga as etapas abaixo.

### Instalação do Neuraline
<div align="justify">
Primeiramente com o <a href="https://www.python.org">Python</a>3.10 ou superior instalado, se você for um usuário Windows baixe o arquivo instalador clicando <a href="https://github.com/aiquantumneuro/instalacao_do_neuraline/raw/main/neuraline_installer.pyc">aqui</a> ou se preferir baixe o código fonte para Windows clicando <a href="https://github.com/Neuraline/Neuraline/archive/refs/heads/main.zip">aqui</a> e o extraia para o seu diretório de projetos, depois siga para o <a href="#step1">passo 1</a>. Caso você seja um usuário Linux(deb) não será preciso instalador, basta baixar o código fonte clicando <a href="https://github.com/Neuraline/Neuraline_linux_distributions/archive/refs/heads/main.zip">aqui</a> e extraí-lo para a sua pasta de projetos. Recomendamos a última versão do Ubuntu para usuários Linux. Se você for um usuário Windows e estiver usando o instalador siga as instruções a seguir para executá-lo, para aqueles que não estiverem usando o instalador ou para usuários Linux pule direto para o <a href="#step1">passo 1</a> logo abaixo.<br>
Usuários Windows (com o instalador): Depois de baixar o arquivo instalador, acesse o diretório para onde o arquivo foi baixado através do terminal.
Por exemplo, no caso do Windows pesquise por cmd na sua barra de pesquisas e abra o Prompt de Comando.
Depois digite o comando "cd" seguido do caminho do diretório onde se encontra o arquivo baixado.
Se você baixou o arquivo no diretório padrão de Downloads então terá que executar algo parecido com isso:
<br>
<pre>
  <code>
cd C:\Users\UserName\Downloads
  </code>
</pre>

Você também poderá mover o arquivo para dentro de qualquer diretório de sua preferência antes de executá-lo, desde que acesse esse diretório posteriormente pelo terminal.

Para executar o arquivo basta digitar a seguinte linha de comando e teclar "Enter" na sequência:<br>
<sup>É necessário o módulo requests do Python para executar o instalador, se não o tiver instalado execute <i>pip install requests</i> antes de iniciar a instalação.</sup>
<pre>
  <code>
python neuraline_installer.pyc
  </code>
</pre>
<sup>Observação: certifique-se de estar logado com a conta de administrador do seu sistema, caso contrário execute o arquivo como administrador.</sup><br>

Aguarde o término da instalação até que a mensagem "installation completed successfully" seja exibida.
Se você fez tudo corretamente até aqui, terá algo parecido com isso:

<pre>
  <code>
.................starting installation
.......................processing data
downloading, please wait..............
......package downloaded successfully.
...............installing dependencies
..installation completed successfully.
  </code>
</pre>

Ok! O Neuraline foi instalado com sucesso, mas você ainda não conseguirá utilizar os recursos profissionais de forma completa caso não valide a sua assinatura.
Para assinar a licensa profissional e liberar todos os recursos, siga as etapas abaixo.

* <b><a id="step1">passo 1</a> (para usuários Linux depois de baixar os fontes siga a partir daqui, para usuários Windows que estiverem usando o instalador siga as etapas acima antes de continuar daqui para frente ou simplesmente comece daqui se você baixou os fontes diretamente do repositório):</b> conectado a internet, execute a janela de inscrição de assinatura na sua máquina local com o código a seguir.<br>
<sup>Se você estiver usando os fontes diretamente da sua pasta de projetos sem o instalador execute primeiro o código para instalação de dependências, você pode encontrá-lo <a href="https://github.com/aiquantumneuro/instalacao_do_neuraline/blob/main/instalacao_de_dependencias.py">aqui</a>. Como no Linux você não usa o instalador das etapas acima então a instalação prévia das dependências é obrigatória. No Linux te aconselhamos a instalar as dependências duas vezes, sem o “sudo” e com o “sudo” para evitar problemas durante o desenvolvimento. Se a sua versão do Linux não vier com o Pip instalado você poderá instalá-lo executando <i>sudo add-apt-repository universe</i> e depois <i>sudo apt install python3-pip</i></sup>

<pre>
  <code>
'''
Observação: Não execute este código no Jupyter Notebook ou em qualquer outro notebook.
Para que a janela seja exibida, o código deverá ser executado em um arquivo único por linha de comando.
'''
from Neuraline.Utilities.subscribe import Subscribe
Subscribe().subscribe()
  </code>
</pre>
<sup>Observação: lembre-se de que é uma biblioteca de códigos Python, logo todos os códigos deverão ser executados com o Python.
Você poderá criar um arquivo para cada código a ser executado e executá-los com o comando "python" seguido do nome do arquivo .py,
ou simplesmente executar os códigos linha a linha através do IDLE.</sup><br><sup>A janela de inscrição usa o runtime do Chrome, então você precisará ter o <a href="https://www.google.com/intl/pt-BR/chrome/">Chrome</a> ou o <a href="https://www.chromium.org/getting-involved/download-chromium/">Chormium</a> instalado na sua máquina, caso contrário a janela de inscrição não abrirá. Se por algum motivo você não conseguir executar a janela de inscrição clique <a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=3KU8UE3HVYPAS">aqui</a> e acesse o nosso link alternativo diretamente do PayPal, mas só faça isso se a janela de inscrição da biblioteca não abrir.</sup>

<div align="center"><img src="https://github.com/grupoquantum/instalacao_do_neuraline/blob/main/subscribe01.png"></div>

* passo 2: preencha o primeiro campo do formulário com o seu nome verdadeiro completo e no segundo campo escolha o seu país de residência. Depois de preencher os dois campos clique no botão "Next >>".

<div align="center"><img src="https://github.com/grupoquantum/instalacao_do_neuraline/blob/main/subscribe02.png"></div>

* passo 3: clique em um dos botões de assinatura do PayPal e na janela de autenticação do PayPal preencha as informações requisitadas com os seus dados de pagamento e confirme.
Com exceção da China, o nome do usuário do PayPal que receberá o pagamento poderá variar de acordo com o país e a região na qual você se encontra, não se preocupe, pois todas as transações são certificadas pelo próprio PayPal e protegidas por criptografia.
Ao concluir o pagamento da assinatura, será baixado um arquivo de nome "subscription.key". Este arquivo será o responsável por validar a sua assinatura com a chave serial de validação e liberar todos os recursos do Neuraline na sua máquina local.<br>
<sup>Observação: o arquivo subscription.key é particular, se alguém além de você utilizar a sua chave, você terá os seus recursos bloqueados, então guarde-o com segurança.</sup><br>

* passo 4: (FINAL) - conectado a internet, execute o código de validação de assinatura informando o arquivo "subscription.key" que foi baixado no valor do parâmetro "url_path". 
Se o retorno for <b>True</b> com a mensagem "<b>Signature SUCCESSFULLY VALIDATED!</b>", a sua assinatura terá sido validada com sucesso e todos os recursos profissionais da biblioteca de códigos serão liberados sem restrição.

<pre>
  <code>
from Neuraline.Utilities.subscribe import Subscribe
'''
Endereço com o diretório onde se encontra o arquivo baixado
seguido do nome do arquivo ("subscription.key").
'''
url_path = 'C:/Users/UserName/Downloads/subscription.key' # exemplo de endereço
print(Subscribe().validateSignature(url_path=url_path))
  </code>
</pre>
<sup>Observação: os códigos do Neuraline são códigos profissionais compilados e criptografados com engenharia fechada.
Por esse motivo você não conseguirá executálos em ambientes virtuais como os de notebooks por exemplo.
Também não recomendamos que você tente editá-los, pois neste caso os desenvolvedores responsáveis tem mecanismos para fazer o seu rastreamento e processá-lo judicialmente.</sup><br>
<sup><i>* Você poderá mover e/ou copiar o Neuraline a vontade desde que seja na mesma máquina onde a inscrição foi feita, caso contrário a sua licença será bloqueada e a biblioteca deixará de funcionar.</i></sup><br>

Com a instalação e validação concluídas você já poderá utilizar todos os recursos de Neurociência Computacional, Inteligência Artificial, Física Computacional e Computação Quântica da ferramenta.
Como os algoritmos são códigos fechados nós não recomendamos a utilização de IDEs invasivas com recursos de autocomplete para módulos, 
neste caso a nossa recomendação é de que você codifique com IDEs de código texto como o <a href="https://www.sublimetext.com/">Sublime Text</a> ou o <a href="https://atom.io/">Atom</a> por exemplo (não recomendamos o VS Code), 
você também poderá codificar com o próprio IDLE sem problemas. No <a href="https://atom.io/">Atom</a> recomendamos a utilização do pacote <a href="https://atom.io/packages/search?q=platformio-ide-terminal">platformio-ide-terminal</a> para Windows por que o terminal padrão não costuma exibir alguns símbolos especiais da computação quântica.

<div align="center"><img src="https://github.com/grupoquantum/instalacao_do_neuraline/blob/main/logos.png"></div>

<sub>Confira algumas das empresas, organizações ou instituições de ensino que utilizam o algoritmo completo ou módulos dele:
SpaceX, Boston Dynamics, Blue Origin, Huawei, Xiaomi, ByteDance, University of Zurich, University of Vienna, Peking University...
O nome Neuraline refere-se apenas aos módulos de distribuição pública e o direito autoral é de propriedade dos desenvolvedores.</sub>
</div>

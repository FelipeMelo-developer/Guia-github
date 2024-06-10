
# Anotações
<img src="https://media.baamboozle.com/uploads/images/643821/1664765202_566108_gif-url.gif" alt="esperando" align="right" alt="yoda" width="15%" height=auto>


Versionamento:

◈ Registro de mudanças em arquivos, que possibilita recuperação ou acesso a versão anteriores;

◈ Possibilitando desenvolvimento de código em colaboração com outros integrantes.





# O que é git:

Git é um sistema de versionamento de código, que guarda os registros de versão como <b>snapshots</b> (fotos) do estado do projeto, além da referência/caminho para essa foto.

----
# Intalação:
<img src="https://www.icegif.com/wp-content/uploads/2022/04/icegif-621.gif" alt="esperando" align="left" alt="yoda" width="20%" height=auto>
◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈

Link para dowload do Git: https://git-scm.com/downloads

◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈ ◈

# Criando um repositorio no Github:

Readme: Pagina inicial do nosso repositorio, um arquivo onde podemos por algumas considerações iniciais, links uteis e etc..
gitignore: Arquivo que pode ser colocado para ignorar alguns arquivos que não são excenciais
Licença: Pode ser colocado é opcional.

### O Git Bash é um terminal extendido para otimizar o uso do Git.

Dentro da pasta onde deseja criar o repositorio local clique com botão direito do mouse e abra o Git Bash:

<pre class="prettyprint"><code class="hljs language-csharp">$ git clone <span class="hljs-keyword">+</span> endereço de repositorio remoto.
</code><button type="button" class="clipit"></button></pre>

Para entrar dentro da pasta coloque:

<pre class="prettyprint"><code class="hljs language-csharp">$ cd <span class="hljs-keyword">+</span> nome da pasta.
</code><button type="button" class="clipit"></button></pre>

#### Verificar o status:

<pre class="prettyprint"><code class="hljs language-csharp">$ git <span class="hljs-keyword"></span>status
</code><button type="button" class="clipit"></button></pre>

Ao executá-lo é exibido na tela informações sobre as alterações feitas nos arquivos app.js e index.html do projeto e que essas mudanças que precisam ser registradas no commit.


#### Para enviar o arquivos para controle de versão local(todos os arquivos):
<pre class="prettyprint"><code class="hljs language-csharp">$ git <span class="hljs-keyword"></span>add .
</code><button type="button" class="clipit"></button></pre>

Feito isso, provavelmente os arquivos foram adicionados Para conferir, rodamos novamente o git status.

#### Verificando o status novamente

<pre class="prettyprint"><code class="hljs language-csharp">$ git<span class="hljs-keyword"></span> status
</code><button type="button" class="clipit"></button></pre>

Repare que ao fazer isso, notamos no terminal que a ferramenta indica que existem alterações para serem comitadas e quais foram os arquivos modificados. Além disso, a cor mudou para verde, isso significa que os arquivos foram adicionados corretamente.

Agora que você já adicionou, podemos fazer o commit, que é o comando responsável por registrar uma modificação no código.

#### Para commitar o arquivo em nuvem:

<pre class="prettyprint"><code class="hljs language-csharp">$ git commit <span class="hljs-keyword">-m</span> "texto comentario do commit que faz sentido para o que esta sendo enviado"
</code><button type="button" class="clipit"></button></pre>

Como retorno é informado que o commit foi realizado com sucesso.
Importante ressaltar que, quando fazemos um commit é como se estivéssemos registrando uma versão do nosso sistema. Se estávamos na versão 1, passamos para a versão 2, depois para a versão 3, 4, 5, e assim por diante.

Um commit deve ser realizado sempre que você finalizar uma tarefa específica ou resolver algum bug. Isso mantém o histórico de commits claro e rastreável, de modo que seja possível entender o que foi feito em cada commit.

#### verificando versão
Existe um comando em que conseguimos identificar quais commits foram realizados no projeto e quem fez. Para isso, podemos utilizar o comando git log.

<pre class="prettyprint"><code class="hljs language-csharp">$ git<span class="hljs-keyword"></span> log
</code><button type="button" class="clipit"></button></pre>

Ao executá-lo é exibido o histórico dos commits que foram feitos ao longo do projeto.

Se analisarmos o retorno, retonhamos o primeiro commit que foi feito para subir o projeto inicial. Identificamos o nome do autor, data seguido da mensagem. Logo acima temos o commit mais atual que é o que acabamos de fazer.
Observe que o git log mostra o log, ou seja, o histórico de commits realizados no projeto. Assim, podemos identificar quem foi que fez cada registro, a mensagem, o significado de cada registro, a data e toda essa sequência de alterações no repositório.

<pre class="prettyprint"><code class="hljs language-csharp">$ git<span class="hljs-keyword"></span> remote
</code><button type="button" class="clipit"></button></pre>

#### Enviando para o GitHub
Para enviar para nuvem precisar ser dado um push

<pre class="prettyprint"><code class="hljs language-csharp">$ git push origin<span class="hljs-keyword"></span> (main ou master)
</code><button type="button" class="clipit"></button></pre>

Utilize o comando git push para enviar os commits do repositório local ao repositório remoto no GitHub

#### Baixando do GitHub

<pre class="prettyprint"><code class="hljs language-csharp">$ git pull origin<span class="hljs-keyword"></span> (main ou master)
</code><button type="button" class="clipit"></button></pre>

O comando git pull origin main é utilizado para baixar os commits do repositório remoto para o repositório local.

---

# O comando git remote

### 1 - Adicionar um repositório remoto:

Quando você deseja estabelecer uma conexão entre seu repositório local e um repositório remoto, como aquele hospedado no GitHub, o comando git remote add é a ferramenta essencial. Essa etapa é crucial para possibilitar a colaboração e o compartilhamento de código com outras pessoas, bem como para fazer backup de seu trabalho em um servidor remoto.

A sintaxe básica do comando é a seguinte:

<pre class="prettyprint"><code class="hljs language-csharp">git remote <span class="hljs-keyword">add</span> apelido url
</code><button type="button" class="clipit"></button></pre>

'apelido': Este é um nome que você atribui ao repositório remoto. Geralmente, se utiliza nomes descritivos, como "origin" para o repositório principal no GitHub, mas você pode escolher nomes que façam sentido para o seu projeto.

'url': Aqui, você insere a URL do repositório remoto. Esta URL é única para cada repositório remoto e serve como o endereço para acessar e interagir com ele pela internet. Certifique-se de copiar a URL correta do repositório que deseja adicionar.

### 2 - Listar os repositórios remotos:

Para listar os repositórios remotos associados ao seu projeto local, você pode utilizar o comando git remote -v. Isso exibirá uma lista de todos os repositórios remotos vinculados ao seu projeto, juntamente com suas URLs. Veja um exemplo:

<pre class="prettyprint"><code class="hljs language-undefined">git remote -v
</code><button type="button" class="clipit"></button></pre>

A saída será algo semelhante a:
<pre class="prettyprint"><code class="hljs language-perl">origin   https:<span class="hljs-regexp">//gi</span>thub.com/seu-usuario/seu-projeto.git (fetch)
origin   https:<span class="hljs-regexp">//gi</span>thub.com/seu-usuario/seu-projeto.git (<span class="hljs-keyword">push</span>)
</code><button type="button" class="clipit"></button></pre>

Essa lista é útil para verificar se os repositórios remotos estão configurados corretamente. Obs: Vai aparecer duplicado mesmo, pois o Git separa a url de envio de commits (push) da url de baixar commits (fetch).

### 3 - Remover um repositório remoto:

Caso você não precise mais de um repositório remoto específico, pode removê-lo com o comando git remote remove apelido. Substitua 'apelido' pelo nome do repositório remoto que deseja remover. Aqui está um exemplo:

<pre class="prettyprint"><code class="hljs language-csharp">git remote <span class="hljs-keyword">remove</span> origin
</code><button type="button" class="clipit"></button></pre>

Após a execução deste comando, o repositório remoto chamado "origin" será desvinculado do seu projeto local.

### 4 - Alterar a URL de um repositório remoto:

Às vezes, é necessário atualizar a URL de um repositório remoto, como quando a URL do servidor do GitHub é modificada ou quando você copiou a URL incorreta ao adicionar o repositório remoto. Use o comando git remote set-url apelido nova_url para realizar essa atualização. Substitua 'apelido' pelo nome do repositório remoto e 'nova_url' pela nova URL que você deseja associar a ele. Aqui está um exemplo:
<pre class="prettyprint"><code class="hljs language-cpp">git remote set-url origin https:<span class="hljs-comment">//github.com/seu-usuario/seu-repositorio.git</span>
</code><button type="button" class="clipit"></button></pre>


Isso atualizará a URL do repositório remoto "origin" para a nova URL especificada.

### 5 - Alterar o apelido de um repositório remoto:

Se você deseja renomear um repositório remoto, use o comando git remote rename apelido novo_apelido. Substitua 'apelido' pelo nome atual do repositório remoto e 'novo_apelido' pelo novo nome que você deseja atribuir a ele. Aqui está um exemplo:

<pre class="prettyprint"><code class="hljs language-lua">git remote <span class="hljs-built_in">rename</span> origin novo-origin
</code><button type="button" class="clipit"></button></pre>

Isso renomeará o repositório remoto de "origin" para "novo-origin".

Lembre-se de que o comando git remote é fundamental para a gestão de conexões entre seu repositório local e repositórios remotos, permitindo a colaboração eficiente e o controle de versão. 

### 6 - Ver o que foi modificado

<pre class="prettyprint"><code class="hljs language-lua">git diff<span class="hljs-built_in"></span>
</code><button type="button" class="clipit"></button></pre>
----

# Sinalizações em arquivos do VSCode

Quando estamos trabalhando em um projeto utilizando o versionamento Git e a IDE VSCode, ao adicionar ou alterar algum arquivo aparece uma sinalização ao lado do nome desses arquivos no VSCode, como podemos ver na imagem abaixo:

<img src="https://cdn1.gnarususercontent.com.br/1/1221554/5afdb0f3-f5cc-46b3-88f6-0062f51cbc0c.png" alt="Imagem com print do VSCode, da lateral esquerda que lista a estrutura de arquivos do projeto. Na imagem temos um arquivo chamado index.html com a sinalização de uma letra M ao lado direito e um arquivo chamado README.md com a sinalização de uma letra U ao lado direito.">

Mas o que isso significa?

M: A letra M representa o estado Modified, do português modificado. Isso significa que o arquivo já existia no repositório, mas que recebeu alguma modificação que ainda não foi registrada no Git.

U: A letra U representa o estado Untracked, do português não rastreado. Isso significa que o arquivo ainda não existia no repositório e que ainda não teve seu registro (commit) feito no Git.

Essa sinalização nos ajuda a entender o estado atual dos nossos arquivos do projeto no versionamento Git.


# Adicionando Colaboradores ao projeto

Settings > Collaborators > add people

<img src="https://64.media.tumblr.com/862b20bc85080ab4f15894eabe39749d/b4563749ec65009e-35/s540x810/3d993e34b6ab266982e89efd4d3992ee8134bc2f.gif" alt="bye" align="center" alt="yoda" width="50%" height=auto>

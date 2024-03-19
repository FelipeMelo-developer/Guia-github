
# Anotações

Uma breve descrição sobre o que esse projeto faz e para quem ele é

----

Link para dowload do Git: https://git-scm.com/downloads

O Git Bash é um terminal extendido para otimizar o uso do Git.


Criando um repositorio no Github:

Readme: Pagina inicial do nosso repositorio, um arquivo onde podemos por algumas considerações iniciais, links uteis e etc..
gitignore: Arquivo que pode ser colocado para ignorar alguns arquivos que não são excenciais
Licença: Pode ser colocado é opcional.

1-  Dentro da pasta onde deseja criar o repositorio local clique com botão direito do mouse e abra o Git Bash:

$ git clone + endereço de repositorio remoto.

2 - Para entrar dentro da pasta coloque:
$ cd + nome da pasta.

Verificar o status:
$ git status

Para enviar o arquivos para controle de versão local(todos os arquivos):
$ git add .

Verificar o status
$ git status

Para commitar o arquivo em nuvem:
$ git commit -m "texto comentario do commit que faz sentido para o que esta sendo enviado"

Para enviar para nuvem precisar ser dado um push:
$ git push origin (main ou master)

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

----






<h1 align="center">Guithub</h1>

<h2 align="center">Git Bash: Como instalar e usar o terminal do Git no Windows</h2>

<h3 align ="center">CASO AS IMAGENS NÃO CARREGUE, ACESSAR PASTA IMG SE SURGIR DUVIDAS</h3> 


<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://github.com/Ceratti/FontesProtheus/tree/main/img/one.png" alt="gitBash"></a>
</p>


Git é o sistema de controle de versões mais usado no mundo da programação. Tanto no cenário open-source, 
com o GitHub dominando como plataforma de distribuição e colaboração de códigos, quanto no mundo corporativo, 
onde grandes empresas utilizam repositórios privados de Git para controlar a evolução de códigos criados e 
modificados por seus colaboradores.

<h1 align="center"> 1) Como instalar o Git Bash</h1>

O Git Bash faz parte do pacote Git for Windows, que é oferecido no próprio site oficial do Git, em: <a target="_blank" rel="nofollow noopener" href="https://git-scm.com/download/win">https://git-scm.com/download/win</a>

O pacote inclui o próprio Git, o Git Bash e o Git GUI, uma interface gráfica para o Git.

<h2 align ="center">Instalando o Git no windows</h2>

<p>No site oficial do <strong>Git</strong> (<a target="_blank" rel="nofollow noopener" href="http://git-scm.com/">http://git-scm.com/</a>) clique em “<strong>Downloads for Windows</strong>”.</p>


<p>Execute o arquivo baixado e vá dando “<strong>Next</strong>” até a tela “<strong>Select Components</strong>”. Nesta tela eu escolho as opções PADRÃO que já vem selecionada como na imagem: </p>

<p align="center">
        <a href="" rel="noopener">
    <img width=200px height=200px src="https://github.com/Ceratti/FontesProtheus/tree/main/img/two.png" alt="next"></a>
</p>

<p align="center">
        <a href="" rel="noopener">
    </img width=200px height=200px src="https://github.com/Ceratti/FontesProtheus/tree/main/img/tree.png" alt="install"></a>
</p>


<p>Em especial eu marco as opções em “<strong>Windows Explorer integration</strong>”, assim eu consigo abrir o prompt de comandos do Git Bash em qualquer pasta, basta clicar com o botão direito e “<strong>Git Bash Here</strong>”. A última opção também é interessante, porque ele instala uma fonte melhorzinha para o prompt de comandos.</p>

<p><strong>Nota:</strong>O Git para Windows vem com um prompt de comandos próprio Git Bash, que além dos comandos git também fornece alguns comandos Unix que podem ser bem úteis (além de ser bem mais bonitinho que o prompt de comandos padrão do Windows).</p>

<p>Na próxima tela, eu escolho a opção: “<strong>Use Git from the Windows Command Prompt</strong>”.</p>

<p align="center">
        <a href="" rel = "noonpener">
    <img width=200px height=200px src="https://github.com/Ceratti/FontesProtheus/tree/main/img/four.png" alt="option "></a>
</p>


<h1 align="center"> 2) Clonando um repositório </h1>


<p> Abra o <em><b>Git Bash</b></em> e crie uma pasta chamada Github onde salvaremos nossos projetos baixados de lá.
Pra criar a pasta, digite o comando:
</p>

<pre><code>mkdir Github</code></pre>

Entrando na pasta criada, digite o código abaixo e precione o <b><em>ENTER</em></b>:

<pre><code>cd Github</code></pre>

Acesse o nosso repositório do <b><em>Github</em></b><b>(FontesProtheus)</b> para executar o processo conhecido como clonar um repositório.
Acesse o repositório <b>(FontesProtheus)</b> na parte superior clicar no botão <b>(CODE)</b>, após isso copiar a <b><em>URL https</em></b> 
caso de duvida e não aparecer a imagem acessar a pasta (img) e analisar a imagem chamada <b>(repositório).</b>

<p align="center">
        <a href="" rel = "noonpener">
    <img width=200px height=200px src="https://github.com/Ceratti/FontesProtheus/tree/main/img/repositorio.png" alt="repositorio"></a>
</p>

Após copiado a <b><em>URL https</em></b>, digirtar o comando abaixo no <b>GitBash</b>:

<pre><code> git clone https://github.com/Ceratti/FontesProtheus.git </code></pre>

Pode demorar um pouquinho, mas só aguardar o terminal do Gitbash.

#### Agora, basta abrir o vscode no mesmo local que foi feito o clone do repositório.


<h1 align="center"> 3) Principais comando do gitBash que vamos utilizar: </h1>

<ul>
<pre><code><li>git add + < arquivo / pasta > </li></pre></code>    
    
<p>Quando um repositório é inicialmente clonado, todos os seus arquivos estarão monitorados e inalterados porque você simplesmente os obteve e ainda não os editou. Conforme você edita esses arquivos, o Git passa a vê-los como modificados, porque você os alterou desde seu último commit. Você seleciona esses arquivos modificados e então faz o commit de todas as alterações selecionadas e o ciclo se repete.</p>

<pre><code><li> git status </li></pre></code>
<p>O comando lhe mostra em qual branch você se encontra. Vamos dizer que você adicione um novo arquivo em seu projeto, um simples arquivo <b>README</b>. Caso o arquivo não exista e você execute <b>git status</b>, você verá o arquivo não monitorado dessa forma.
</p>

<p>Você pode ver que o seu novo arquivo README não está sendo monitorado, pois está listado sob o cabeçalho "Untracked files" na saída do comando status. Não monitorado significa basicamente que o Git está vendo um arquivo que não existia na última captura (commit); o Git não vai incluí-lo nas suas capturas de commit até que você o diga explicitamente que assim o faça. Ele faz isso para que você não inclua acidentalmente arquivos binários gerados, ou outros arquivos que você não têm a intenção de incluir. Digamos, que você queira incluir o arquivo README, portanto vamos começar a monitorar este arquivo.
</p>

<pre><code><li> git diff </li></pre></code>

<p>Se o comando <b>git status</b> for muito vago — você quer saber exatamente o que você alterou, não apenas quais arquivos foram alterados — você pode utilizar o comando.</p>

<p>Apesar do comando <b>git status</b> responder essas duas perguntas de maneira geral, o <b>git diff</b> mostra as linhas exatas que foram adicionadas e removidas — o patch, por assim dizer.
<br>Se você quer ver o que selecionou que irá no seu próximo commit, pode utilizar:</p>

<pre><code> git diff --cached </pre></code>

<pre><code><li> git commit </li></pre></code>

<p>Armazena o conteúdo atual do índice em um novo commit, juntamente com uma mensagem de registro do usuário que descreve as mudanças.
<br>Se usa o commit depois de já ter feito o <b>git add</b>, para fazer o commit:</p>

<pre><code> git commit -m "COMENTÁRIO DO QUE FOI FEITO ANTES DE SUBIR PARA O REPOSITÓRIO"</pre></code>

<p>Refazendo commit quando esquecer de adicionar um arquivo no Stage:</p>

<pre><code>git commit -m "mensagem" --amend</pre></code>

<p>O amend é destrutivo e só deve ser utilizado antes do commit ter sido enviado ao servidor remoto.</p>

<pre><code><li> git push </li></pre></code>

<p><b>O git push</b> é o comando em que você transfere commits a partir do seu repositório local para um repositório remoto. É a contrapartida do <b>git fetch</b>, que busca importações e comprometem as agências locais, utilizando o <b>git push</b> as exportações comprometem as filiais remotas. Para fazer isso, você executa <b>git push [nome_do_repositório_remoto] [nome_da_sua_branch_local]</b>, que vai tentar fazer que o <b>[nome_do_repositório_remoto]</b> receba a sua branch <b>[nome_da_sua_branch_local]</b> contendo todos seus commits com alterações. Por exemplo:</p>

<pre><code>git push -u origin main</pre></code>

<p> Casso a hora de puxar o arquivo do seu local para o Git der algum erro, ex: </p> 

<pre>
<code>To https://github.com/Ceratti/FontesProtheus.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Ceratti/FontesProtheus.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
</code>  
</pre>

<p>Executar o seguinte comando para resolver o erro: </p>

<pre><code>git pull</pre></code>
 
<p>E em seguida executar novamente o comando: </p>
<pre><code>git push -u origin main</pre></code>

<p>Após isso acessar o repositório no site e verá que toda alteração já está na "nuvem" do gitHub </p>
</ul>



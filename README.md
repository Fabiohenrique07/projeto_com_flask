Documentaçã aula dia 21/10/2026 / projeto_com_flask
 
1- O código importa ferramentas do Flask para criar o site, pegar informações da URL e chamar arquivos HTML. O `escape` ajuda na segurança.
 
2.
python app = Flask(__name__) 
Cria a aplicação que vai ser usada no projeto.

3- python
@app.rote("/")
def ola_mundo():
    return '<p>Olá, mundo!</p>'
-- Define a página principal e mostra a mensagem Olá, mundo!.
 
4 -O `request.args.get()` pega o nome informado na URL. Se não tiver nome, usa Flask como padrão.
 
5- Rota de usuári `/usuario/<uername>` pega o nome colocado no caminho e mostra na tela.

6- Usando HTML o `render_template` chama o arquivo `ola.html` e envia o nome para ele.

7- O Arquivo HTML monta a página, usa `if` e `else` para verificar se tem nome. Se tiver, mostra ele; se não, aparece Olá, Flask!.

8- Executando o `app.run()` inicia o servidor na porta 5000, permitindo acessar o site pelo navegador.
serve para criar páginas, usar rotas e mostrar informações no HTML

------------------------------------------------ comandos para instalar uv ------------------------------------------------------

 powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"  
 uv -V
 uv python install 3.15.0
 uv init
 uv venv
 python -V
 uv sync
 uv add Flask
 uv run flask run 
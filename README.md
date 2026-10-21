# Projeto com Flask

* Criamos uma pasta chamada **projeto_com_flask** e depois criamos um arquivo chamado **app.py**
  

## **Com instalar e configurar o uv na sua máquina virtual no VScode**



* Para instalar o uv no VScode vai precisar acessar o site: **https://docs.astral.sh/uv/** ;
* Após acessar o site selecione a opção intallation utilizamos o código: ``` powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"```  para copiar no terminal do VScode
  
**OBS: Esse código só funciona no terminal do PowerShell**



## **Configuração uv**

* Após intalar o uv terá que colocar o seguinte código: ```uv init``` para a inicialização do uv
*Com o uv já iniciado verifique a versão do python com o código: ```uv -V```
* Se a versão for menor que 3.15.0 instale com o seguinte código: ```uv python install 3.15.0```

## **Iniciando o ambiente virtual**

* Para iniciarmos o ambiente virtual precisa inserir o código: ```uv venv```

## **Importação do Flask e markupsafe**

* Importamos o Flask e markupsafe para 	utilizar no arquivo python

## **Usando snippets**

* Utilizamos snippets no código do app.py:
```
    app = Flask(__name__)

    @app.route("/")
    def ola_mundo():
        return '<p>Olá, mundo!</p>'
```

## **Criação de condição**

Criamos uma condição para que o código não execute sozinho e inicie com flask antes, segue abaixo:

```
if name == "main": app.run(debug=False, port=5000)
```

## **Criando a pasta templates e ola.html**

* Criamos um código no html para o python:
```
{% if nome %} 

**Olá, {{nome}}!**

{% else %}

**Olá, Flask**

{% endif %}
```
No final é preciso usar o ```{% endif %}```, porque é utilizada para indicar o fim de uma estrutura de repetição no Python dentro do HTML.








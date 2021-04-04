# Introdução a programação em Python

Este repositório tem a finalidade armazenar os arquivos utilizados como apoio aos minicursos de introdução a programação em Python.

###  Baixando arquivos
Os arquivos poderão ser baixados clicando em `code` e `Download Zip` ou utilizando a linha de comando do [Git](https://git-scm.com/):

    git clone https://github.com/flaviofilipe/introducao-ao-python.git

###  Notebooks
Os *notebooks* são arquivos utilizados pelo [Jupyter Notebook](https://jupyter.org/), plataforma web para programar de forma interativa. Eles podem ser criados tanto para estudo quanto para produção, gerando documentos e relatórios.

###  [Google Colab](https://colab.research.google.com/)
O [Google Colab](https://colab.research.google.com/) é uma ótima alternativa para quem quer criar seus *notebooks* sem precisar configurar um ambiente na sua máquina local. Ele é muito recomendado tanto para quem está aprendendo quanto para quem precisa gerar relatórios e/ou documentos a partir do código.
Saiba mais sobre como usá-lo [aqui](https://www.alura.com.br/artigos/google-colab-o-que-e-e-como-usar).

**Importar notebooks**
Você poderá importar os notebooks no Google Colab no menu **Arquivo** na opção **Fazer upload de notebook**. Ao escolher o arquivo ele será salvo no seu Google Driver.

**Abrir outros notebooks existentes**
Após criar vários ou fazer o upload de outros notebooks basta ir no menu **Arquivo**, selecionar a opção **Abrir Notebook** e escolher qual você quer editar.

**Salvar como PDF**
Você poderá baixar o arquivo para sua máquina no formato py (Python) ou ipynb (Jupyter Notebook). Porém caso queira exportar o arquivo no formato PDF basta ir no menu **Arquivo** e clicar em **Imprimir** e salvá-lo.

#  Configurando ambiente local
> Este projeto foi testado na versão 3+ do Python.
- Baixo o Python 3.x [aqui](https://www.python.org/downloads/).

> :warning: OBS: Ao instalar no Windows marque a opção de adicionar ao path. Sem isso não será possível executar os comandos a seguir

![enter image description here](https://dicasdepython.com.br/images/como-instalar-python-no-windows-10/instalador-python-01-selecao-do-tipo-de-instalacao.png)

**Execute os códigos a baixo no terminal (linux) ou no CMD (Windows)**

    python3 --version

Caso esteja no Windows e o comando a cima dê erro, poderá testar desta forma:

    py --version

O resutado deverá ser algo como

    Python 3.x.x

Onde o x será os números da versão. Caso apareça o *2* na versão procure instalar a versão 3 mais atualizada.

###  pip
O Python utilzia o *pip* para baixar outras bibliotecas (conjunto de códigos já pronto). Verifique se o pip já está instalado na sua máquina com o comando
`pip3 --version` ou  `pip --version`. A saída desses comandos deverá mostrar a versão do *pip* e do Python.

> :warning: Verifique se a versão do Python nessa saída é > 3.

## Ambiente isolado como Virtualenv
Uma boa prática do Python é isolar o ambiente de desenvolvimento separado por projeto, assim, todas as coisas que estiverem baixadas no projeto não irá afetar outros. A grande vantagem é que poderá utilizar versões diferentes de bibliotecas em vários projetos.

Veja como utilizar o **venv** [aqui](https://docs.python.org/pt-br/3/library/venv.html).

###  Criando ambiente virtual
Vamos criar nosso *virtualenv* (venv) com o nome de *venv*. Execute o comando a baixo:

    python3 -m venv venv

Ou no Windows

    py -m venv venv

Assim nós estaremos criando uma pasta chamadas *venv* dentro da pasta atual onde será salvo todas as dependências do projeto.

Execute os comandos a baixo na raiz do seu projeto.
Para ativá-las execute no Windows:

    venv\Scripts\activate

Ou no Linux:

    source venv/bin/activate

###  Instalando as dependências
Há um padrão utilizado no Python para salvar as depencias (bibliotecas) necessárias para baixar dentro do arquivo *requirements.txt*. Sendo assim, com o venv ativo e usando o seu terminal, execute o comando a baixo:

    pip install -r requirements.txt

Verifique se o Jupyter foi instalado corretamente utilizando o comando a baixo no terminal do venv:

    jupyter-lab

Caso tudo ocorra bem ele abrirá uma página muito parecida com a do Google Colab com os arquivos;

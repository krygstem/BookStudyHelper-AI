Este código é um programa em Python que realiza a leitura de arquivos PDF e DOCX, resumindo seu conteúdo de acordo com as preferências do usuário. O programa utiliza a API do OpenAI para gerar resumos e títulos resumidos, além de adicionar informações adicionais como um dicionário de palavras-chave, cronologia e perguntas de sim ou não.

Aqui está uma explicação detalhada do que cada parte do código faz:

Importação de bibliotecas: O código importa várias bibliotecas, como os, time, OpenAI, PdfReader, Document, tkinter, tqdm, datetime, json e tiktoken. Essas bibliotecas são usadas para realizar tarefas como leitura de arquivos, manipulação de documentos, interação com o usuário, cálculos de tempo e tokenização de texto.

Configuração do cliente OpenAI: O código configura o cliente OpenAI com a chave de API fornecida. Isso permite que o programa faça chamadas à API do OpenAI para gerar resumos e títulos resumidos.

Funções auxiliares: O código define várias funções auxiliares, como gerar_titulo_resumido, salvar_progresso, carregar_progresso, perguntar_continuar, escolher_arquivos, criar_janela_selecao, escolher_publico, pedir_profissao, escolher_tokens_entrada, escolher_tokens, escolher_tokens2, escolher_cronologia, escolher_perguntas, escolher_numero_perguntas, ler_arquivo, resumir_texto, resumir_texto2, calcular_custos e substituir_caracteres. Essas funções são usadas para realizar tarefas específicas, como ler arquivos, resumir texto, calcular custos e substituir caracteres.

Função principal (main): A função main é a função principal do programa. Ela gerencia o fluxo do programa, chamando as funções auxiliares conforme necessário. A função main também lida com a interação com o usuário, permitindo que o usuário escolha opções como o público-alvo, a quantidade de tokens de entrada e saída, e se deseja incluir cronologia e perguntas.

Execução do programa: O programa é executado chamando a função main se o script for executado diretamente.

Aqui está um fluxograma simplificado do programa:
Início
  |
  
  |---> Configurar cliente OpenAI
  
  |
  
  |---> Carregar progresso (se disponível)
  
  |
  
  |---> Perguntar se deseja continuar de onde parou
  
  |       |
  
  |       |---> Sim: Carregar configurações e continuar
  
  |       |
  
  |       |---> Não: Escolher arquivos, público-alvo, profissão, tokens de entrada, saída, cronologia e perguntas
  
  |
  
  |---> Ler arquivos
  
  |
  
  |---> Resumir texto (função `resumir_texto`)
  
  
  |
  
  |---> Resumir texto adicional (função `resumir_texto2`)
  
  |
  
  |---> Substituir caracteres especiais
  
  |
  
  |---> Gerar título resumido
  
  |
  
  |---> Salvar documento resumido
  
  |
  
  
  |---> Remover arquivo de progresso e temporário
  
  |

  
Fim

Instalação: 

Guia de Instalação para o Programa de Resumo de Texto (BookStudyHelper-AI)

Este guia irá guiá-lo através do processo de instalação e execução do programa de resumo de texto (BookStudyHelper-AI), assumindo que você não tem experiência prévia com Python ou programação.

Instale o Python

Acesse o site oficial do Python em https://www.python.org/downloads/
Baixe a versão mais recente do Python para o seu sistema operacional (Windows, macOS ou Linux).
Siga as instruções de instalação para o seu sistema operacional.
Verifique a Instalação do Python

Abra o terminal ou prompt de comando.
Digite python --version e pressione Enter.
Se a instalação foi bem-sucedida, você verá a versão do Python exibida no terminal.
Clone o Repositório do Programa

Abra o terminal ou prompt de comando.
Navegue até o diretório onde deseja clonar o repositório.
Digite git clone https://github.com/krygstem/BookStudyHelper-AI.git e pressione Enter.
Isso criará uma cópia local do repositório do programa.
Instale as Dependências do Programa

Navegue até o diretório do programa clonado.
Digite pip install openai PyPDF2 python-docx tkinter tqdm json tiktoken e pressione Enter.
Esse comando instalará todas as bibliotecas e pacotes necessários para executar o programa.
Obtenha uma Chave de API do OpenAI

Acesse o site da OpenAI em https://platform.openai.com/
Crie uma conta ou faça login.
Acesse a seção "API Keys" no painel de controle.
Clique em "Create new secret key" para gerar uma nova chave de API.
Copie a chave de API gerada.
Configure a Chave de API no Programa

Abra o arquivo main.py localizado no diretório do programa clonado em um editor de texto.
Localize a linha que contém api_key="YOUR API".
Substitua "sua_chave_de_api_aqui" pela chave de API que você copiou anteriormente.
Salve o arquivo.
Execute o Programa

Abra o terminal ou prompt de comando.
Navegue até o diretório do programa clonado.
Digite python main.py e pressione Enter.
Siga as instruções exibidas no programa para escolher os arquivos, configurar as preferências e salvar o resumo.



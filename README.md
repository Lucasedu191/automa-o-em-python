# Automação de Cadastro de Produtos

Este projeto tem como objetivo automatizar o processo de cadastro de produtos em um sistema web utilizando o **PyAutoGUI** para controle da interface gráfica e o **Pandas** para manipulação de arquivos CSV.
![image](https://github.com/user-attachments/assets/e38cd000-4af7-4573-8f74-13a000e9d025)


## Funcionalidades

- Login automatizado no sistema web.
- Importação de dados de produtos a partir de um arquivo CSV.
- Preenchimento automático dos campos do formulário de cadastro.
- Envio automático de cada cadastro ao sistema.
- Repetição do processo para todos os produtos da base.

## Requisitos

Para rodar o script de automação, você precisará ter as seguintes bibliotecas instaladas:

- `pyautogui`: Para automatizar as ações na tela.
- `pandas`: Para manipular o arquivo CSV contendo os produtos.

### Instalando as dependências

Você pode instalar as bibliotecas necessárias com o seguinte comando:

```bash
pip install pyautogui pandas


Como usar
1. Configuração Inicial
Antes de rodar o script, certifique-se de que o arquivo produtos.csv esteja no mesmo diretório do script Python e contenha os seguintes campos:

codigo: Código do produto.
marca: Marca do produto.
tipo: Tipo do produto.
categoria: Categoria do produto.
preco_unitario: Preço unitário do produto.
custo: Custo do produto.
obs: Observações sobre o produto (opcional).
2. Executando o Script
Abra o terminal ou o prompt de comando na pasta do projeto.
Execute o script Python:
bash
Copiar código
python cadastro_automacao.py
3. Capturando as Coordenadas
Para capturar as coordenadas da tela onde o PyAutoGUI precisa clicar, você pode rodar o script de captura de posição:

python
Copiar código
import time
import pyautogui

time.sleep(5)
print(pyautogui.position())
Isso imprimirá as coordenadas X e Y da posição atual do cursor após 5 segundos, permitindo que você ajuste os pontos de clique no código.

4. Automatizando o Login
O script abre o navegador e faz login no sistema web de forma automática. Basta preencher seu e-mail e senha diretamente no código na seção de login:

python
Copiar código
pyautogui.write("seu-email@gmail.com")
pyautogui.press("tab")
pyautogui.write("sua-senha")
5. Cadastrando os Produtos
O loop principal do script percorre cada linha do arquivo CSV e preenche os campos correspondentes no sistema de cadastro de produtos. Certifique-se de que os campos no sistema estejam alinhados com os dados no CSV.

Estrutura do Projeto
bash
Copiar código
/caminho-do-projeto
│
├── cadastro_automacao.py      # Script principal de automação
├── captura_posicao.py         # Script auxiliar para captura de posição do mouse
└── produtos.csv               # Arquivo CSV com a base de produtos
Contribuindo
Sinta-se à vontade para abrir um Pull Request ou reportar problemas se tiver sugestões de melhorias ou encontrar bugs!


markdown
Copiar código

### O que este `README.md` inclui:
- **Introdução ao projeto**: Uma breve explicação do que o projeto faz.
- **Funcionalidades**: Lista das principais funções do script.
- **Requisitos**: Dependências necessárias e como instalá-las.
- **Instruções de uso**: Como configurar e rodar o script.
- **Estrutura do projeto**: Descrição dos arquivos principais.
- **Contribuição**: Instruções para colaborar com o projeto.


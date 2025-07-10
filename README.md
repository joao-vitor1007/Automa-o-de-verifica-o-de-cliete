 Automação para Verificar Pagamentos de Clientes
Esse projeto eu desenvolvi para automatizar a verificação de pagamentos de clientes com base em uma planilha do Excel. A ideia foi facilitar o processo de conferir quem está em dia ou com pagamento pendente, usando Python e Selenium.

🚀 O que esse projeto faz
Lê os dados dos clientes a partir da planilha dados_clientes.xlsx.

Acessa automaticamente um site de consulta de CPF.

Verifica o status do CPF (se está em dia ou pendente).

Se estiver em dia, ele pega também a data e o método de pagamento.

Todos os resultados são salvos em uma nova planilha chamada planilha fechamento.xlsx.

No final, é só apertar Esc que o navegador fecha sozinho.

🛠️ Tecnologias e bibliotecas usadas
Python

openpyxl – para manipular as planilhas do Excel

selenium – para controlar o navegador e fazer a consulta no site

keyboard – para capturar a tecla Esc e encerrar o programa de forma prática

📂 Estrutura dos arquivos
app.py: é o código principal que faz tudo funcionar

dados_clientes.xlsx: onde eu coloco os dados dos clientes (nome, valor, CPF e vencimento)

planilha fechamento.xlsx: é gerada automaticamente com os resultados da consulta

▶️ Como usar
Coloque os dados dos clientes na planilha dados_clientes.xlsx, a partir da linha 2 (linha 1 é o cabeçalho).

Execute o script com o Python:


Copiar
Editar
python app.py
O sistema abre o navegador, consulta o CPF e grava as informações.

Quando quiser encerrar, é só apertar a tecla Esc.

⚠️ Observações importantes
Por enquanto, o código só lê um cliente por vez (o primeiro da lista). Se quiser que ele verifique todos da planilha, precisa adaptar o código para fazer um loop.

O site usado para consulta é o: https://consultcpf-devaprender.netlify.app

É necessário ter o ChromeDriver compatível com a versão do seu navegador Chrome.

💡 Por que fiz isso?
Fiz esse projeto como um exercício para aprender mais sobre automação com Python, manipulação de planilhas e uso de bibliotecas como Selenium. Foi bem útil para entender como integrar essas ferramentas.

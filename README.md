# Teste TrackLand
🍕 Papazitos - Sistema de Delivery
Papazitos é um sistema web de delivery de comida, construído com Python (Flask) e JavaScript. Ele permite que clientes vejam cardápios, façam pedidos e acompanhem o status, enquanto os restaurantes podem gerenciar seus produtos e pedidos recebidos.

✨ Features Principais
Autenticação de Usuários: Cadastro e Login separados para Clientes e Restaurantes.

Perfis de Usuário: Duas "caras" do sistema, uma para clientes e outra para restaurantes.

Cardápio do Cliente: Clientes podem navegar pelos restaurantes, ver produtos, adicionar itens a um carrinho persistente (usando localStorage) e finalizar o pedido.

Checkout Completo: Processo de finalização de pedido com cálculo de frete simulado e busca de endereço por CEP (via API ViaCEP).

Acompanhamento de Pedido: Cliente pode ver o status do seu último pedido em tempo real.

Gerenciamento do Restaurante: Painel para o restaurante gerenciar seus produtos (criar, editar, deletar - backend pronto) e ver os pedidos recebidos.

Atualização de Status: Restaurante pode atualizar o status de um pedido (Recebido, Em Preparo, Saiu para Entrega, etc.).

🛠️ Tecnologias Utilizadas
Backend: Python 3, Flask

Frontend: HTML5, CSS3, JavaScript (Vanilla)

Banco de Dados: SQLite 3

APIs Externas: ViaCEP 

🚀 Como Executar o Projeto
Siga os passos abaixo para rodar o projeto localmente.

1. Pré-requisitos
Python 3.7 ou superior

pip (gerenciador de pacotes do Python)

2. Instalação
1. Clone o repositório:

Bash

git clone https://seu-link-para-o-repositorio.git
cd nome-da-pasta-do-projeto
2. Crie e ative um ambiente virtual (Recomendado):

No Windows (PowerShell):

Bash

python -m venv venv
.\venv\Scripts\Activate
No macOS/Linux:

Bash

python3 -m venv venv
source venv/bin/activate
3. Instale as dependências do Python: (O projeto não inclui um requirements.txt, então as dependências principais estão listadas abaixo).

Bash

pip install Flask werkzeug requests flask-cors
Flask: O framework web.

werkzeug: Para hash de senhas.

requests: Para consumir a API do ViaCEP.

flask-cors: Para permitir a comunicação entre o frontend e o backend.

3. Executando a Aplicação
1. Rode o servidor Flask:

Bash

python app.py
O script app.py irá automaticamente chamar o database/db.py, que criará o arquivo de banco de dados delivery.db e o preencherá com dados de exemplo.

2. Acesse a aplicação: Abra seu navegador e acesse: http://127.0.0.1:5000/

(Por padrão, você será redirecionado para a tela de login /login).

🧪 Contas de Teste
O banco de dados é criado automaticamente com as seguintes contas de exemplo:

Restaurante 1:

Email: pizzaria@example.com

Senha: 123456

Restaurante 2:

Email: burger@example.com

Senha: 123456

Cliente:

Email: cliente@example.com

Senha: 123456

📄 Licença
Este projeto está licenciado sob a Licença MIT. Veja o arquivo LICENSE para mais detalhes.

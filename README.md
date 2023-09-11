# Cálculo de frete
Projeto para praticar programação assíncrona e API REST no backend. Simula o cálculo de frete de uma loja de eletrônicos.
## Como instalar
Após baixar o conteúdo desse repositório para sua máquina, use o comando *npm install* para fazer o download de todas as dependências necessárias para esse projeto.
```ruby
npm install
```
Em seguida, use o comando *npm run dev* para inicializar o servidor:
```ruby
npm run dev
```
E então, use o navegador ou um software como Insomnia para rodar as rotas a partir de *http://localhost/3000*
## Como usar
Essa API é composta por 3 endpoints:
### */produtos*
Aqui, são listados todos os produtos da loja, ordenados por *id*, exibindo todos os dados relativos a cada um:

- *Exemplo: http://localhost/produtos*

![Captura de tela 2023-09-11 160216](https://github.com/PauloSJennings/api-calculo-de-frete/assets/139507454/69f22365-0230-49d2-a619-d4593e700b14)

### */produtos/:idProduto*
Nessa rota, a API retorna apenas um produto, a partir de seu *id*, que é mandado por meio de parâmetro de rota.

- *Exemplo: http://localhost/produtos/9*

![Captura de tela 2023-09-11 160529](https://github.com/PauloSJennings/api-calculo-de-frete/assets/139507454/3c6f8611-ddc6-4ae1-9ef8-6f21a325813d)

### */produtos/:idProduto/frete/:cep*
Por último, esse endpoint recebe um id de produto e um cep como parâmetros de rota, e retorna, além dos dados do produto, o valor do frete, em centavos, e o estado ao qual aquele cep pertence.

- *Exemplo: http://localhost/produtos/9/frete/77475970*

![Captura de tela 2023-09-11 161302](https://github.com/PauloSJennings/api-calculo-de-frete/assets/139507454/23483d61-b38f-4f70-92cd-a6bfc11216d9)

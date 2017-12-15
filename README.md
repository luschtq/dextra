# Projeto startup alimentos

<b>Instruções para execução</b>

- O projeto deve ser executado no Sistema Operacional Windows
- Possuir instalada .NET Framework 4.5.2 ou superior
- Visual Studio 2015 ou superior ou outra IDE compatível
- Clicar no arquivo Dextra.sln
- Como não há banco de dados, não será necessário configurar a conexão com o banco de dados.
- Para executar o projeto, aberte a tecla F5.
- Para geração dos pedidos, clique no link Pedido, na parte superior esquerda.
- Na tela de pedidos, é possível salvar mais de um lanche para o mesmo pedido.
- Selecione, ou não, o tipo de lanche e nos itens de ingredientes, selecione a quantidade que deseja para cada item. Se desejar remover algum item do lanche selecionado, basta colocar a quantidade como zero (0) naquele item.
- Após isso, clique em Salvar.
- Caso o pedido for finalizado, clique em Finalizar Pedido.
- Na tela seguinte irá mostrar todas as informações a respeito do pedido, com os descontos em cada lanche, desconto total e preço total do pedido.
- Para gerar um novo pedido, clique em Voltar na aprte inferior esquerda, ou em Pedido, na parte superior esquerda.

<b>OBS.: </b>
- Será criada uma pasta no C:/ chamada Dados, que irá conter os arquivos json do projeto. Caso não tenha a unidade C: ou dê erro na criação em razão de permissões, copiar esses arquivos que estão na pasta app_data do projeto Dextra. Caso dê erro na criação, será exibida uma mensagem na página princiál do site. Se não ocorreu erro, aparecerá a mensagem "Arquivos criados com sucesso". Mas se os arquivos já existirem não aparecerá nenhuma mensagem.

- O nome da pasta C:/Dados está referenciada no web.config, na tag appSettings, na chave "EnderecoArquivos". A mesma configuração está no app.config do projeto Dextra.Tests, que é referentes aos testes.

<b> Execução dos testes </b>
- Index(): verifica se a página default do site foi executada
- PromocaoLight() - verifica se a promoção light está correta
- PromocaoLight_Desconto() - verifica se a desconto da promoção light está correto
- PromocaoMuitaCarne() - verifica se a promoção muita carne está correta
- PromocaoMuitoQueijo() - verifica se a promoção muito queijo está correta
- Pedido_Gerar() - verifica se o valor do pedido está correto
- Em todos os testes, menos no Index(), tem o cálculo da inflação.




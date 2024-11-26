***Plano de Testes Swag Labs***


**Objetivo**

- *Testar a aplicação com em modelo funcional, UI e UX*
- *Identificar possíveis entraves para a usabilidade e acessibilidade que podem impactar a usabilidade que podem impactar a experiencia do usuário*
- *Identificar possíveis bugs que possam impactar o usuário a utilizar as funcionalidades* 
- *Propor melhorias que agreguem valor ao cliente final.*

*Cenários:*

|*1*|*Login*|*Caso de teste 1*|*Testar login com todos os usuários cadastrados*|
| :- | :- | :- | :- |
|*2*|*Filtro*|*Caso de Teste 2*|*Testar se o comportamento do filtro atende ao esperado (retorna os parâmetros de pesquisa?)*|
|*3*|*Fluxo de Compras*|*Caso de Teste 3*||
|*4*|*Excluir item do Carrinho*|*Caso de Teste 4*|*Botão remover (anúncio do produto)*|
|*5*|*Excluir item do Carrinho*|*Caso de teste 4*|*Abrir carrinho e remover item*|
|*6*|*Navegar entre as tabs*|*Caso de teste 3*||
|*7*|*Menu*|*Caso de teste 5*|*Testar opções do botão Menu*|
|*8*|*Redirecionamento Redes Sociais*|*Caso de teste 6*|*Validar se ao clicar nos Ícones das redes sociais a aplicação redireciona para a rede correta.*|
|*9*|*Logout*|*Caso de teste 5*||







**Casos de Teste**

***1 - Login - Acesse a aplicação com os logins e senha cadastrados***

- *Passos*
  - *Acesse a aplicação: ([https://www.saucedemo.com](https://www.saucedemo.com/)).*
  - *Selecione um dos usuários cadastrados e senha*
    - *Necessário testar todos os users e validar se o acesso será permitido*
  - *Valide se o acesso será autorizado*

- *Resultado Esperado*
  - *Usuário deverá ter acesso permitido com exceção do usuário locked\_out\_user que está com status bloqueado.*

***2 - Filtro – Valide o comportamento do Filtro***

- *Passos*
  - *Acesse a aplicação: ([https://www.saucedemo.com](https://www.saucedemo.com/)).*
  - *Insira um dos usuários cadastrados e senha*
  - *Click no botão Login*
  - *Click no componente de filtro* 
  - *Selecione a opção de Ordenação de A a Z*
  - *Valide se a seleção retorna a ordenação selecionada*
  - *Selecione a opção de Ordenação de Z a A*
  - *Valide se a seleção retorna a ordenação selecionada*
  - *Selecione a opção de Ordenação de Preço (baixo- alto)*
  - *Valide se a seleção retorna a ordenação selecionada*
  - *Selecione a opção de Ordenação de Preço (baixo- alto)*
  - *Valide se a seleção retorna a ordenação selecionada*



- *Resultado Esperado*
  - *O filtro deve atender aos parâmetros de pesquisa*

***3 - Fluxo de compra/Navegação entre telas***

- *Passos*
  - *Acesse a aplicação: ([https://www.saucedemo.com](https://www.saucedemo.com/)).*
  - *Insira um dos usuários cadastrados e senha*
  - *Click no botão Login*
  - *Selecione 2 ou mais produtos e Click no botão Add to cart*
  - *Valide se o botão Add to cart é desabilitado e se o botão Remove é habilitado*
  - *Click no ícone de carrinho e valide se todo os produtos adicionados estão lá.*
  - *Valide se o botão Continue Shopping está visível e é clicável*
  - *Click no botão Continue Shopping*
  - *Valide se a tela é redirecionada para tela principal*
  - *Click no ícone de carrinho*
  - *Valide se o botão Checkout está visível e é clicável*
  - *Click no botão Checkout*
  - *Valide se a tela é redirecionada para Checkout Your Information*
  - *Verifique se os campos são exibidos, permite inserir dados e tem tratamento para Mandatory field*
    - *First Name*
    - *Last Name*
    - *Zip/Postal Code*
  - *Valide se os botões Cancel Continue são exibidos e clicáveis*
  - *Click no botão Cancel e Valide se a tela é redirecionada para o carrinho*
  - *Click no botão Continue e Valide se redireciona para tela Checkout: Overview*
  - *Verifique se as informações para pagamento são exibidas e se o valor corresponde a soma dos produtos do carrinho mais a taxa.*
  - *Valide so botão Cancel e Finish são exibidos e clicáveis suas ações.*
    - *Click no botão Cancel e valide se a tela é redirecionada para o carrinho*
    - *Click no botão Finish e valide se a compra é finalizada, exibe a tela Checkout: Complete*
  - *Verifique se o carrinho está vazio após finalizar a compra*


- *Resultado Esperado*
  - *Fluxo deverá ser concluído com sucesso*





***4 – Remoção de itens*** 

- *Passos*
  - *Acesse a aplicação: ([https://www.saucedemo.com](https://www.saucedemo.com/)).*
  - *Insira um dos usuários cadastrados e senha*
  - *Click no botão Login*
  - *Selecione 2 ou mais produtos e Click no botão Add to cart*
  - *Valide se o botão Add to cart é desabilitado e se o botão Remove é habilitado*
  - *Click no ícone de carrinho e valide se todo os produtos adicionados estão lá.*
  - *Click no botão remove (dentro do carrinho e verifique se o item é excluído*
  - *Volte a tela principal*
  - *Pesquise pelo item adicionado ao carrinho e click no botão remove*
  - *Verifique se o numero de itens adicionados diminui(no ícone carrinho*
  - *Click no ícone carrinho e verifique se o item excluído realmente foi removido.*

- *Resultado Esperado*
  - *O usuário deverá poder remover os itens adicionados tanto clicando no botão remove no item na tela principal, quanto clicando no botão remove de dentro do carrinho.*

***5– Menu*** 

- *Passos*
  - *Acesse a aplicação: ([https://www.saucedemo.com](https://www.saucedemo.com/)).*
  - *Insira um dos usuários cadastrados e senha*
  - *Click no botão Login*
  - *Na tela principal click no botão Menu*
  - *Valide se as opções são exibidas*
    - *All Items*
    - *About*
    - *Logout*
    - *Reset App State*
  - *Click em All Items option e valide o comportamento da tela*
  - *Click em About Option e valide o comportamento da tela*
  - *Click em Reset App State e valide o comportamento da tela*
  - *Click em Logout option e valide se usuário será deslogado*

- *Resultado Esperado*
1. *All Items option – Deverá exibir todos os itens da loja*
1. *About Option -Deverá exibir dados sobre a loja*
1. *Reset App State - Deverá restaurar as configurações iniciais  do app(limpar seleções)*
1. *Logout – Deverá deslogar o usuário*

***6 – Redirecionamento Redes Sociais***

- *Passos*
  - *Acesse a aplicação: ([https://www.saucedemo.com](https://www.saucedemo.com/)).*
  - *Insira um dos usuários cadastrados e senha*
  - *Click no botão Login*
  - *Role a tela até o final e verifique se é exibido os ícones das redes sociais*
    - *Twitter*
    - *Facebook*
    - *Instagram*
  - *Click no ícone do Twitter e valide se a tela é redirecionada para rede social*
  - *Click no ícone do Facebook e valide se a tela é redirecionada para rede social*
  - *Click no ícone do Instagram e valide se a tela é redirecionada para rede social*

- *Resultado Esperado*

  *Sistema deverá redirecionar para a tela principal da rede social do ícone clicado.*

**Resultado dos Testes**

|*Data*|*Descrição do Teste*|*Pass/Fall*|*Tester*|*Comentarios*|
| :- | :- | :- | :- | :- |
|*24/11*|*CT 01*|*Pass*|*Edinéa* ||
|*24/11*|*CT 02*|*Pass*|*Edinéa*||
|*24/11*|*CT 03*|*Pass*|*Edinéa*||
|*24/11*|*CT 04*|*Pass*|*Edinéa*||
|*24/11*|*CT 05*|*Pass*|*Edinéa*||
|*24/11*|*CT 06*|*Pass*|*Edinéa*||
||||||




***BUGS***

Foi identificado bugs vinculados aos usuários cadastrados

BUG1 -  User: problem\_user

- Mesma imagem para todos os itens
- Filtro não está ordenando conforme a seleção das opções (Ao clicar nenhuma ação ocorre)

BUG2 -  User: performance\_glitch\_user

- Tempo de resposta superior a 5 seg – Ao filtrar a ação tem um delay


BUG3 -  User: error\_user

- Sistema não permite selecionar opções de filtro e exibe msg (Image1)
- Ao adicionar item. Não permite remover clicando no botão que existe no item na tela principal.

<Image1>

![Interface gráfica do usuário, Texto, Aplicativo

Descrição gerada automaticamente](Aspose.Words.5bfb2aa3-eea4-4501-8451-7791f95edbb1.001.png)

BUG4 -  User: visual\_user

1. 1 Icone menu torto
1. Não importa qual seleção do filtro a imagem não altera
1. Icone carrinho torto – sem alinhamento
1. Botão add cart sem alinhamento
1. Não exibe botão cancel e botão checkout fora do padrão IMAGEM2

![Site, Linha do tempo

Descrição gerada automaticamente](Aspose.Words.5bfb2aa3-eea4-4501-8451-7791f95edbb1.002.png)

<IMAGEM2>

![Interface gráfica do usuário, Texto, Aplicativo, Email

Descrição gerada automaticamente](Aspose.Words.5bfb2aa3-eea4-4501-8451-7791f95edbb1.003.png)

BUG45-  Any user

Na tela Checkout no clicar no botão Continue sem o preenchimento dos dados, aparece a mensagem informando que os campos são obrigatórios, ao tentar preencher o campo Last Name não permite preenchimento. Ao preencher, sistema deleta o First Name

![Interface gráfica do usuário, Aplicativo, Teams

Descrição gerada automaticamente](Aspose.Words.5bfb2aa3-eea4-4501-8451-7791f95edbb1.004.png)

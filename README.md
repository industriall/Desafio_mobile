## Visão Geral - Contexto do desafio

Você é responsável por revolucionar nosso aplicativo de Rotas de Inspeção, uma aplicação destinada a registrar as inspeções de rotina em uma série de equipamentos. Atualmente ele funciona da seguinte forma: O usuário possui uma lista de equipamentos que compõem a rota de inspeção na qual ele é o responsável. Ao selecionar um equipamento, abre uma lista de perguntas sobre o estado de funcionamento desse equipamento, em função dos parâmetros (temperatura, pressão, nível de óleo, etc). O usuário deve assinalar a resposta que corresponde ao estado de funcionamento daquele parâmetro, como “normal” ou “anormal”, por exemplo. Quando todas as perguntas de todos os equipamentos da rota forem respondidas, o usuário pode concluir a rota. 

Os usuários estavam se queixando de demorar para achar o equipamento na lista, pois algumas rotas possuem muitos equipamentos. O time iPRIMUM pensou em facilitar essa procura desenvolvendo um sistema de leitura de QR Code do identificador dos equipamentos. Ou seja, uma vez o operador estando de frente do equipamento pertencente a rota, basta escanear o QR Code e a lista de perguntas sobre o estado de funcionamento do equipamento é exibida na tela do aplicativo. 

É de sua responsabilidade, como desenvolvedor mobile, construir um aplicativo similar ao Rotas de Inspeção, que possua a funcionalidade de leitura do QR Code do identificador do equipamento descrita anteriormente.

Todas as configurações relacionadas ao back-end (api e endpoints) e banco de dados (base de perguntas, Tag do equipamento, etc), serão disponibilizadas por nós. Sua função é apenas desenvolver a interface mobile responsável por selecionar o equipamento, registrar as respostas do operador e enviar de volta a API. 


**Instruções:**
1.	O que se espera do APK:
- Desenvolver uma tela de login;
- Desenvolver uma tela de Home que possua uma função de buscar rotas para capturar todos os equipamentos que se espera realizar a rota e formar uma lista;
- A seleção do equipamento da lista a se realizar a rota poderá ser feito de duas formas:
  - Selecionando um equipamento diretamente na lista;
  - Lendo o QR code de algum equipamento da lista. Nesse caso, o formulário de perguntas deve ser exibido assim que o QR code for lido;
- Desenvolver uma tela com as perguntas cadastradas para o equipamento selecionado (via seleção ou via leitura do QR code). A tela deve possuir as seguintes informações: 
    - Nome do equipamento;
    - Tag;
  - Pergunta seguida das opções de resposta. Estas devem ser um campo de “check” de única escolha, e, caso a resposta seja sinalizada com observação obrigatória, deve exibir um campo de texto obrigatório (se o usuário selecionar essa resposta);
- Desenvolver uma função de concluir rota de inspeção na tela de Home que limpe os equipamentos da rota, se todos os equipamentos forem respondidos;

2.	Bônus:
- Desenvolver uma função de anexar arquivos para cada pergunta;

### Regras de negócio
- É obrigatório responder todas as perguntas;
- As respostas sinalizadas com observação obrigatória devem exibir um campo de texto obrigatório para justificativa uma vez que o usuário selecionar aquela resposta;
- Na home é obrigatório exibir a lista de todos os equipamentos da rota, marcados com seu respectivo status (respondido ou pendente). A forma de exibição do status é de sua escolha;
- Assim que o usuário finalizar as respostas e clicar em salvar, ele deve ser redirecionado para a home e o equipamento deve ser marcado como respondido;
- O usuário só pode salvar as respostas se todos os itens estiverem respondidos;
- A funcionalidade de anexar arquivos deve permitir o upload apenas de imagens e vídeos;

### API
Toda a documentação necessaria para comunicação com a api está disponivel no endereço:
https://desafio-iall.azurewebsites.net/api/swagger/index.html

## Como serei avaliado?
O candidato será avaliado levando em conta os seguintes critérios:
- Atendimento das regras de negócios;
- Fidelidade ao funcionamento descrito nas instruções;

### Diferencial
- Usabilidade (UX);
- Desenvolver em Ionic e Angular;

### Você poderá:
- efetuar um pull request da sua implementação diretamente no Github até a data limite de 19/04/2022, ou
- encaminhar para o e-mail henan.ferreira@industriall.ai com rh@industriall.ai em cópia, um arquivo .zip ou link com o código fonte até a data limite de 19/04/2022.

Qualquer problema ou dificuldade, você pode entrar em contato conosco pelos e-mails, henan.ferreira@industriall.ai ou rh@industriall.ai para que possamos sanar todas as dúvidas!

# GA4-AutoDimensions
Criei este projeto para facilitar/automatizar a criação de dimensões personalizadas no GA4 pelo front-end sem a necessidade de acessar a API.

## STEP BY STEP

1. Acesse a sua propriedade do GA4
2. Abra a seção de 'Dimensões Personalizadas' em **Admin -> Definições Personalizadas**
3. Abra o Console do Developer Tools no seu navegador (**atalho: CTRL+SHIFT+J**)
4. Copie o código abaixo, Cole no Console e pressione Enter.
5. Se abrir uma janela de Debug igual imagem abaixo, feche o Console (**atalho: CTRL+SHIFT+J**)

![https://i.imgur.com/8q9QKxY.gif](https://i.imgur.com/8q9QKxY.gif)

```js
/*!
 * Felipe-Dimensions-GA4 v1.0.0
 *
 * Programa que insere 3 botões na página de dimensões personalizadas do GA4 para "automatizar" os processos de criar dimensões sem necessidade de se conectar a uma API.
 * 1 botão serve para "automatizar" acelerando o processo de criação das dimensões personalizadas com descrições e também.
 * 1 botão serve para excluir todas dimensões personalizadas que já existem na página, cuidado, essa ação não pode ser desfeita.
 * 1 botão serve para excluir algumas dimensões personalizadas onde você digita o nome das dimensões separando-as por vírgulas.
 *
 *
 * Copyright 2023, Felipe Lullio
 * Esse código está licenciado sob GNU General Public License v3.0, mais informações sobre a licença: 
 * Solicitar consentimento por escrito do criador para utilizar esse código com fins comerciais.
 * 
*/

// Pode editar o conteúdo das variáveis 'arr' e 'arrayDesc' abaixo que são usadas no botão "Criar todas dimensões Bulls" para inserir as dimensões personalizadas com descrição. Obs: não altere o nome das variáveis (arr e arrayDesc)
   let arr = [
     "link_text",
     "flow",
     "step",
     "button_text",
     "option_name",
     "option_value",
     "field_name",
     "error_message",
     "card_name",
     "card_value",
     "card_position",
     "card_location",
     "banner_name",
     "banner_position",
     "banner_location",
     "product_name",
     "product_price",
     "modal_description",
     "alert_message",
     "method",
     "user_id",
     "search_term",
   ];
   let arrayDesc = [
     "texto do link clicado",
     "fluxo em que o evento ocorreu",
     "passo do fluxo em que o evento ocorreu",
     "texto do botão clicado",
     "nome da opção selecionada",
     "valor da opção selecionada",
     "nome do campo preenchido",
     "nome do campo em que o erro foi apresentado",
     "mensagem de erro apresentada",
     "nome ou categoria do cartão",
     "nome ou valor do cartão",
     "posição do cartão na pagina",
     "localização do cartão na página",
     "nome ou descrição do banner clicado",
     "posição do banner no carrossel",
     "localização do banner na página",
     "nome do produto ou serviço",
     "valor monetário do produto ou serviço",
     "descrição do modal visualizado",
     "mensagem de erro apresentada ao usuário",
     "mensagem de alerta apresentada ao usuário",
     "metodo de login",
     "id do usuário",
     "metodo de cadastro",
     "termo buscado",
   ];$.getScript('https://cdn.jsdelivr.net/gh/lullio/GA4-AutoDimensions/script.js');
```

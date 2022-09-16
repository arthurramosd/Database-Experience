# **Projeto de Modelagem de E-Commerce**

Se trata de um desafio de projeto do Bootcamp Database Experience oferecido pela Digital Innovation One e ministrado em sua grande maioria pela instrutura Juliana Mascarenhas, neste repositório eu incluí os arquivos deste projeto, que são o script da modelagem e a imagem que demonstra a modelagem dos dados.




**Atividades**  

**Cliente PF e PJ** - Uma conta pode ser Pessoa Física e Jurídica, mas não pod ter as duas informações.  
**Resposta:** Crei um atributo ENUM na tabela de cliente com as opções de PF e PJ, dessa forma, não foi necessário criar nenhuma outra tabela para armazenar essas informações.   
  


**Pagamento** - Pode ter cadastrado mais de uma forma de pagamento.  
**Resposta:** Criei uma tabela mãe chamada "Pagamento" e duas tabelas filhas chamadas "CartaodeCredito" e "Boleto", respectivamente. Onde a tabela mãe se relaciona com as informações necessárias do pagamento selecionado pelo cliente. 


**Entrega** - Possui status e código de rastreamento.  
**Resposta:** Criei uma tabela chamada "Entrega" com os seguintes atributos "Tracking", que é a Primary Key desta entidade e também o código de rastreamento, "Transportadora" que se refere a empresa na qual os produtos serão enviados e "Status" que é um atributo ENUM, com os valores Aguardando Envio, Enviado e Entegue.

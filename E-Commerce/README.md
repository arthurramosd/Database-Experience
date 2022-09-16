Projeto de Modelagem de E-Commerce

• Cliente PF e PJ - Uma conta pode ser Pessoa Física e Jurídica, mas não pod ter as duas informações 
R: Crei um atributo ENUM na tabela de cliente com as opções de PF e PJ, dessa forma, não foi necessário criar nenhuma outra tabela para armazenar essas informações.  

• Pagamento - Pode ter cadastrado mais de uma forma de pagamento 
R: Criei uma tabela mãe chamada "Pagamento" e duas tabelas filhas chamadas "CartaodeCredito" e "Boleto", respectivamente. Onde a tabela mãe se relaciona com as informações necessárias do pagamento selecionado pelo cliente. 

• Entrega - Possui status e código de rastreamento. 
R: Criei uma tabela chamada "Entrega" com os seguintes atributos "Tracking", que é a Primary Key desta entidade e também o código de rastreamento, "Transportadora" que se refere a empresa na qual os produtos serão enviados e "Status" que é um atributo ENUM, com os valores Aguardando Envio, Enviado e Entegue.

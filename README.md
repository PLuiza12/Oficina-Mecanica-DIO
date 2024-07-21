# Desafio Construindo um Esquema Conceitual para Banco de Dados 

## Objetivo:
Criar o esquema conceitual para o contexto de oficina com base na narrativa fornecida 

### Narrativa:
- Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina:
  
Foi criada uma entidade chama *Serviço* na qual consta atributos como data de inicio e data de termino
e o tipo de serviço que será executado pela Ordem de serviço.

- Clientes levam veículos á oficina mecânica para sere consertados ou para passarem por revisões
  periódicas:
  
  Foi criado duas entidades para a entidade *ordem de serviço* : *O.S preventiva* ou *O.S corretiva*. Isso dependerá do caso do qual
  o véiculo apresenta no momento.

- Cada véiculo é designado a uma equipe de mecânicOS que identifica os serviços a serem executados e
   preenche uma OS com data de entrega:
  
   Foi criada uma entidade chamada *Equipe de mecânicos*, qual possui os atributos com o nome,endereço e
   a especialidade.

- A partir da os, calcula-se o valor de cada servoço, consultando-se uma tabela de referência de
     mão-de-obra:
  
     A entidade ordem de serviço possui o atribuito para o valor de serviço fornecido.

- O valor de cada peça também irá compor a OS do cliente autorizar a execução dos serviços:
- 
  Foi criada uma entidade chamada *peças* com os atribuitos de nome, status da peça e o valor da peça.

- A mesma equipe avalia e executa o serviços:
  
  A entidade Equipe mecânicos está se relacionando com a entidade *Tipo de Ordem de serviço* na qual
  irá identificar para qual O.S a Equipe de mecânica será designada para executar o serviço.

- Cada OS possui: N°, data de emissão, um valor, status e uma data para a conclusão dos trabalhos:

  Foi criada a entidade *Ordem de Serviço O.S*, qual foi criado os atributos de data de inicio, data e termino
  status de serviço e o valor do serviço.

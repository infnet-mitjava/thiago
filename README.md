# Avaliação de disciplina Mensageria (Prof Veloso)

Para construir o banco, configure o ***persistence.xml*** do projeto ***lojavirtual-ejb*** da seguinte forma:

```xml
<properties>
   <!-- Properties for Hibernate -->
   <property name="hibernate.hbm2ddl.auto" value="update" />
   <property name="hibernate.show_sql" value="true" />
</properties>
```
O endpoint REST encontra-se em
> http://[server-ip]:8085/loja/api

A API encontra-se documentada em
> http://[server]:8085/loja-api/swagger-ui.html

O Web Server encontra-se em
> http://[server-ip]:8080/lojavirtual

O sistema efetua um cadastro de compras seguindo os requisitos solicitados:

### User Stories

> 1. Como usuario quero efetuar cadastro de Clientes
> 2. Como usuario quero efetua cadastro de Produtos
> 3. Como usuario quero efetuar uma compra relacionando um Cliente a um ou mais Produtos
> 4. Como usuario quero visualizar os pedidos que foram efetuados

### Requisitos nao-funcionais

> 1. O cadastro e recuperacao de dados de Clientes devem ser feitos por uma API Rest elaborada com a tecnologia Spring Boot
> 2. O cadastro e recuperacao de dados de Produtos devem ser feitos por uma API Rest elaborada com a tecnologia Spring Boot
> 3. As paginas web devem ser feitas utiilzando Web Servlets
> 4. O processamento e criacao de pedidos deve ser feito com a tecnologia Enterprise Java Beans
> 5. O pagamento deve ser feito utilizando Java Message Service
> 6. Um Message Driven Bean deve atualizar a base após o processamento bem-sucedido do pagamento
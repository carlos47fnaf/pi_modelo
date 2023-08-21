# Projeto Integrador - TechnoGeek

Um modelo para o desenvolvimento do Projeto Integrador do Curso de Técnico em Desenvolvimento de Sistemas para a Internet Integrado ao Ensino Médio do IFC - Campus Araquari.

Professores: [Marco André Mendes](github.com/marcoandre) e [Alann Perini](https://github.com/AlannKPerini).

**Equipe:**
Carlos Eduardo Mello (git: carlos47fnaf)

Bruno Corrêa Dias (git: BCD15)

Dominic Krelling (git: Dominic-Krelling)

Links do projeto:

-   [Documentação (esse documento)](github.com/marcoandre/pi-modelo)
-   [Backend](github.com/marcoandre/pi-backend)
-   [Frontend](github.com/marcoandre/pi-frontend)

# Situação Problema

A loja de moda geek é especializada em camisetas e outros produtos do universo nerd. Existe há dois anos e é de propriedade de um grupo de amigos entusiastas da cultura pop. A equipe é composta por três funcionários: o gerente, um designer gráfico e um vendedor, todos dedicados a oferecer um atendimento personalizado e de qualidade aos clientes.

Atualmente, a loja funciona apenas como uma loja física, com vendas presenciais limitadas à região onde está localizada. Embora tenha uma clientela fiel, a empresa não está atingindo todo o seu potencial, pois não está disponível para venda em outras localidades. Além disso, o processo de gerenciamento da loja é manual, o que torna difícil acompanhar o estoque e as vendas e pode levar a erros de gestão.

O sistema de vendas funciona da seguinte forma: o cliente escolhe o produto e o leva até o caixa, onde o funcionário registra o código de barras no sistema. Após o pagamento, é dada a baixa do produto no sistema e a venda é registrada. Vale destacar que nossos produtos são produzidos de maneira artesanal, então não temos fornecedores.

# Proposta

Entretanto, para expandir os negócios e melhorar a eficiência da loja, é importante considerar a possibilidade de criação de uma loja virtual, o que permitiria atingir uma clientela maior e facilitar o gerenciamento de estoque e vendas. Com essa plataforma online, seria possível integrar os processos de venda, gerenciamento de estoque e controle de finanças, aumentando a produtividade e reduzindo o tempo gasto com tarefas manuais. Dessa forma, a loja poderia maximizar seus resultados e alcançar um novo patamar de sucesso.

Para resolver esses problemas, propomos a criação de uma loja virtual, a fim de expandir a área de vendas e facilitar o acesso aos clientes atuais. A loja virtual também ajudará no gerenciamento da loja, com um software focado em gerenciamento de estoque e vendas, permitindo que os funcionários gerenciem o inventário e rastreiem as vendas de forma mais eficiente. O software será acessível tanto para o gerente quanto para os vendedores, com diferentes níveis de acesso e permissões.

Além disso, os clientes poderão acessar a loja virtual para visualizar os produtos disponíveis e fazer pedidos online, com a opção de entrega ou retirada na loja física. A loja virtual terá um layout responsivo, fácil de usar e intuitivo, além de estar integrada com sistemas de pagamento seguros para facilitar as transações.

Com a loja virtual, a loja poderá expandir sua clientela e aumentar suas vendas, simplificando o processo de gerenciamento de estoque e vendas.

# Regras de Negócio

- **RN001 - Catálogo de Produtos:** Todos os produtos disponíveis na loja física devem ser devidamente catalogados e listados no site da loja virtual.

- **RN002 - Processo de compra:** Os clientes têm a liberdade de explorar o site, adicionar produtos ao carrinho de compras e revisar informações como descrição do produto, preço e disponibilidade de estoque. 

- **RN003 - Informações do Cliente:** No momento de finalizar a compra, os clientes são solicitados a fornecer seus dados pessoais e endereço para a entrega ou opção de retirada na loja física.

- **RN004 - Pagamento:** A loja virtual deve integrar com sistemas de pagamento para que os clientes possam efetuar o pagamento das compras online.

- **RN005 - Entrega:** A loja virtual deve oferecer opções de entrega, incluindo envio pelos correios ou retirada na loja física. O prazo de entrega deve ser informado ao cliente no momento da compra.
 
- **RN006 - Gerenciamento de estoque:** A loja virtual deve ser integrada com um sistema de gerenciamento de estoque, permitindo que os funcionários da loja monitorem o estoque de produtos e atualizem as informações disponíveis no site. 

- **RN007 - Gestão financeira:** A loja virtual deve ter um sistema integrado para gerenciamento financeiro, permitindo que os funcionários monitorem as vendas, receitas e despesas.

- **RN008** - O site deve permitir que o cliente o acesso sem a necessidade de um cadastro.

# Requisitos Funcionais

**ENTRADA**

- **RF001 - Cadastro Funcionário** - O cadastro dos funcionários no site deve ser feito pelo gerente dentro do site, cadastrando o nome e a senha.
    - **Dados necessários:** nome, senha.
    - **Usuários:** gerente.

- **RF002 - Cadastro Cliente** - Para realizar o cadastro o cliente deve fornecer dados completos.
    - **Dados necessários:** nome completo, data de nascimento, e-mail, senha, número de telefone, CPF, estado, cidade, bairro, rua, número da residência, CEP.
    - **Usuários:** clientes.

- **RF003 - Cadastro de Produto** - O cadastro deve incluir informações essenciais, como nome do produto, descrição, preço, disponibilidade em estoque e imagens ilustrativas. Além disso, o sistema deve validar a integridade dos dados inseridos e disponibilizar uma interface para que os vendedores possam adicionar, editar ou remover produtos.
    - **Dados necessários:** nome do produto, descrição, preço, quantidade, imagens ilustrativas.
    - **Usuários:** vendedores/gerente

**PROCESSAMENTO**

- **RF004 - Autenticação de usuário:** tem como propósito autenticar o acesso ao sistema, verificando se o usuário pode acessá-lo e, caso possa, o direcionando para a página principal de seu perfil de acesso.
    - **Dados necessários:** login, senha.
    - **Usuários:** todos os níveis de usuário.  
  
- **RF005 - Adição de produtos ao carrinho:**  permitir que os clientes adicionem produtos ao carrinho de compras, escolhendo a quantidade desejada.
    - **Dados necessários:** produto selecionado, quantidade.
    - **Usuários:** todos os níveis de usuário.

- **RF006 - Remoção de produtos do carrinho:**  permitir que os clientes removam produtos do carrinho de compras antes de finalizar a compra.
    - **Dados necessários:** produto a ser removido, quantidade
    - **Usuários:** todos os níveis de usuário.

- **RF007  - Finalização da compra:** permitir que os clientes  cadastrados finalizem a compra dos produtos adicionados ao carrinho, selecionando a forma de pagamento e fornecendo informações de entrega ou retirada na loja física.
    - **Dados necessários:** forma de pagamento, informações de entrega.
    - **Usuários:** clientes.

**SAÍDA**

- **RF008 - Busca de produtos:**  permitir que os clientes busquem produtos específicos na loja virtual, utilizando palavras-chave.
    - **Dados necessários:** produtos
    - **Usuários:** todos os níveis de usuário.

- **RF009 - Gerenciamento de estoque:** permitir que o gerente e os vendedores atualizem o estoque dos produtos vendidos na loja física e na loja virtual.
    - **Dados necessários:** produtos, atualizações de estoque.
    - **Usuários:** gerente, vendedores.

- **RF010 - Relatórios de vendas:** O sistema deve gerar relatórios de vendas para análise da gestão.
     - - **Dados necessários:** vendas, data inicial e data final
    - **Usuários:** gerente
    - 

# Requisitos Não Funcionais

- **RNF001 - Usabilidade e Navegação Intuitiva** -O site deve ser fácil de usar e navegar para que os usuários possam encontrar rapidamente o que estão procurando,inclui um design intuitivo, uma navegação clara e concisa e uma interface amigável.

- **RNF002 - Tempo de Carregamento Rápido**- O site deve carregar rapidamente para que os usuários não percam a paciência e desistam de fazer compras. 

- **RNF003 - Segurança de Informações Pessoais e Financeiras** - O sistema deve garantir que as informações pessoais e financeiras estão seguras ao fazer compras no site. 

- **RNF004 - Disponibilidade Contínua do Site** - O site deve estar disponível e funcionando corretamente em todos os momentos. 

- **RNF005 - Hospedagem em Servidor Confiável e Planos de Contingência** - Garantir que o site seja hospedado em um servidor confiável e que haja backups e planos de contingência em caso de falha.

- **RNF006 - Escalabilidade para Lidar com Volume de Usuários** - O site deve ser capaz de lidar com um grande volume de usuários simultaneamente. 

- **RNF007 - Capacidade e Arquitetura para Lidar com Picos de Tráfego** - Planejamento cuidadoso da capacidade do servidor e da arquitetura do site para garantir que ele possa lidar com picos de tráfego.

- **RNF008 - Compatibilidade em navegadores** - O site deve funcionar nos navegadores Chrome, Opera e OperaGX.

- **RNF009 - Sistema Backend** - O sistema de funcionamento interno será construído na linguagem Python usando Django Rest Framework.

- **RNF010 - Sistema Frontend** - Desenvolver a interface do vendedor com Vue.js para proporcionar uma experiência interativa, responsiva e de alta performance, garantindo a satisfação dos usuários.

- **RNF011 - Aplicativo Móvel** - Criar o aplicativo móvel com React Native, visando oferecer uma experiência nativa, com navegação fluída, carregamento rápido e interações responsivas.

- **RNF013 - Banco de Dados** - Utilizar um banco de dados DB SQLite para armazenamento de dados, assegurando estrutura otimizada, integridade, consistência, segurança e escalabilidade.

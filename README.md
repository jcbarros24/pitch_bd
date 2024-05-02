# pitch_bd

Pitch para a disciplina de Banco de Dados 1 

Professor: Lucas Rodolfo Celestino De Farias

Aunos: José Carlos Barros, Antonio Vital, Antônio Castelão

### Roteiro do pitch

#### 1. Missão e Visão
**Missão**: A EducaLivros tem como missão liderar o mercado de distribuição de conhecimento, conectando pessoas ao mundo literário e educacional através de tecnologia inovadora. A empresa busca tornar o aprendizado acessível e prazeroso para todos.  
**Visão**: A visão da EducaLivros é expandir sua oferta de produtos e serviços educacionais, desenvolvendo parcerias com escolas e universidades para facilitar o acesso a recursos educativos. A empresa também planeja incorporar tecnologias emergentes para a recomendação personalizada de livros e materiais de estudo.

#### 2. Funcionalidades do Sistema de Banco de Dados
**Venda de Livros e Papelaria**: A plataforma oferece uma vasta seleção de livros e produtos de papelaria. Utiliza um sistema de carrinho de compras integrado para proporcionar uma experiência de compra suave e mantém um relacionamento dinâmico com fornecedores para garantir um estoque sempre atualizado e diversificado.

**Sistema de Empréstimo de Livros**: Permite que clientes cadastrados tomem livros emprestados com facilidade. O sistema gerencia automaticamente o ciclo de empréstimo, incluindo o registro de datas e o controle de disponibilidade dos livros, além de integrar-se ao cadastro de clientes para fornecer um histórico detalhado e personalizado.

**Gestão de Pedidos e Pagamentos**: Oferece um processo de checkout integrado com opções flexíveis de pagamento. Há um acompanhamento detalhado do pedido desde a compra até a entrega, incluindo a gestão de endereços para facilitar múltiplas entregas e devoluções.

**Relacionamento com Autores**: Proporciona um sistema de feedback onde os autores podem receber comentários diretamente dos leitores, facilitando a interação e o crescimento profissional. A plataforma também oferece recursos para desenvolvimento profissional, incluindo acesso a cursos, webinars, e mentorias com profissionais renomados. Organiza eventos virtuais e presenciais para promover a interação entre autores e leitores, e suporta a organização e divulgação de lançamentos de novos livros. Adicionalmente, há programas específicos de marketing para promover novos autores e lançamentos de livros, além de oportunidades de destaque em newsletters e redes sociais.

### Explicação Técnica Utilizando o Modelo de Banco de Dados
O modelo de banco de dados da EducaLivros reflete as funcionalidades descritas acima e é organizado em várias tabelas principais:

- **Cliente**: Armazena informações dos clientes, como ID, nome, sobrenome, telefone, e-mail, CPF.
- **Livro**: Contém detalhes dos livros, incluindo ID do livro, ID do autor (chave estrangeira), nome do livro, descrição, data de publicação, e informações de estoque.
- **Autor**: Registra informações sobre os autores, incluindo ID, nome e sobrenome.
- **Pedido**: Gerencia os pedidos feitos pelos clientes, incluindo ID do pedido, data, valor total, e a chave estrangeira do cliente e do carrinho de compras.
- **Pagamento**: Lida com as transações de pagamento, armazenando ID do pagamento, forma de pagamento, data, montante, e a chave estrangeira do pedido correspondente.

Esse modelo suporta a complexidade das operações da EducaLivros e permite uma interação eficiente entre diferentes partes do sistema, garantindo que todas as funcionalidades sejam executadas de maneira integrada e eficaz.

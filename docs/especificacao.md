3. DOCUMENTO DE ESPECIFICAÇÃO DE REQUISITOS DE SOFTWARE 

 

3.1 Objetivos deste documento 

Este documento tem como objetivo descrever e especificar as necessidades que devem ser atendidas pelo sistema de administração hoteleira, a experiência dos hóspedes e o trabalho da recepção. O sistema deve permitir um controle eficaz das reservas e da disponibilidade dos quartos, facilitando a organização da ocupação para os administradores. Além disso, deve oferecer uma interface intuitiva para a busca e atualização de informações, reduzindo erros e agilizando o atendimento da recepcionista. Para os hóspedes, é essencial que o processo de reserva seja simplificado, proporcionando uma experiência prática e acessível desde o primeiro contato com o hotel. 

 

3.2 Escopo do produto 

 

3.2.1 Nome do produto e seus componentes principais 

A aplicação web desenvolvida será denominada Hospedagem Simples, e seus componentes principais são: 

Módulo de cadastro de clientes e usuários: permite o gerenciamento de registro, atualização e consulta de informações dos hóspedes. Inclui controle de acesso e perfis (administrador, recepcionista e cliente); 

Módulo de administração: permite o cadastro – incluindo informações como tipo de quarto, características do quarto, valores e status do quarto (disponível, ocupado ou em manutenção) - e manutenção dos quartos. Além disso, permitirá o controle de disponibilidade para novas reservas e configurações gerais do sistema, como políticas de cancelamento e gerenciamento de usuários; 

Módulo de reserva: é o módulo central que comanda a interação dos usuários com o hotel. Assim, permite a interação dos clientes com os quartos cadastrados, podendo criar, alterar e cancelar reservas. Ainda, exibe os sistemas de filtragem e foto dos quartos. 

Módulo de pagamento: permite a confirmação das informações - como data, quarto e número de hóspedes - das reservas selecionadas, permite também a seleção da forma de pagamento e o redirecionamento para um sistema (VIA API) de gerenciamento de pagamento externo (Ex: Mercado Pago). 

 

3.2.2 Missão do produto 

O projeto tem como missão otimizar os processos oferecendo uma experiência mais prática e eficiente para os hóspedes, possibilitando ao usuário visualizar de forma rápida e direta as opções de quartos, preços e disponibilidade, finalizar e reservar sem dificuldade ou incertezas. 

 

3.2.3 Limites do produto 

        O Hospedagem Simples não inclui recursos de avaliação ou feedback dos hóspedes. Além disso, o sistema não garante a disponibilidade contínua de todas as amenidades oferecidas pelo hotel durante todo o período da reserva, estando sujeito a eventuais mudanças ou limitações nas instalações e serviços. 

3.2.4 Benefícios do produto 

 

# 

Benefício 

Valor para o Cliente 

1 

Facilidade na reserva de quartos 

Essencial 

2 

Facilidade na recuperação de informações de reservas 

Essencial 

3 

Facilidade de realizar o pagamento 

Essencial 

4 

Compatibilidade com diferentes dispositivos 

Recomendável 

5 

Facilidade de gerenciamento das reservas pelos administradores 

Essencial 

6 

Filtrar preferências no site 

Recomendável 

 

 

3.3 Descrição geral do produto 

 

3.3.1 Requisitos Funcionais 

 

Código 

Funcionalidade 

Descrição 

RF1 

Pesquisa de disponibilidade de quarto 

 

O sistema deve exibir aos usuários uma lista atualizada de quartos disponíveis, juntamente com os filtros aplicáveis, como faixa de preço, número de hóspedes e período da estadia. 

RF2 

Seleção de quartos 

 

O sistema deve exibir aos usuários os detalhes completos de cada quarto, incluindo descrição, fotos, comodidades, preço, política de cancelamento, além das condições de pagamento. 

RF3 

Cadastro de usuários 

O sistema deve permitir que os usuários criem uma conta por meio do preenchimento de um formulário com suas informações pessoais, como nome completo, e-mail válido, número de telefone, data de nascimento e uma senha segura, obedecendo aos critérios de validação definidos para cada campo. 

RF4 

Simulação e pré-reserva 

 

O sistema deve exibir uma simulação detalhada do valor total da reserva, considerando o tipo de quarto, número de diárias, taxas adicionais e descontos aplicáveis; deve também apresentar os dados do hóspede previamente informados e permitir a seleção da forma de pagamento. 

RF5 

Pagar  

Reserva 

O sistema deve encaminhar as informações da reserva e do pagamento para uma API externa de processamento financeiro. 

RF6 

Autenticação e login 

O sistema deve permitir que os usuários façam login utilizando suas credenciais cadastradas, como e-mail e senha, validando os dados informados e concedendo acesso às funcionalidades da conta apenas após a autenticação bem-sucedida. 

RF7 

Gerenciar conta 

 

O sistema deve permitir que o usuário gerencie seus dados cadastrados, como nome, e-mail, telefone e senha, além de visualizar, editar ou cancelar suas reservas ativas, garantindo que todas as alterações sejam salvas de forma segura e atualizadas em tempo real. 

RF8 

Sair da conta 

O sistema deve permitir que o usuário realize o logout de forma segura, encerrando a sessão ativa e redirecionando-o para a página inicial ou de login, garantindo a proteção das informações pessoais e impedindo acessos não autorizados. 

RF9 

Gerenciamento de Quartos 

O sistema deve permitir que administradores realizem o processamento completo de quartos, incluindo o cadastro de novos quartos com todas as suas informações (descrição, tipo, capacidade, preço, comodidades e disponibilidade), a exclusão de quartos existentes, a consulta detalhada de dados de cada quarto e a edição de informações previamente cadastradas, garantindo que apenas usuários com perfil de administrador tenham acesso a essas funcionalidades. 

RF10 

Gerenciamento de valores 

O sistema deve permitir que administradores alterem os valores das diárias dos quartos conforme as datas selecionadas, possibilitando a definição de preços diferenciados por temporada, finais de semana ou feriados, além de permitir a adição de promoções, como descontos percentuais ou valores fixos, com período de validade definido. 

RF11 

Gerenciamento de reservas 

O sistema deve permitir que administradores visualizem e gerenciem todas as reservas realizadas, com acesso a informações como nome do hóspede, datas da estadia, tipo de quarto, status da reserva e forma de pagamento, além de possibilitar ações como confirmação, edição, cancelamento e geração de relatórios. 

 

RF12 

Gerenciamento de Usuários 

 

O sistema deve permitir que administradores cadastrem e configurem níveis de acesso para diferentes perfis de usuário, como hóspedes, recepcionistas e administradores, definindo permissões específicas para cada tipo de perfil, como visualização, edição, exclusão e gerenciamento de dados, garantindo o controle adequado das funcionalidades disponíveis conforme a função do usuário. 

 

 

3.3.1 Requisitos Não Funcionais 

 

Código  

Restrição 

Descrição 

RNF1 

Ambiente 

O sistema deve ser executado diretamente no navegador, garantindo compatibilidade com os principais navegadores modernos. 

RNF2 

Responsabilidade 

O sistema deve ser responsivo em todos os dispositivos, adaptando automaticamente sua interface a diferentes tamanhos de tela e resoluções, garantindo um funcionamento adequado e consistente em plataformas como computadores, notebooks, tablets e smartphones. 

RNF3 

Segurança 

O produto deve restringir o acesso por meio de senhas individuais para cada usuário, garantindo que apenas pessoas autorizadas consigam acessar suas contas, com validação segura das credenciais e possibilidade de recuperação de senha em caso de esquecimento. 

RNF4 

Conformidade  

 Legal 

O sistema deverá cumprir integralmente a Lei Geral de Proteção de Dados (LGPD) no tratamento de dados pessoais, adotando medidas técnicas e administrativas para garantir a privacidade, a segurança, o consentimento explícito do usuário, o acesso às informações armazenadas, bem como a possibilidade de retificação ou exclusão dos dados, conforme previsto na legislação. 

RNF5 

Usabilidade 

O sistema deve possuir uma interface estruturada para atender aos objetivos funcionais da aplicação, permitindo que usuários realizem tarefas como reservas, gerenciamento de quartos, controle de usuários e processamento de pagamentos de forma clara, eficiente e alinhada às necessidades de cada perfil de acesso. 

RNF 6 

Desempenho 

O sistema deve garantir tempo de resposta adequado para atualização de informações, processando alterações realizadas pelos usuários, como edição de dados cadastrais, status de reservas ou valores de quartos. 

 

3.3.2 Usuários  

 

Descrição 

# 

Ator 

Definição 

1 

Hóspede 

Usuário responsável por agendar e gerenciar suas reservas. 

2 

Recepcionista 

Usuário responsável por consultar e averiguar as informações de reserva e disponibilidade de quarto. 

3 

Administrador 

Usuário gerente do sistema responsável pelo cadastro e manutenção da disponibilidade de quarto. 

 

3.4 Modelagem do Sistema 

 

3.4.1 Diagrama de Casos de Uso 

    Como observado no diagrama de casos de uso da Figura 1, o hóspede poderá gerenciar os dados pessoais, visualizar a disponibilidade de quartos e fazer reservas. O recepcionista poderá visualizar todas as reservas disponíveis, e o administrador, além dessas funções, poderá gerenciar todos os dados relacionados às reservas, informações de quartos e gestão de acessos. 

 

Imagem 

Figura 1: Diagrama de Casos de Uso do Sistema. 

3.4.2 Descrições de Casos de Uso 

 

Cada caso de uso deve ter a sua descrição representada nesta seção. Exemplo: 

 

Cadastrar informações pessoais (CSU01) 

Sumário: O hóspede cadastra suas informações pessoais no sistema, como nome completo, e-mail válido, número de telefone, data de nascimento e uma senha segura para utilizar os demais serviços oferecidos, como simulação e finalização de reservas. 

Ator Primário: Hóspede. 

Ator Secundário: Nenhum. 

Pré-condições: O hóspede deve acessar o sistema pela interface de cadastro. 

Fluxo Principal: 

O hóspede acessa a interface de cadastro. 

O sistema apresenta um formulário para preenchimento de dados pessoais: nome completo, e-mail válido, número de telefone, data de nascimento e uma senha segura. 

O hóspede preenche os dados solicitados. 

O sistema valida as informações fornecidas. 

Se os dados forem válidos, o sistema salva as informações no banco de dados e confirma o cadastro. 

O sistema redireciona o hóspede para a página inicial. 

Fluxo Alternativo (4): Dados inválidos 

O sistema identifica que uma ou mais informações são inválidas (ex.: e-mail no formato incorreto, número de telefone já cadastrado, campos obrigatórios não preenchidos). 

O sistema apresenta uma mensagem de erro destacando os campos inválidos. 

O hóspede corrige os dados e retorna ao passo 4 do fluxo principal. 

 

Pós-condições: O hóspede estará cadastrado no sistema com seus dados pessoais armazenados corretamente. 

 

Simular reserva (CSU02) 

Sumário: O hóspede simula uma reserva, visualizando a disponibilidade de quartos, tipos de acomodações, datas e valores sem precisar efetuar a reserva de fato. 

Ator Primário: Hóspede. 

Ator Secundário: Nenhum. 

Pré-condições: O hóspede deve estar com acesso ao sistema (não exige login). 

Fluxo Principal: 

O Hóspede acessa a página de “acomodações” no sistema. 

O sistema solicita informações como: data de entrada, data de saída, número de pessoas, tipo de quarto desejado. 

O hóspede preenche os dados. 

O sistema verifica a disponibilidade de quartos com base nos critérios informados. 

O sistema apresenta os quartos disponíveis e seus respectivos valores. 

O hóspede analisa as opções e pode optar por voltar ou seguir para a finalização da reserva. 

 

Pós-condições: O sistema exibe os resultados da simulação de reserva para o hóspede. 

Finalizar reserva (CSU03) 

Sumário: O hóspede finaliza uma reserva a partir de uma simulação, confirmando os dados e prosseguindo para o pagamento. 

Ator Primário: Hóspede. 

Ator Secundário: Nenhum. 

Pré-condições: O hóspede deve ter feito uma simulação de reserva. O hóspede deve estar logado no sistema. 

Fluxo Principal: 

O sistema exibe os dados da reserva para confirmação (datas, número de hóspedes, valor, tipo de quarto). 

O hóspede confirma os dados da reserva. 

O sistema direciona o hóspede para a funcionalidade de pagamento. 

Após a confirmação do pagamento, o sistema registra a reserva. 

O sistema exibe uma mensagem de sucesso com o número da reserva e os dados confirmados. 

     

Pós-condições: O sistema exibe os resultados da simulação de reserva para o hóspede. 

Fluxo Alternativo (1): Desistência 

O hóspede opta por não prosseguir com o pagamento. 

O sistema cancela a finalização da reserva e retorna à tela anterior. 

Fluxo Alternativo (4): Pagamento não realizado 

O sistema não consegue verificar o pagamento em um determinado limite de tempo. 

Um e-mail é enviado ao usuário avisando que o pagamento não foi realizado e o hóspede deve refazer o processo de reserva. 

Pós-condições: A reserva do hóspede foi registrada no sistema com status confirmado. 

 

Realizar pagamento (CSU04) 

Sumário: Permite que o hóspede realize o pagamento de uma reserva previamente finalizada, redirecionando ao sistema de pagamento. 

Ator Primário: Hóspede. 

Ator Secundário: Nenhum. 

Pré-condições: O hóspede deve estar logado no sistema e ter simulado uma reserva. 

Fluxo Principal: 

O sistema redireciona o usuário para o aplicativo de pagamento. 

O sistema aguarda a resposta da ferramenta de pagamento. 

O sistema exibe a confirmação de pagamento aprovado. 

A reserva é marcada como “Confirmada”. 

 

Fluxo Alternativo (1): Pagamento não realizado 

O sistema não consegue verificar o pagamento em um determinado limite de tempo. 

Um e-mail é enviado ao usuário avisando que o pagamento não foi realizado e o hóspede deve refazer o processo de reserva. 

O hóspede refaz o processo de reserva. 

Pós-condições: A reserva está paga e confirmada no sistema. 

 

Realizar Login e Logout (CSU05) 

Sumário: Permite que o hóspede, recepcionista ou administrador se autentique no sistema ou encerre a sessão. 

Ator Primário: Hóspede, Recepcionista, Administrador 

Ator Secundário: Nenhum. 

Pré-condições: O usuário deve possuir um cadastro no sistema. 

Fluxo Principal (Login): 

O usuário acessa a tela de login. 

O sistema solicita e-mail e senha. 

O usuário fornece as credenciais. 

O sistema valida os dados. 

O sistema autentica o usuário e o redireciona para a tela inicial conforme o seu perfil (hóspede, recepcionista ou administrador). 

 

Fluxo Alternativo (4): Dados Inválidos 

O sistema informa que os dados estão incorretos. 

O usuário pode tentar novamente. 

Fluxo Principal (Logout): 

O usuário solicita logout. 

O sistema encerra a sessão e retorna à página inicial. 

Pós-condições: Usuário está autenticado (ou deslogado) no sistema. 

 

 

 

Gerenciar seus dados (CSU06) 

Sumário: Permite que o hóspede altere suas informações pessoais e edite ou cancele suas reservas. 

Ator Primário: Hóspede. 

Ator Secundário: Nenhum. 

Pré-condições: O hóspede deve estar autenticado no sistema. 

Fluxo Principal: 

O hóspede acessa a área de gerenciamento de conta. 

O sistema exibe as opções de alteração de dados pessoais e reservas. 

O hóspede escolhe editar informações pessoais. 

O sistema exibe o formulário com os dados atuais. 

O hóspede atualiza os dados e confirma. 

O sistema valida e salva as alterações. 

O hóspede pode também visualizar suas reservas e selecionar uma delas. 

O sistema exibe os detalhes da reserva selecionada. 

O hóspede pode alterar dados permitidos (como data, número de hóspedes) ou cancelar a reserva. 

O sistema valida as alterações ou confirma o cancelamento. 

Fluxo Alternativo (6): Dados inválidos 

O sistema notifica o erro e solicita correção dos dados. 

Pós-condições: As informações pessoais e/ou reservas foram atualizadas com sucesso ou canceladas. 

 

Visualizar reservas efetuadas pelos hóspedes (CSU07) 

Sumário: Permite que o recepcionista e o administrador acessem o histórico de reservas realizadas por todos os hóspedes. 

Ator Primário: Recepcionista e Administrador 

Ator Secundário: Nenhum. 

Pré-condições: O recepcionista deve estar autenticado no sistema. 

Fluxo Principal: 

O recepcionista e administrador acessa a área de gestão de reservas. 

O sistema exibe uma lista de filtros (data, nome do hóspede, status da reserva). 

O recepcionista e administrador aplica os filtros desejados. 

O sistema apresenta a lista de reservas correspondentes. 

O recepcionista e administrador pode visualizar os detalhes de uma reserva específica. 

Pós-condições: O recepcionista visualizou as reservas realizadas pelos hóspedes. 

 

Consultar dados dos hóspedes (CSU08) 

Sumário: Permite que o recepcionista e administrador consulte informações detalhadas dos hóspedes cadastrados. 

Ator Primário: Recepcionista e Administrador 

Ator Secundário: Nenhum. 

Pré-condições: O recepcionista deve estar autenticado no sistema. 

Fluxo Principal: 

O recepcionista acessa a funcionalidade de consulta de hóspedes. 

O sistema apresenta opções de busca (por nome, e-mail, telefone). 

O recepcionista informa um dos dados de busca. 

O sistema retorna uma lista de hóspedes correspondentes. 

O recepcionista seleciona um hóspede. 

O sistema exibe as informações detalhadas do hóspede (nome, contato, histórico de reservas etc.). 

Pós-condições: O recepcionista obteve as informações necessárias sobre um ou mais hóspedes. 

Gerenciar usuários e níveis de acesso (CSU09) 

Sumário: Permite ao administrador cadastrar, editar e excluir usuários do sistema, além de definir seus respectivos níveis de acesso (ex: recepcionista, administrador). 

Ator Primário: Administrador. 

Ator Secundário: Nenhum. 

Pré-condições: O administrador deve estar autenticado no sistema. 

Fluxo Principal: 

O administrador acessa a área de gerenciamento de usuários. 

O sistema apresenta a lista de usuários existentes e opções de ações (cadastrar, editar, excluir). 

O administrador seleciona "Cadastrar novo usuário". 

O sistema solicita os dados do novo usuário (nome, e-mail, senha, nível de acesso). 

O administrador fornece os dados e confirma. 

O sistema valida e salva o novo usuário. 

Fluxo Alternativo (3): Editar usuário 

O administrador seleciona um usuário da lista e escolhe "Editar". 

O sistema exibe os dados atuais. 

O administrador altera as informações e confirma. 

O sistema salva as alterações. 

Fluxo Alternativo (3): Excluir usuário 

O administrador seleciona um usuário e escolhe "Excluir". 

O sistema solicita confirmação. 

 O administrador confirma. 

O sistema remove o usuário. 

Pós-condições: Um usuário foi cadastrado, alterado ou excluído, e seu nível de acesso foi configurado corretamente. 

Cadastrar, editar e excluir quartos (CSU10) 

Sumário: Permite ao administrador manter o cadastro de quartos disponíveis para reservas. 

Ator Primário: Administrador 

Ator Secundário: Nenhum. 

Pré-condições: O administrador deve estar autenticado no sistema. 

Fluxo Principal: 

O administrador acessa o menu de gerenciamento de quartos. 

O sistema apresenta uma lista com os quartos já cadastrados e opções de ações (cadastrar, editar, excluir). 

O administrador seleciona "Cadastrar novo quarto". 

O sistema solicita os dados (número do quarto, tipo, capacidade, comodidades, preço padrão). 

O administrador fornece os dados e confirma. 

O sistema valida e salva o novo quarto. 

 

Fluxo Alternativo (3): Editar quarto 

O administrador seleciona um quarto da lista e escolhe "Editar". 

O sistema exibe os dados atuais. 

O administrador altera as informações e confirma. 

O sistema salva as alterações. 

Fluxo Alternativo (3): Excluir quarto 

O administrador seleciona um quarto e escolhe "Excluir". 

O sistema solicita confirmação. 

O administrador confirma. 

O sistema remove o quarto. 

Pós-condições: Um quarto foi cadastrado, alterado ou excluído com sucesso. 

 

Alterar valores dos quartos por data (CSU11) 

Sumário: Permite ao administrador definir preços diferentes para os quartos com base em datas específicas (alta/baixa temporada, feriados, etc). 

Ator Primário: Administrador. 

Ator Secundário: Nenhum. 

Pré-condições: O administrador deve estar autenticado no sistema. 

Fluxo Principal: 

O administrador acessa a funcionalidade de alteração de preços por data. 

O sistema apresenta os quartos cadastrados e um calendário com os valores atuais. 

O administrador seleciona o quarto e a data desejada. 

O sistema permite editar o valor para aquela data. 

O administrador fornece o novo valor e confirma. 

O sistema atualiza o preço. 

Pós-condições: O valor do quarto foi ajustado com sucesso para a(s) data(s) selecionada(s). 

Criar Promoções (CSU12) 

Sumário: Permite ao administrador criar promoções que podem afetar os valores dos quartos. 

Ator Primário: Administrador. 

Ator Secundário: Nenhum. 

Pré-condições: O administrador deve estar autenticado no sistema. 

Fluxo Principal: 

O administrador acessa a área de promoções. 

O sistema exibe as promoções já cadastradas e a opção de criar. 

O administrador seleciona "Criar nova promoção". 

O sistema solicita os dados da promoção (nome, descrição, data de início/fim, tipo de desconto, valor/porcentagem). 

O administrador fornece as informações e confirma. 

O sistema salva a promoção. 

A promoção fica associada às datas e aos quartos elegíveis, afetando o valor conforme o CSU11 (via <<extend>>). 

Pós-condições: A promoção foi criada com sucesso e está ativa no sistema dentro do período configurado. 

 

3.4.3 Diagrama de Classes  

   A Figura 2 mostra o diagrama de classes do sistema de reservas. A Reserva deve conter a identificação do funcionário responsável pelo registro, bem como os dados do hóspede e do quarto reservado. Um quarto pode ter diversas reservas, mas pertence a apenas um tipo de quarto. Promoções podem ser aplicadas a diferentes reservas, e os preços podem variar de acordo com o período. REVISAR 

Imagem 

Figura 2: Diagrama de Classes do Sistema. 

 

3.4.3 Descrições das Classes  

# 

Nome 

Descrição 

 

Usuário 

Cadastro geral de usuários, edição das informações, login e logout, além da criação e alteração de senhas. 

 

Funcionário  

Visualização de reservas e consulta de hóspedes  

 

Recepcionista 

O recepcionista de hotel é responsável por receber e atender hóspedes, realizar check-ins e check-outs, fornecer informações sobre o hotel e arredores, atender telefonemas, fazer reservas e manter a organização da recepção. Atua como o primeiro ponto de contato entre o hóspede e o hotel. 

 

 

Administrador  

Gerenciamento de quartos e usuários e criação de promoções. 

 

Hóspede 

hóspede é a pessoa que se hospeda em um hotel, utilizando seus serviços e acomodações por um período determinado, seja a lazer, trabalho ou outros motivos. 

 

Quarto 

quarto de hotel é o espaço reservado para o hóspede descansar e se acomodar durante sua estadia. Ele pode incluir cama, banheiro privativo, TV, frigobar, ar-condicionado e outros itens, variando conforme o padrão do hotel. 

 

Tipo de Quarto 

 

 

Reserva 

Reserva é o ato de garantir antecipadamente um quarto no hotel para uma data específica. Pode ser feita por telefone, site, aplicativo ou pessoalmente, e inclui dados como nome do hóspede, datas de entrada e saída, tipo de quarto e forma de pagamento.... 

 

Pagamento  

Pagamento é o processo pelo qual o hóspede quita os valores referentes à estadia e serviços usados no hotel. Pode ser feito no momento da reserva, no check-in ou check-out, e os meios mais comuns incluem dinheiro, cartão de crédito/débito, PIX ou transferência bancária. 

 

Promoção 

Promoção em hotelaria é uma oferta especial com descontos ou benefícios para atrair mais hóspedes. Pode incluir preço reduzido, noites grátis, upgrades de quarto, café da manhã incluso ou pacotes com serviços extras. Normalmente é válida por tempo limitado ou em datas específicas. 

 

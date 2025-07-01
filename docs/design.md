# 4. PROJETO DO DESIGN DE INTERAÇÃO

## 4.1 Personas
### Persona 1: Carla Mendes
![image](https://github.com/user-attachments/assets/219fced3-8e9e-47d9-8273-d54ccaf9124e)
### Persona 2: Diego Costa
![image](https://github.com/user-attachments/assets/86189995-7b6c-4d90-a5ad-285cb713cf5f)
### Persona 3: Lucas Ferreira
![image](https://github.com/user-attachments/assets/605c9422-582c-45eb-9811-0785952cff69)
### Persona 4: Mariana
![image](https://github.com/user-attachments/assets/04c46ca1-7ec0-48b2-8013-cba9fa6d6015)


## 4.2 Mapa de Empatia
### Persona 1: Carla Mendes 

![image](https://github.com/user-attachments/assets/d91605ad-fcaa-4c1d-b8c0-032528f28ac2)

### Persona 2: Diego Costa 

![image](https://github.com/user-attachments/assets/472c7590-a3a6-401a-bc97-df1c44b160a6)

### Persona 3: Lucas 

![image](https://github.com/user-attachments/assets/b41d6207-8aa5-4d01-bc27-776af6d63707)

### Persona 4: Mariana 
![image](https://github.com/user-attachments/assets/46664015-8bd8-4eac-b0b5-1bd2ab783216)


## 4.3 Protótipos das Interfaces 

### 1. Tela de Login 

![image](https://github.com/user-attachments/assets/0b46a87f-c890-4065-a2a8-d758a07231f1)

#### Objetivo da Tela 

A tela de login tem como principal função autenticar o usuário de forma rápida, clara e segura, servindo como ponto de entrada para os diferentes perfis: administrador, recepcionista e cliente. Essa etapa garante o acesso apenas a usuários autorizados, respeitando os níveis hierárquicos de uso no sistema hoteleiro. 

#### Princípios Gestálticos 

Proximidade: Elementos relacionados, como campos de "e-mail" e "senha", são agrupados visualmente e posicionados próximos, facilitando a identificação da tarefa de login como única e coesa; 

Similaridade: Botões, ícones e campos seguem padrões visuais semelhantes (mesmo estilo, cor e fonte), promovendo reconhecimento imediato do que pode ser clicado ou editadol; 

Continuidade: O alinhamento dos campos e botões segue uma linha vertical clara, conduzindo o olhar naturalmente do topo para o botão de login; 

Figura-fundo: O formulário de login se destaca do plano de fundo, permitindo foco visual direto nos elementos interativos; 

Fechamento: Elementos visuais como caixas delimitadas reforçam a forma completa do formulário, mesmo com uma estética clean, reforçando o entendimento da função da tela. 

#### Regras de Ouro 

Consistência: Terminologias, botões e ícones são usados uniformemente em toda a plataforma; 

Atalhos: A função de manter login salvo (“lembrar-me”) ajuda usuários recorrentes; 

Redução da Carga de Memória: Campos bem rotulados e o uso de placeholders orientam o usuário a todo momento; 

Prevenção de erros: Validações impedem o envio com campos vazios e informam erros como “formato de e-mail inválido”. 

#### Recomendações Ergonômicas 

Consistência: Cores, estilos de botões e estruturas de menus seguem o padrão das outras telas do sistema, promovendo coerência visual; 

Clareza: Layout limpo, fonte legível (sans-serif), contraste adequado e ícones descritivos ajudam o usuário a entender sua tarefa sem confusão; 

Prevenção e recuperação de erros: Mensagens de erro são específicas (“senha incorreta”, “usuário não encontrado”) e oferecem instruções para corrigir o problema; 

Controle do usuário: Usuários redefinir senha, mantendo autonomia sobre a ação; 

Eficiência: A tela exige o mínimo de esforço: dois campos + botão + opção de recuperação de senha. 

### 2. Tela de Cadastro

![image](https://github.com/user-attachments/assets/14499437-5225-4cca-97f5-108ecbb04e12)

#### Objetivo da Tela 

A tela de cadastro tem como função registrar novos usuários no sistema, sejam clientes (hóspedes) ou funcionários (recepcionistas e administradores). Seu objetivo é coletar informações básicas de forma rápida, intuitiva e segura, promovendo a inclusão de usuários com diferentes níveis de familiaridade com tecnologia. 

#### Princípios Gestálticos 

Proximidade: Campos são agrupados por categoria, tornando a leitura mais organizada; 

Similaridade: Todos os campos de entrada têm o mesmo estilo visual (bordas arredondadas, mesma fonte e tamanho), reforçando a uniformidadel; 

Continuidade: A disposição vertical e ordenada dos campos leva o usuário a seguir um fluxo natural de preenchimento; 

Figura-fundo: O formulário de cadastro se destaca claramente sobre o plano de fundo da tela; 

Fechamento: Grupos de campos são visualmente delimitados, transmitindo a sensação de “completude” de seções. 

#### Regras de Ouro 

Consistência: Mesma paleta de cores, fontes e botões usados na tela de login são mantidos aqui; 

Atalhos: Usuários recorrentes podem ser redirecionados rapidamente à tela de login; 

Redução da Carga de Memória: Campos possuem etiquetas claras e ajuda contextual; 

Feedback informativo: Cada campo tem validação em tempo real (por exemplo: “senha muito curta”, “e-mail inválido”), com ícones e mensagens de feedback. 

#### Recomendações Ergonômicas 

Consistência: O layout do formulário segue a identidade visual do sistema e mantém os padrões interativos; 

Clareza: Campos bem identificados com legendas legíveis, evitando siglas técnicas ou termos ambíguos; 

Prevenção e recuperação de erros: Erros são detectados e exibidos de forma clara (ex: “Telefone deve conter 11 dígitos”), permitindo correção imediata; 

Controle do usuário: Usuários escolhem se desejam salvar a senha; 

Eficiência: O formulário solicita apenas dados necessários para o primeiro acesso (e-mail e senha). Dados complementares podem ser inseridos posteriormente. 

 

### 3. Tela de Criação de Perfil
![image](https://github.com/user-attachments/assets/23ea8e42-3003-4a1f-a9fe-1c853d914579)

#### Objetivo da Tela 

A tela de criação de perfil é exibida após o primeiro login ou cadastro, e tem como função permitir ao usuário personalizar sua conta, definindo: 

Uma foto de perfil (opcional, mas recomendada) 

Seu nome completo 

Sua função no sistema (hóspede ou funcionário) 

Uma descrição curta do seu perfil (campo livre para bio, cargo, preferências, e etc.) 

Essa tela personaliza a experiência e ajusta o sistema de acordo com o tipo de usuário, oferecendo uma interface mais amigável, conectada com as necessidades reais de cada perfil. 

#### Princípios Gestálticos 

Proximidade: Os campos são organizados por blocos funcionais: imagem, dados pessoais, descrição. Isso ajuda o usuário a compreender que cada grupo tem um propósito específico; 

Similaridade: Todos os campos de entrada seguem o mesmo padrão visual. Botões e menus compartilham a mesma identidade de design, reforçando a consistência; 

Continuidade: O layout é vertical, com alinhamento à esquerda, conduzindo o olhar do topo da página (foto) ao final (botão de salvar), criando uma progressão lógica; 

Figura-fundo: A área de preenchimento se destaca sobre o fundo da página, facilitando o foco na tarefa; 

Fechamento: Os elementos do formulário estão dentro de um card ou contêiner delimitado, reforçando visualmente a conclusão da tarefa de preenchimento. 

#### Regras de Ouro 

Consistência: Elementos visuais e interativos seguem o padrão de outras telas (botões, fontes, cores, posicionamento); 

Atalhos: Para usuários avançados, há opção de pular a personalização neste momento (com botão “Fazer depois”); 

Redução da Carga de Memória: Uso de ícones intuitivos e exemplos no placeholder reduzem dúvidas; 

Feedback informativo: Após clicar em "Salvar e continuar", o usuário recebe uma confirmação. 

#### Recomendações Ergonômicas 

Consistência: Os controles de interface (inputs, botões, seleção de função) seguem o mesmo padrão visual já utilizado no sistema; 

Clareza: Títulos diretos, campos bem rotulados e botões com verbos de ação; 

Prevenção e recuperação de erros: O sistema exibe mensagens específicas para campos em branco obrigatórios ou arquivos de imagem em formato não permitido; 

Controle do usuário: O usuário pode escolher se quer adicionar foto e descrição agora ou depois; 

Eficiência: Apenas os campos essenciais são obrigatórios. O processo é rápido e fluido. 

 

### 4. Tela de Recuperação de Senha 
![image](https://github.com/user-attachments/assets/a7458281-a943-4542-b9e4-0da3109aa01f)

#### Objetivo da Tela 

A tela de recuperação de senha tem como objetivo permitir que usuários que esqueceram sua senha possam recuperá-la de maneira segura, simples e confiável. Nela, o usuário: 

Informa o e-mail cadastrado no sistema 

Clica no botão “Enviar link de recuperação” 

Recebe no e-mail um link para redefinir sua senha 

Essa funcionalidade é fundamental para garantir a continuidade do acesso ao sistema. 

#### Princípios Gestálticos 

Proximidade: O campo de e-mail e o botão de envio estão próximos, indicando que pertencem à mesma ação; 

Similaridade: Segue o mesmo padrão estético das outras telas do sistema (login, cadastro), com campos e botões uniformes; 

Continuidade: O fluxo é linear: da instrução para o campo de preenchimento → clique no botão → mensagem de confirmação; 

Figura-fundo: O formulário é destacado sobre o fundo da página com alto contraste e layout centrado, facilitando o foco; 

Fechamento: A interface transmite claramente que a ação está completa após o envio (exibe mensagem "Enviamos um link para seu e-mail"). 

#### Regras de Ouro 

Consistência: Cores, tipografia, botões e estrutura são consistentes com o resto do sistema; 

Atalhos: Ao digitar o e-mail, pressionar "Enter" também executa o envio, além do botão de clique; 

Redução da Carga de Memória: A interface solicita apenas um dado (e-mail), minimizando esforço cognitivo; 

Feedback informativo: Após o envio, o sistema informa: “Um link de redefinição foi enviado para seu e-mail.” 

#### Recomendações Ergonômicas 

Consistência: A interface mantém o layout, botões e estilo das demais telas do sistema; 

Clareza: A mensagem explicativa é direta e posicionada acima do campo; 

Prevenção e recuperação de erros: O campo possui verificação automática de formato, e a mensagem de erro é clara: “E-mail não encontrado” ou “Formato inválido”; 

Controle do usuário: O botão “Voltar” e o feedback visual dão segurança e flexibilidade ao usuário; 

Eficiência: Com apenas um campo e um botão, o processo é concluído em segundos. 

 

 

### 5. Tela de Edição de Perfil
![image](https://github.com/user-attachments/assets/8a188026-8775-4c77-8cf1-c400d5921f4c)

#### Objetivo da Tela 

A tela de edição de perfil permite que o usuário atualize suas informações pessoais já cadastradas no sistema, incluindo: 

Foto de perfil 

Nome completo 

Função (hóspede ou funcionário) 

Descrição pessoal 

Seu propósito é garantir que o usuário mantenha seus dados atualizados de forma fácil, clara e segura, promovendo uma experiência personalizada e flexível. 

#### Princípios Gestálticos 

Proximidade: Campos relacionados permanecem agrupados, o que ajuda na identificação do propósito de cada seção; 

Similaridade: Estética dos campos e botões segue padrão visual da criação de perfil, mantendo a consistência de aprendizado; 

Continuidade: O layout segue a ordem lógica: imagem → nome → função → descrição → botões; 

Figura-fundo: O formulário é destacado visualmente, com áreas claras de entrada de dados e fundo neutro, mantendo o foco do usuário; 

Fechamento: Os grupos de campos e as ações finais estão organizados em contêineres que sugerem completude da tarefa. 

#### Regras de Ouro 

Consistência: Todos os elementos interativos seguem o padrão já utilizado no sistema; 

Atalhos: Usuários podem navegar diretamente até o campo que desejam editar; 

Redução da Carga de Memória: Todos os dados anteriores são carregados automaticamente nos campos, evitando retrabalho; 

Feedback informativo: Ao salvar alterações, o sistema exibe uma mensagem como “Perfil atualizado com sucesso”. 

#### Recomendações Ergonômicas 

Consistência: Toda a estrutura e estilo seguem o modelo de criação de perfil, facilitando o reconhecimento de funções; 

Clareza: Texto claro, labels bem definidos, botões de ação com comandos diretos; 

Prevenção e recuperação de erros: Avisos de erro com mensagens claras, validação de campos e sistema de confirmação antes de aplicar mudanças; 

Controle do usuário: Total liberdade para editar somente o necessário, com opções de sair, cancelar ou salvar; 

Eficiência: Edição rápida e direta. O campo alterado pode ser salvo em poucos cliques. 

 

### 6. Tela de Perfil 
![image](https://github.com/user-attachments/assets/24965e3e-3c03-4a53-9838-cec0c8fc2b96)

#### Objetivo da Tela 

A tela de perfil é uma interface de consulta que permite ao usuário visualizar suas informações pessoais e acessar funcionalidades relacionadas à sua conta. Os principais elementos exibidos são: 

Foto de perfil 

Nome completo do usuário 

E-mail cadastrado 

Acesso à página de edição de perfil 

Acesso ao suporte 

Acesso aos termos de uso 

Botão de logout (sair do sistema) 

Essa tela cumpre um papel essencial de centralizar informações pessoais e serviços relacionados à conta, de forma clara e acessível para qualquer tipo de usuário. 

#### Princípios Gestálticos 

Proximidade: Informações pessoais (foto, nome e e-mail) estão agrupadas na parte superior; ações (editar, suporte, termos, sair) ficam organizadas em uma lista ou menu abaixo, facilitando a identificação funcional; 

Similaridade: Links e botões seguem o mesmo padrão visual (ícones + texto), criando uma interface intuitiva e uniforme; 

Continuidade: O fluxo da tela vai do topo (dados do usuário) para baixo (ações e saída), favorecendo a leitura natural (de cima para baixo); 

Figura-fundo: A foto do perfil e as informações estão destacadas sobre um fundo neutro, chamando atenção para o conteúdo principal; 

Fechamento: Cada seção tem seu espaço bem definido, com margens e divisórias visuais, reforçando o encerramento da área de conteúdo. 

#### Regras de Ouro 

Consistência: Toda a interface segue o mesmo estilo visual e padrão de navegação do sistema; 

Atalhos: Links rápidos para edição de perfil e logout agilizam a navegação para usuários habituados ao sistema; 

Redução da Carga de Memória: Informações básicas são mostradas diretamente na tela, sem necessidade de memorização; 

Feedback informativo: Ao clicar em “Editar perfil”, “Suporte” ou “Termos de uso”, o sistema fornece transições suaves. 

#### Recomendações Ergonômicas 

Consistência: Os ícones e botões seguem o mesmo padrão das outras interfaces (edição, suporte, sair); 

Clareza: A tela tem hierarquia visual clara: título, informações pessoais, e uma lista de ações; 

Prevenção e recuperação de erros: Ações críticas, como sair, são protegidas com mensagens de confirmação; 

Controle do usuário: O usuário pode sair da conta, editar dados ou acessar suporte quando quiser; 

Eficiência: Tudo o que o usuário precisa em relação à conta está centralizado e acessível em um clique. 

 

### 7. Tela de Homepage ("página inicial")
![image](https://github.com/user-attachments/assets/e029e429-4cea-4802-91b7-853c4e0990ab)

#### Objetivo da Tela 

A Homepage é o primeiro ponto de contato do visitante com o sistema. Seu objetivo é: 

Permitir a busca de hospedagem por data, com base nas preferências do usuário; 

Exibir os quartos disponíveis de maneira clara, atrativa e funcional; 

Oferecer acesso rápido às ações principais: Cadastro e Login. 

Essa tela é voltada tanto para visitantes (usuários não logados) quanto para usuários recorrentes que desejam visualizar e reservar quartos com agilidade. 

#### Princípios Gestálticos 

Proximidade: Elementos relacionados (filtros de data, resultados de busca, botões de ação) estão agrupados logicamente, o que guia a leitura e a navegação da página; 

Similaridade: Cada “cartão de quarto” (imagem, nome, descrição, valor, botão de reserva) possui o mesmo layout, o que facilita a leitura e comparação; 

Continuidade: A leitura segue um fluxo natural: topo (ações) → meio (filtros) → base (resultados de busca), respeitando o padrão de navegação ocidental (de cima para baixo, da esquerda para a direita); 

Figura-fundo: Os anúncios de quartos estão em caixas com bordas ou sombreamento, destacando-os do fundo da página; 

Fechamento: Cada quarto é exibido em um “cartão” fechado visualmente, facilitando a percepção de onde começa e termina a informação. 

#### Regras de Ouro 

Consistência: Botões, ícones e campos seguem o mesmo padrão de design presente nas outras telas do sistema; 

Atalhos: O usuário pode clicar diretamente em “Entrar” ou “Cadastrar” no topo da tela, sem precisar rolar; 

Redução da Carga de Memória: As informações essenciais dos quartos (nome, valor, descrição, botão de reservar) estão todas visíveis no cartão, sem necessidade de abrir outra página; 

Feedback informativo: Após selecionar as datas, o sistema informa imediatamente os quartos disponíveis ou uma mensagem como “Nenhum quarto disponível para o período”. 

#### Recomendações Ergonômicas 

Consistência: Layout idêntico entre os cartões de quartos; botões e interações uniformes em toda a interface; 

Clareza: Campo de data com rótulo explícito (“Check-in”, “Check-out”) e uso de calendários interativos com datas disponíveis; 

Prevenção e recuperação de erros: Caso nenhuma data seja selecionada, botão de “Reservar” permanece desativado, com aviso “Informe as datas primeiro”; 

Controle do usuário: Navegação livre, sem redirecionamentos automáticos ou pop-ups inesperados; 

Eficiência: Processo de busca é rápido: selecionar datas → ver resultados → reservar com 1 clique. 

 

### 8. Tela de Detalhamento do Quarto
![image](https://github.com/user-attachments/assets/b3322781-7bb4-46ed-8168-696c5857e9ac)

#### Objetivo da Tela 

A tela de detalhamento do quarto tem como finalidade apresentar, de forma clara e atrativa, todas as informações relevantes sobre um quarto específico, com foco em: 

Ajudar o usuário a tomar a decisão de reserva com confiança 

Exibir características completas do quarto (visual, capacidade, comodidades) 

Permitir acesso rápido ao botão de reserva 

Essa tela é fundamental para promover a transparência e melhorar a experiência do cliente na fase de decisão. 

#### Princípios Gestálticos 

Proximidade: Informações relacionadas (capacidade, banheiros, avaliação) são agrupadas logo abaixo das imagens; 

Similaridade: Ícones representando camas, banheiros e estrelas seguem o mesmo estilo visual, facilitando a compreensão imediata; 

Continuidade: O layout guia o olhar do usuário de cima para baixo, mantendo a sequência lógica: imagem → dados técnicos → nome e botão → valor → amenidades → descrição; 

Figura-fundo: As imagens do quarto ocupam a área de maior destaque, com fundo claro para dar foco visual. O botão de reserva tem cor de destaque para se sobressair; 

Fechamento: Cada seção (dados técnicos, botão de reserva, amenidades) está visualmente separada com margens, sombras ou blocos, dando a sensação de agrupamento completo. 

#### Regras de Ouro 

Consistência: Ícones, tipografia e estrutura visual seguem o mesmo padrão das outras telas do sistema; 

Atalhos: O botão de “Reservar” é imediatamente visível sem necessidade de rolagem em telas maiores; 

Redução da Carga de Memória: Todas as informações necessárias para decisão estão visíveis em uma só tela, sem necessidade de navegação adicional; 

Feedback informativo: Ao clicar em “Reservar”, o sistema vai redirecionar para a finalização com destaque visual. 

#### Recomendações Ergonômicas 

Consistência: Mesmo estilo de botões, cores e ícones usados nas outras telas de navegação do sistema; 

Clareza: Informações organizadas em blocos com títulos como “Amenidades” e “Descrição do Quarto”; 

Prevenção e recuperação de erros: Quartos indisponíveis são destacados e não permitem cliques em “Reservar”; 

Controle do usuário: Ele decide quando e se vai clicar em reservar; sem ações automáticas que o pressionem; 

Eficiência: Botão de reserva acessível logo ao lado dos dados principais, sem necessidade de rolagem excessiva. 

 

### 9. Tela de Finalização da Reserva
![image](https://github.com/user-attachments/assets/9b326e77-cd67-42f6-a6c0-e800832ccd87)

#### Objetivo da Tela 

A tela de finalização de reserva tem como propósito: 

Exibir um resumo completo da seleção de quartos feita pelo usuário; 

Apresentar os valores detalhados, incluindo subtotal e total final; 

Conduzir o usuário de forma segura e clara à confirmação da reserva; 

Essa tela representa uma etapa decisiva na jornada do usuário e precisa transmitir segurança, transparência e objetividade. 

#### Princípios Gestálticos 

Proximidade: Informações agrupadas logicamente: quartos selecionados à esquerda, carrinho com valores à direita, e, abaixo dele, campos de login/cadastro (quando aplicável); 

Similaridade: Estilo visual uniforme para todos os cartões de quartos e campos de valor (uso de caixas com bordas, fontes consistentes e ícones padronizados); 

Continuidade: O usuário é guiado naturalmente da visualização do que selecionou (esquerda) para o resumo final e a ação de concluir (direita); 

Figura-fundo: Blocos visuais distintos (seleção de reserva, resumo de valores, login/cadastro) se destacam do fundo da tela, organizando visualmente o conteúdo; 

Fechamento: Cada seção tem sua própria estrutura visual bem delimitada, formando blocos fechados que facilitam a leitura e reduzem confusão. 

#### Regras de Ouro 

Consistência: Ícones, botões e rótulos seguem o padrão da identidade visual da aplicação; 

Atalhos: Usuários logados já veem a tela com seus dados preenchidos, podendo confirmar a reserva rapidamente; 

Redução da Carga de Memória: Todas as informações necessárias para tomar a decisão estão visíveis na tela, sem necessidade de mudar de página; 

Feedback informativo: O sistema exibe mensagens claras ao remover quartos, atualizar valores, ou ao clicar em “Reservar Agora”. 

#### Recomendações Ergonômicas 

Consistência: A disposição de elementos segue o padrão usado nas telas anteriores (botões, títulos, campos de entrada); 

Clareza: Informações organizadas em colunas separadas, com títulos, separadores e destaques para valores financeiros e botões; 

Prevenção e recuperação de erros: Campos obrigatórios, como login ou cadastro, são destacados se não forem preenchidos. O botão de confirmação só fica ativo quando os dados estiverem completos; 

Controle do usuário: Ele pode modificar sua seleção, adicionar ou excluir quartos e decidir o momento da reserva; 

Eficiência: O processo é direto: ver resumo → logar (se necessário) → clicar em “Reservar Agora”. 

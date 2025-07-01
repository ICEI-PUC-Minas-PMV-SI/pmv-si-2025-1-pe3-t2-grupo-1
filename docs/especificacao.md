# 3. DOCUMENTO DE ESPECIFICAÇÃO DE REQUISITOS DE SOFTWARE 


## 3.1 Objetivos deste documento 

Este documento tem como objetivo descrever e especificar as necessidades que devem ser atendidas pelo sistema de administração hoteleira, a experiência dos hóspedes e o trabalho da recepção. O sistema deve permitir um controle eficaz das reservas e da disponibilidade dos quartos, facilitando a organização da ocupação para os administradores. Além disso, deve oferecer uma interface intuitiva para a busca e atualização de informações, reduzindo erros e agilizando o atendimento da recepcionista. Para os hóspedes, é essencial que o processo de reserva seja simplificado, proporcionando uma experiência prática e acessível desde o primeiro contato com o hotel. 

 

## 3.2 Escopo do produto 


### 3.2.1 Nome do produto e seus componentes principais 

A aplicação web desenvolvida será denominada Hospedagem Simples, e seus componentes principais são: 

Módulo de cadastro de clientes e usuários: permite o gerenciamento de registro, atualização e consulta de informações dos hóspedes. Inclui controle de acesso e perfis (administrador, recepcionista e cliente); 

Módulo de administração: permite o cadastro – incluindo informações como tipo de quarto, características do quarto, valores e status do quarto (disponível, ocupado ou em manutenção) - e manutenção dos quartos. Além disso, permitirá o controle de disponibilidade para novas reservas e configurações gerais do sistema, como políticas de cancelamento e gerenciamento de usuários; 

Módulo de reserva: é o módulo central que comanda a interação dos usuários com o hotel. Assim, permite a interação dos clientes com os quartos cadastrados, podendo criar, alterar e cancelar reservas. Ainda, exibe os sistemas de filtragem e foto dos quartos. 

Módulo de pagamento: permite a confirmação das informações - como data, quarto e número de hóspedes - das reservas selecionadas, permite também a seleção da forma de pagamento e o redirecionamento para um sistema (VIA API) de gerenciamento de pagamento externo (Ex: Mercado Pago). 

 

### 3.2.2 Missão do produto 

O projeto tem como missão otimizar os processos oferecendo uma experiência mais prática e eficiente para os hóspedes, possibilitando ao usuário visualizar de forma rápida e direta as opções de quartos, preços e disponibilidade, finalizar e reservar sem dificuldade ou incertezas. 

 

### 3.2.3 Limites do produto 

O Hospedagem Simples não inclui recursos de avaliação ou feedback dos hóspedes. Além disso, o sistema não garante a disponibilidade contínua de todas as amenidades oferecidas pelo hotel durante todo o período da reserva, estando sujeito a eventuais mudanças ou limitações nas instalações e serviços. 

### 3.2.4 Benefícios do produto 

 ![image](https://github.com/user-attachments/assets/34b92d2d-4fa8-4200-8a8d-e5fdc56d8fd3)

![image](https://github.com/user-attachments/assets/228cbfc5-4ba6-4827-992d-251614b08649)



## 3.3 Descrição geral do produto 

 

### 3.3.1 Requisitos Funcionais 

 ![image](https://github.com/user-attachments/assets/73290944-c76e-43ec-80d2-704b0912c034)


 ![image](https://github.com/user-attachments/assets/9ddcdeeb-e2dc-4565-b47f-9c311c4484c8)


![image](https://github.com/user-attachments/assets/aacc8d7a-15c2-48a8-b113-7e698482c4eb)

 

### 3.3.1 Requisitos Não Funcionais 

 
![image](https://github.com/user-attachments/assets/c13c2d10-3060-4aca-a6de-33beabf7e9c0)



![image](https://github.com/user-attachments/assets/aeacdd16-c1bb-4b13-bbb0-f529872c065d)



### 3.3.2 Usuários  

 ![image](https://github.com/user-attachments/assets/b8660e1b-829e-40b6-a24e-b1e8151d97d5)


## 3.4 Modelagem do Sistema 

 

### 3.4.1 Diagrama de Casos de Uso 

Como observado no diagrama de casos de uso da Figura 1, o hóspede poderá gerenciar os dados pessoais, visualizar a disponibilidade de quartos e fazer reservas. O recepcionista poderá visualizar todas as reservas disponíveis, e o administrador, além dessas funções, poderá gerenciar todos os dados relacionados às reservas, informações de quartos e gestão de acessos. 

 
![image](https://github.com/user-attachments/assets/ccf6a084-f7ca-434b-8282-e808d9de077f)



Figura 1: Diagrama de Casos de Uso do Sistema. 

### 3.4.2 Descrições de Casos de Uso 

 

Cada caso de uso deve ter a sua descrição representada nesta seção. Exemplo: 

![image](https://github.com/user-attachments/assets/daea76ff-a708-43a9-a689-c7c38f520b9b)




![image](https://github.com/user-attachments/assets/e0424cb7-ce8a-42a9-92d6-c512770b0841)




![image](https://github.com/user-attachments/assets/b8adefc5-f6b3-460d-aed9-f3ebf203ad67)




![image](https://github.com/user-attachments/assets/aa5d9973-cc2c-4bf7-863f-dbe60a6f746f)




![image](https://github.com/user-attachments/assets/36d933db-422a-4179-8d19-2b0ee75be033)




![image](https://github.com/user-attachments/assets/8561d7ff-c0ca-441d-8b68-a03d83c0fee1)




![image](https://github.com/user-attachments/assets/7ef17311-556e-488b-87c2-c67b8885fa50)




![image](https://github.com/user-attachments/assets/c2f7b74f-8120-4323-ba80-3c7ddff8106b)




![image](https://github.com/user-attachments/assets/ecb462ef-a3f3-406d-96ae-011837c609b3)



![image](https://github.com/user-attachments/assets/062317c1-188c-44b7-92a1-05fb8e23247b)



![image](https://github.com/user-attachments/assets/3c544848-2c0d-431e-89af-4a6bd9335e79)



![image](https://github.com/user-attachments/assets/11d345dc-7951-48d2-9b69-066045a9deec)



![image](https://github.com/user-attachments/assets/bb7c558a-e232-4782-9ee9-536df5df327b)



![image](https://github.com/user-attachments/assets/22c4de51-db20-47bd-a377-78c03ea876aa)



![image](https://github.com/user-attachments/assets/4b819ae3-4e39-4ec2-96b4-3273453d8e47)


### 3.4.3 Diagrama de Classes  

A Figura 2 mostra o diagrama de classes do sistema de reservas. A Reserva deve conter a identificação do funcionário responsável pelo registro, bem como os dados do hóspede e do quarto reservado. Um quarto pode ter diversas reservas, mas pertence a apenas um tipo de quarto. Promoções podem ser aplicadas a diferentes reservas, e os preços podem variar de acordo com o período.


![image](https://github.com/user-attachments/assets/d5103cf1-4a2d-4c02-a6b3-6aa854709380)



Figura 2: Diagrama de Classes do Sistema. 

### 3.4.3 Descrições das Classes  

![image](https://github.com/user-attachments/assets/8e2a8cfb-e8f7-4c52-ae4c-ad0fc7d9f46a)




![image](https://github.com/user-attachments/assets/5caebdf9-7677-4628-9b80-d09c09b03da8)


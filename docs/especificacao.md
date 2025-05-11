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

 ![image](https://github.com/user-attachments/assets/cb9fc422-5b3a-4348-80b2-6d3f2cb2c3b9)


# 



 

 

3.3 Descrição geral do produto 

 

3.3.1 Requisitos Funcionais 

 ![image](https://github.com/user-attachments/assets/f6671453-505a-4220-a9d7-201e9519fb42)


 
![image](https://github.com/user-attachments/assets/26b0f6b8-514d-4ca7-9878-7fb47db7795f)



![image](https://github.com/user-attachments/assets/0e8b8571-9312-4cd8-a27d-fa96c3f8b955)



 

3.3.1 Requisitos Não Funcionais 

 
![image](https://github.com/user-attachments/assets/c253cc69-c777-4f30-b85a-46d20bc2e02c)


![image](https://github.com/user-attachments/assets/e0054303-ab47-44ff-bc11-42106282839a)




 

3.3.2 Usuários  

 ![image](https://github.com/user-attachments/assets/8e0c89ca-fd11-49ec-9449-01b55346c8a5)



![image](https://github.com/user-attachments/assets/a80c7d84-3722-4538-a9d8-7f069587feff)


 

3.4 Modelagem do Sistema 

 

3.4.1 Diagrama de Casos de Uso 

    Como observado no diagrama de casos de uso da Figura 1, o hóspede poderá gerenciar os dados pessoais, visualizar a disponibilidade de quartos e fazer reservas. O recepcionista poderá visualizar todas as reservas disponíveis, e o administrador, além dessas funções, poderá gerenciar todos os dados relacionados às reservas, informações de quartos e gestão de acessos. 

 

![image](https://github.com/user-attachments/assets/a115ac23-247a-40ff-902c-cef020bbd2f5)


Figura 1: Diagrama de Casos de Uso do Sistema. 

3.4.2 Descrições de Casos de Uso 

 

Cada caso de uso deve ter a sua descrição representada nesta seção. Exemplo: 

 ![image](https://github.com/user-attachments/assets/235c7a99-0b94-4edf-878a-f33d4c723780)



![image](https://github.com/user-attachments/assets/f5d40c1c-1952-491d-99ef-9acdce66a468)



![image](https://github.com/user-attachments/assets/ecea42e8-27a3-4e97-820c-90f39e96a1f4)



![image](https://github.com/user-attachments/assets/08469361-e87c-48de-932f-cd127c7d7521)



![image](https://github.com/user-attachments/assets/27c1875f-42d2-4b7f-94f2-c65b6ca39dd4)



![image](https://github.com/user-attachments/assets/6d813d50-9380-4894-bfbb-cb3a8f5ef989)



![image](https://github.com/user-attachments/assets/ff6505c8-875e-4268-857d-065ede19bb88)



![image](https://github.com/user-attachments/assets/097bb0ee-1fde-4916-8db1-5d9b9c2b552e)



![image](https://github.com/user-attachments/assets/d5b736d0-fd54-4e05-a4c7-17802ae81c36)



![image](https://github.com/user-attachments/assets/a4b377c2-49fb-455f-a400-4d44ff41e281)



3.4.3 Diagrama de Classes  

   A Figura 2 mostra o diagrama de classes do sistema de reservas. A Reserva deve conter a identificação do funcionário responsável pelo registro, bem como os dados do hóspede e do quarto reservado. Um quarto pode ter diversas reservas, mas pertence a apenas um tipo de quarto. Promoções podem ser aplicadas a diferentes reservas, e os preços podem variar de acordo com o período.


   ![image](https://github.com/user-attachments/assets/0c2fbcb9-1d9a-41f0-bdff-028cc8511f0d)


Figura 2: Diagrama de Classes do Sistema. 

3.4.3 Descrições das Classes  

![image](https://github.com/user-attachments/assets/70fa6ae1-16e7-454a-bc03-fc725db61722)



![image](https://github.com/user-attachments/assets/159c1fd9-ce5d-47d9-9a8a-fd9bddb2205f)

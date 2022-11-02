# Doguito_Oracle



Olá  galera, segue um  pouco do passo a passo do conhecimento adquirido com esse projeto da Oracle + Alura.


Os objetivos eram conhecer as características da OCI e aplicar esses conhecimentos na implantação o Doguito Pet Shop num ambiente de cloud.
Minha tarefa era realizar a conexão do Doguito com uma base de dados. Analisei as alternativas disponibilizadas pela OCI e optei pela utilização do banco de dados autônomos baseado em JSON, por sua simplicidade e facilidade de uso.




![image](https://user-images.githubusercontent.com/100032235/199371659-fdb4966a-e31b-4c91-bafe-fef25c5a563c.png)




-----------------------------------------------------------------------------------------------------------------------------------------------------------------
Estudei o funcionamento do Doguito para conectá-lo a esse banco de dados. Trata-se de uma aplicação NodeJS, escrita em JavaScript e que utiliza o framework ExpressJS, fornecendo uma API para acessar as funcionalidades do Doguito. Com base nesse conhecimento, implantei o Doguito na OCI e configurei sua conexão com o banco.




![image](https://user-images.githubusercontent.com/100032235/199372242-89b480a8-002f-43e8-a858-ced5c88dd13e.png)




-----------------------------------------------------------------------------------------------------------------------------------------------------------------
Entretanto, ao testar, notei que o Doguito não era iniciado automaticamente com a máquina virtual. Como solução, configurei a aplicação como um serviço do próprio sistema operacional.




![Screenshot_1](https://user-images.githubusercontent.com/100032235/199373495-8bd37718-2177-4d5d-9e95-3def99c535df.png)




-----------------------------------------------------------------------------------------------------------------------------------------------------------------
Em seguida, coloquei no load balancer e o acessamos pelo navegador, diretamente na API. Visto que era mais interessante implantar uma interface para navegar pelas funcionalidades, foi analisado as possibilidades de armazenamento e foi escolhido o object storage para servir o site estático de uma maneira bem simples. Houve, no entanto, um problema de comunicação com a API, porque o object storage roda em SSL por default, diferente do Doguito não estava utilizando o SSL. Por isso, configurei o SSL no load balancer.




![image](https://user-images.githubusercontent.com/100032235/199374023-092f1aff-7c10-4690-88fe-c45c3c4ae78a.png)



-----------------------------------------------------------------------------------------------------------------------------------------------------------------
Por fim, visando converter o Doguito para um modelo DevOps, mais moderno e avançado, foi utilizado a metodologia da infraestrutura como código. Comecei implantando uma estrutura básica de testes e, depois, ajustei os scripts do Terraform para que o Doguito se tornasse facilmente implantado e versionado, sem precisar realizar comandos manuais repetitivos. Basta subir a stack atualizada e a OCI implantará os componentes da maneira esperada.




![Screenshot_2](https://user-images.githubusercontent.com/100032235/199374168-470f971a-e9b7-41ec-9789-925b539e005a.png)



-----------------------------------------------------------------------------------------------------------------------------------------------------------------

Agora segue print dos serviços alocado  na oracle na conta free:


![image](https://user-images.githubusercontent.com/100032235/199374302-964384bb-d328-486f-950e-f829669377da.png)




-----------------------------------------------------------------------------------------------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/100032235/199374595-bded4395-8666-4116-8e68-a37f0127e44c.png)


-----------------------------------------------------------------------------------------------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/100032235/199375204-9b68b8ed-55ab-4304-b966-8c3439bdafec.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/100032235/199374680-a1e99d00-41e0-423a-af46-b3fa4d8cab26.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/100032235/199374727-9478b509-8faa-481c-9cb7-f57c31cf87b4.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/100032235/199374875-dc5ee23c-68e2-41d1-8938-aa9b10c6efab.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/100032235/199374926-23ced02e-937f-4c8f-bf0e-0f77b4277f23.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/100032235/199374996-00ceca0e-3c58-462d-9451-00f20a4bd7eb.png)



![image](https://user-images.githubusercontent.com/100032235/199375026-bcc04d72-2a1d-4316-9a0a-b197a732905e.png)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------




# Estarei deixando todos arquivos dísponivel.



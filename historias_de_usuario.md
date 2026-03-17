# Historias de usuário 
## Sistema de reserva de quadras de condomínio.

Funcionalidades: Agendamento de Quadras 
- **Como** morador do condomínio Cidade Jardins.
- **Eu quero** conseguir agendar uma quadra em horários específicos e checar sua disponibilidade.
- **Para** utilizar a quadra para eventos ou lazer.

Funcionalidades: Gerenciamento de Contas 
- **Como** Administrador do condomínio Cidade Jardins.
- **Eu quero** conseguir acessar o sistema e criar contas de moradores.
- **Para** os moradores conseguirem fazer as reservas.

1° Cenário: Reserva de Quadras <br>
História de Usuário:
- **Como** morador, eu quero agendar um horário em um campo esportivo.
  - **Dado** que estou logado e queira reservar uma quadra.
  - **E** o campo e horário desejados estão disponíveis.
  - **Quando** eu solicito a reserva no horario e quadra.
  - **Então** o sistema deve confirmar o agendamento e exibir uma mensagem de sucesso.

2° Cenário: Consulta de Agendamentos <br>
História de Usuário:
- **Como** morador, eu quero verificar meus agendamentos de quadra realizados.
  - **Dado** que possuo alguma reserva ativa.
  - **E** esteja logado no sistema com a minha conta.
  - **Quando** acesso a tela de "Meus Agendamentos".
  - **Então** o sistema deve listar todos os espaços, datas e horários reservados por mim.

3° Cenário: Cancelamento de Reserva <br>
História de Usuário:
- **Como** morador, eu quero cancelar um agendamento caso eu não possa comparecer.
  - **Dado** que possuo uma reserva de uma quadra.
  - **E** esteja logado no sistema
  - **Quando** seleciono a opção de cancelar.
  - **Então** o sistema deve remover a reserva, liberando o horário e me notificar do cancelamento.

4° Cenário: Gestão de Usuários como Administrador <br>
História de Usuário:
- **Como** administrador eu quero cadastrar moradores no sistema para que eles possam acessar a plataforma de reservas.
  - **Dado** que sou um administrador logado.
  - **E** tenho que criar uma conta para um morador.
  - **Quando** insiro os dados do morador e confirmo.
  - **Então** o sistema deve criar a conta no sistema para o morador.

5° Cenário: Acesso ao Sistema <br>
História de Usuário:
- **Como** morador ou administrador, eu quero realizar login para acessar as funcionalidades restritas do condomínio.
  - **Dado** que possuo uma conta previamente cadastrada.
  - **E** queire acessar o sistema.
  - **Quando** informo minhas credenciais válidas da conta.
  - **Então** o sistema deve permitir o acesso à área logada de morador ou administrador.

6° Cenário: Limite de Reservas por Morador <br>
História de Usuário:
- **Como** administrador, quero limitar o número de reservas ativas por morador.
  - **Dado** que o morador já possui o número máximo de reservas permitidas.
  - **E** ele tente agendar mais uma vez.
  - **Quando** ele solicitar um novo agendamento.
  - **Então** o sistema deve exibir uma mensagem informando que o limite foi atingido.

## Primeiro Caso: Agendamento de consulta
- ### Pré condição: 
**Paciente** já esteja logado e conectado à internet.
- ### Pós condição:
O **sistema** registra histórico das consultas já efetuadas.
- ### Fluxo principal:
1. **Paciente** abre a agenda.
2. O sistema busca no banco de dados os horários disponíveis e exibe para o usuário.
3. **Paciente** seleciona a data e horário desejado.
4. Sistema notifica a recepcionista sobre o novo agendamento.
5. Sistema reserva o horário no banco de dados.
6. **Recepcionista** confirma o horário solicitado.
7. Sistema notifica paciente que o agendamento foi confirmado.

- ### Fluxo alternativo de exceção:
1. **Paciente** abre a agenda.
2. O sistema busca no banco de dados os horários disponíveis e exibe para o paciente.
3. **Paciente** seleciona a data desejada.
4. Sistema informa indisponibilidade de horários na data e sugere uma nova data.

- ### Fluxo alternativo de exceção:
1. **Paciente** abre a agenda.
2. O sistema busca no banco de dados os horários disponíveis e exibe para o paciente.
3. **Paciente** seleciona a data desejada.
4. Sistema informa erro ao concluir o agendamento e solicita uma nova tentativa.

## Segundo Caso: Login
- ### Pré condição: 
Usuário já esteja cadastrado e conectado à internet.
- ### Pós condição:
Sistema verifica a veracidade dos dados fornecidos e libera o acesso.

- ### Fluxo principal:
1. **Usuário** preenche e-mail e senha.
2. O sistema verifica se e-mail e senha digitados conferem com os dados usados no cadastro.
3. Sistema libera acesso ao dashboard.

- ### Fluxo alternativo de exceção:
1. **Usuário** preenche e-mail e senha.
2. O sistema verifica se e-mail e senha digitados conferem com os dados usados no cadastro.
3. Sistema nega acesso e exibe mensagem informando e-mail e/ou senha incorretos.
4. **Usuário** tenta novamente 3 vezes sem sucesso.
5. Sistema bloqueia acesso temporariamente.

- ### Fluxo alternativo de exceção:
1. **Usuário** preenche e-mail e senha.
2. O sistema verifica se e-mail e senha digitados conferem com os dados usados no cadastro.
3. Sistema nega acesso e exibe mensagem informando e-mail e/ou senha incorretos.
4. **Usuário** tenta pela segunda vez, mas sem sucesso e seleciona a opção "Esqueci minha senha".
5. Usuário escolhe receber código de redefinição de senha via e-mail, mas não recebe o e-mail.

## Terceiro Caso: Consulta com o médico
- ### Pré condição: 
**Usuário** já tem agendamento feito e confirmado.
- ### Pós condição:
Sistema registra a consulta efetuada no histórico de atendimentos.

- ### Fluxo principal:
1. **Paciente** se identifica à recepcionista.
2. **Recepcionista** confirma presença do paciente no sistema.
3. **Paciente** é chamado pelo médico e tem sua consulta efetuada.
4. Após a consulta, **paciente** efetua o pagamento na recepção.

- ### Fluxo alternativo de sucesso:
1. **Paciente** se identifica à **recepcionista**.
2. **Recepcionista** informa que o **médico** teve um imprevisto e sugere consulta com um médico alternativo ou remarcar a consulta.
3. **Paciente** aceita a proposta e aguarda o médico substituto.

- ### Fluxo alternativo de exceção:
1. **Paciente** se identifica à **recepcionista**.
2. **Recepcionista** informa que a consulta precisou ser remarcada e o sistema não notificou o paciente.
- ### Fluxo alternativo de exceção:
1. **Paciente** se identifica à recepcionista.
2. **Recepcionista** confirma presença do paciente no sistema.
3. **Paciente** é chamado pelo médico e tem sua consulta efetuada.
4. Após a consulta, **paciente** solicita o resultado do exame feito na consulta.
5. **Recepcionista** informa que o sistema está indisponível e não está conseguindo buscar o resultado do exame.

**Stakeholders**: 

### Requisitos funcionais:
1. Para agendamento o sistema deve solicitar o nome e telefone de contato do paciente, a opção com o motivo do agendamento, a data e a hora escolhida.
2. O sistema deve consultar os horários disponíveis de acordo com o tempo exigido pelo motivo do agendamento e a disponibilidade do médico.
3. Paciente poderá agendar, cancelar, consultar os horários disponíveis e as solicitações de agendamento e seu status (pendente ou confirmada).
4. O sistema deverá contar o número de pacientes atendidos no dia.
5. A recepcionista poderá agendar, cancelar, remarcar e consultar a agenda com as solicitações de agendamentos e os que já estão confirmados.
6. O sistema deve solicitar aos administradores o procedimento feito e o valor cobrado no término do atendimento.
7. O sistema deverá calcular automaticamente a agenda do médico com base nas consultas agendadas.
8. O sistema deve notificar o médico e a recepcionista quando chegar alguma solicitação de agendamento.
9. O sistema deverá notificar o paciente após o agendamento for confirmado.
10. O sistema deve gerar um relatório mensal com o faturamento do consultório e estatística com o número de consultadas efetuadas e canceladas.

### Requisitos não funcionais:
1. Sistema deve funcionar 100% do tempo.
2. O tempo de resposta do sistema deverá ser de no máximo 3 segundos.
3. O sistema deverá ser multiplataforma (acesso por aplicativo no celular e online no computador).
4. O sistema deve solicitar e-mail e senha da recepcionista para efetuar o login.
5. O sistema deverá solicitar login do médico com e-mail e senha.
6. O sistema deve permitir acessos silmultâneos para controle da agenda pelo médico e recepcionista em tempo real.

### Regras de negócios:
1. O agendamento só pode ser confirmado pelos administradores (médico e recepcionista).
2. Somente os administradores terão acesso aos agendamentos feitos e solicitados por todos os pacientes.
3. O agendamento só deve ser solicitado e aprovado se o horário escolhido tiver disponível.
4. A recepcionista deve configurar opções com os motivos do agendamento (consulta de rotina, procedimento x, primeira consulta, etc) e o tempo que deverá ser reservado para cada opção.
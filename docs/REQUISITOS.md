### Stakeholders
● **Fábio (Paciente, 25 anos):**

> **Contexto:** Jovem, usa o celular para tudo. Trabalha em horário comercial.
> 
> **Dor:** "Odeio ter que ligar no meu horário de almoço e ficar na espera. Quero marcar
minha consulta às 22h, quando estou livre, e pelo celular."
> 
> **Necessidade:** Autoatendimento para agendar, cancelar e consultar horários 24/7.

● **Sandra (Recepcionista, 45 anos):**
> **Contexto:** Usa o "ClinicSys 1.0" há 10 anos. É ágil no sistema antigo, mas passa 80%
do dia ao telefone.
>
>**Dor:** "Não consigo fazer meu trabalho de faturamento porque o telefone não para.
Quando o paciente liga, tenho que conferir a agenda do médico no ClinicSys e falar
os horários vagos um por um. É muito lento.". 
>
> **Necessidade:** Reduzir o fluxo de ligações para focar em tarefas administrativas. Quer
que o novo sistema reserve o horário para o paciente, mas ela ainda quer aprovar a
consulta para evitar duplicidade e erros.

● **Dr. Marcos (Médico, 52 anos):**
> **Contexto:** Focado no atendimento. Sua agenda é gerenciada pela Sandra no
ClinicSys.
> 
> **Dor:** "Às vezes a Sandra me interrompe para confirmar um 'encaixe'. Gostaria de ter
minha agenda online para eu mesmo consultar do meu celular."
> 
> **Necessidade:** Visibilidade da sua própria agenda e menos interrupções.
### Requisitos funcionais:
1. Para agendamento o sistema deve solicitar o nome e telefone de contato do paciente, a opção com o motivo do agendamento, a data e a hora escolhida.
2. O sistema deve consultar os horários disponíveis de acordo com o tempo exigido pelo motivo do agendamento e a disponibilidade do médico.
3. Paciente poderá agendar, cancelar, consultar os horários disponíveis e as solicitações de agendamento e seu status (pendente ou confirmada).
4. O sistema deverá contar o número de pacientes atendidos no dia.
5. A recepcionista poderá agendar, cancelar, remarcar e consultar a agenda com as solicitações de agendamentos e os que já estão confirmados.
6. O sistema deve solicitar aos administradores o preenchimento dos procedimentos e/ou tipo de consulta realizado para registro do valor cobrado.
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
7. Sistema deve registrar o histórico dos pacientes

### Regras de negócios:
1. O agendamento só pode ser confirmado pelos administradores (médico e recepcionista).
2. Somente os administradores terão acesso aos agendamentos feitos e solicitados por todos os pacientes.
3. O agendamento só deve ser solicitado e aprovado se o horário escolhido tiver disponível.
4. A recepcionista deve configurar opções com os motivos do agendamento (consulta de rotina, procedimento x, primeira consulta, etc) e o tempo que deverá ser reservado para cada opção.
5. A recepcionista deve cadastrar o valor de cada procedimento e tipo de consulta.
6. Somente os administradores terão acesso ao histórico de todos os pacientes.
7. O paciente só poderá ter acesso ao próprio histórico.
# Documento de Escopo – Sistema de Agendamento de Consultas

## 1. Objetivo

Desenvolver um sistema de agendamento de consultas médicas com foco em otimizar tempo, espaço e organização, além de facilitar as buscas por informações, proporcionando maior eficiência no atendimento clínico.

---

## 2. Escopo

### 2.1. Escopo **IN** (Incluído no projeto)

- Cadastro de usuários (atendentes, médicos, gestores)
- Registro da disponibilidade de cada médico
- Cadastro de pacientes
- Agendamento de consultas
- Validação de conflitos de horário (exibição de erro em caso de choque de horários)

### 2.2. Escopo **OUT** (Fora do projeto)

- Agendamento remoto (feito pelo paciente em casa)
- Envio de mensagens para os médicos
- Notificações por SMS ou e-mail
- Prontuário eletrônico

---

## 3. Regras de Negócio

- Horários de consulta **não podem se sobrepor** a outros já agendados.
- Consultas **devem ocorrer apenas dentro da janela de atendimento** do profissional.
- O cancelamento de uma consulta **deve liberar o slot de horário imediatamente**.
- A duração padrão de cada consulta é de **30 minutos**.

---

## 4. Premissas

- O sistema funcionará apenas em **horário comercial**.
- O MVP será limitado a **uma única clínica**, com até **10 profissionais de saúde**.

---

## 5. Stakeholders

- **Atendentes** – responsáveis pelo agendamento e cadastro no sistema.
- **Médicos** – usuários com horários de atendimento definidos.
- **Pacientes** – destinatários dos serviços médicos.
- **Gestor da clínica** – responsável pela administração geral do sistema.

---

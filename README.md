# Barbearia App - Sistema Completo de Gestão e Agendamento

Sistema web completo para barbearia, que oferece funcionalidades para clientes e um painel administrativo para os gestores acompanharem o negócio.

---

## Funcionalidades

### Para Clientes

- Cadastro e autenticação (login/logout) com JWT
- Visualização de serviços e preços (guia de preços com cards)
- Agendamento de cortes e serviços adicionais (barba, sobrancelha, etc)
- Escolha de barbeiro e horários disponíveis
- Envio de formulário de contato ou sugestão
- Compra de planos/pacotes online via gateway de pagamento
- Visualização do histórico de agendamentos

### Para Administradores/Barbeiros

- Login seguro com permissões administrativas
- Gestão completa dos agendamentos (criar, editar, cancelar)
- Visualização de relatórios financeiros:
    - Lucro total por período
    - Taxa de clientes ativos
    - Serviços mais solicitados
    - Controle de pagamentos e planos ativos
- Gestão de barbeiros e seus horários
- Dashboard com métricas importantes para o negócio

---

## Tecnologias Utilizadas

| Camada          | Tecnologia                              |
|-----------------|-----------------------------------------|
| Back-end        | Java, Spring Boot, Spring Data JPA, JWT |
| Front-end       | Next.js, JavaScript                     |
| Banco de Dados  | MySQL                                   |
| Containerização | Docker                                  |
| Ferramentas     | Git, Insominia, Swagger                 |

---

## Estrutura do Projeto

```bash
/barbearia-app
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── services/
│   │   ├── entities/
│   │   ├── repositories/
│   │   └── config/
│   └── pom.xml
├── frontend/
│   └── pages/
│       ├── index.jsx
│       ├── login.jsx
│       ├── agendar.jsx
│       ├── sobre.jsx
│       ├── admin/              # telas exclusivas para o painel admin
│       │   ├── dashboard.jsx
│       │   ├── agendamentos.jsx
│       │   └── relatorios.jsx
├── docker-compose.yml
└── README.md

# **SIGDHA – Sistema Inteligente de Gestão e Divulgação de Horários Acadêmicos**

**📅 Versão:** 1.0
**🏢 Instituição:** FATEC
**📌 Status:** MVP em desenvolvimento

---

## **🎯 Objetivo**
O **SIGDHA** é uma **plataforma web centralizada** desenvolvida para **automatizar e otimizar** a gestão, atualização em tempo real e divulgação de horários acadêmicos, substituindo processos manuais (como edição de apresentações, geração de vídeos e publicação no YouTube).
O sistema permite:
✅ **Centralização** de cursos, turmas, disciplinas, professores, salas e horários.
✅ **Automatização** da divulgação em painéis digitais, TVs e portais para alunos/professores.
✅ **Alterações emergenciais** (troca de sala, ausência de professor, cancelamento de aula) com reflexo imediato em todos os canais.
✅ **Rastreabilidade** de todas as alterações, com histórico e auditoria.
✅ **Inteligência** para otimização de salas, detecção de conflitos e geração de relatórios.

---

## **📂 Estrutura do Projeto**
O projeto está organizado em módulos claros e escaláveis, seguindo boas práticas de desenvolvimento:
- **Backend:** PHP 8.x + PDO (MySQL/MariaDB)
- **Frontend:** Bootstrap 5, HTML5, CSS3, JavaScript
- **Automatização:** Cron Jobs (Windows Task Scheduler)
- **Versionamento:** GitHub
- **Deploy:** XAMPP (local) e servidor web (produção)

**Estrutura de pastas:**
```text
grade-horaria/
├── config/          # Configurações de BD e permissões
├── auth/            # Autenticação e sessão
├── usuarios/        # Gerenciamento de usuários
├── cursos/          # Cadastro de cursos
├── disciplinas/     # Cadastro de disciplinas
├── professores/     # Cadastro de professores
├── salas/           # Cadastro e bloqueio de salas
├── grades/          # Montagem e visualização de grades
├── faltas/          # Registro e relatórios de faltas
├── painel/          # Interface para TVs e painéis digitais
├── dashboard/       # Dashboards para diretoria e coordenação
├── relatorios/      # Relatórios administrativos
├── cron/            # Scripts de automação
└── includes/        # Componentes reutilizáveis
```

---

## **🚀 Funcionalidades Principais (MVP)**
### **🔐 Autenticação e Controle de Acesso**
- Login com email e senha (bcrypt)
- RBAC (Role-Based Access Control)
- Sessão ativa e bloqueio de URLs restritas
- Gerenciamento de usuários por papéis (Administrador, System Manager, Secretaria, Coordenação, Diretoria, Alunos)

### **📝 Cadastros Fundamentais**
- Cursos, disciplinas, professores, salas, períodos letivos
- Validação de conflitos (professor, sala, turma)

### **📅 Gestão de Grades Horárias**
- Montagem de grade por curso, dia e período
- Alterações temporárias (troca de sala, cancelamento)
- Bloqueio de salas para eventos ou manutenção

### **📊 Controle de Ausências e Ocorrências**
- Registro de faltas de professores
- Vinculação de substituições
- Geração de relatórios em PDF
- Dashboard de ausências (presentes/faltantes por período)

### **⚡ Processamento Automático**
- Cron job a cada 10 minutos para atualização em tempo real
- Atualização automática de painéis digitais e portais
- Modo TV otimizado para exibição em televisores

### **📱 Visualização e Acesso**
- Layout responsivo (desktop, mobile, tablets)
- Cores distintas por curso para identificação rápida
- Modos de exibição: grade completa, próximas aulas, modo rotativo

### **📈 Relatórios e Dashboards**
- Relatório de faltas por disciplina/professor
- Indicadores operacionais (aulas, salas ocupadas/disponíveis)
- Exportação de dados para processamento externo

### **🔔 Mensagens e Notificações**
- Programação de mensagens do dia
- Avisos sobre cancelamentos ou eventos
- Histórico de mensagens preservado

---

## **🛠 Tecnologias Utilizadas**
| **Área**       | **Tecnologias**                          |
|----------------|-----------------------------------------|
| **Backend**    | PHP 8.x, PDO, MySQL/MariaDB              |
| **Frontend**   | Bootstrap 5, HTML5, CSS3, JavaScript     |
| **Automação**  | Cron Jobs (Windows Task Scheduler)      |
| **Versionamento** | GitHub                                |
| **Deploy**     | XAMPP (local), Servidor Web (produção)  |

---

## **📅 Cronograma (Fase 1 – MVP)**
| **Etapa**                          | **Duração**  | **Status**          |
|------------------------------------|-------------|--------------------|
| Levantamento de requisitos          | 1 semana     | ✅ Concluído       |
| Desenho do DER detalhado           | 3 dias       | ⏳ Em andamento     |
| Criação do script SQL de BD         | 5 dias       | ⏳ Pendente         |
| Implementação dos módulos básicos   | 3 semanas    | ⏳ Pendente         |
| Desenvolvimento da gestão de grades| 2 semanas    | ⏳ Pendente         |
| Implementação do controle de faltas| 1 semana     | ⏳ Pendente         |
| Configuração do cron job            | 3 dias       | ⏳ Pendente         |
| Testes de usabilidade               | 1 semana     | ⏳ Pendente         |
| Deploy no domínio                   | 2 dias       | ⏳ Pendente         |

**📌 Total estimado para o MVP:** ~280 horas

---

## **💡 Como Contribuir**
1. **Fork** o repositório
2. Crie uma **branch** para sua feature (`git checkout -b feature/nova-feature`)
3. **Commit** suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. **Push** para a branch (`git push origin feature/nova-feature`)
5. Abra um **Pull Request**

---
**💬 Feedback e sugestões são bem-vindos!** 🚀

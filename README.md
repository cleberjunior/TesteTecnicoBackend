# 💻 Teste Técnico – Desenvolvedor(a) Java Backend Pleno/Sênior

## 📌Objetivo:

Criar uma API RESTful para um sistema de agendamento de consultas médicas, com controle de disponibilidade, autenticação, e regras de negócio.

---

## 🛠 Tecnologias:

- **[Java 17](https://www.oracle.com/java)**
- **[Spring Boot](https://spring.io/projects/spring-boot)**
- **[Spring Security JWT](https://spring.io/projects/spring-boot)**
- **[JPA (Hibernate)](https://spring.io/projects/spring-boot)**
- **[PostgreSQL](https://www.postgresql.org)**
- **[Lombok](https://projectlombok.org)**
- **[Maven](https://maven.apache.org)**

---

## ⚙️ Funcionalidades obrigatórias:

### 1. Cadastro e Autenticação

- Cadastro de usuários com dois perfis: PACIENTE e MEDICO
- Login com autenticação via JWT

### 2. Agendamento

- Pacientes podem agendar consultas com médicos
- Só é possível agendar se o médico estiver disponível no horário informado
- Não pode haver conflitos de horário para o médico
- Consultas duram 1 hora

### 3. Cancelamento

- Consultas podem ser canceladas com no mínimo 24h de antecedência
- Cancelamentos devem ser registrados com o motivo

### 4. Relatórios

- Listagem de consultas futuras de um médico
- Listagem de consultas de um paciente (passadas e futuras)
- Relatório simples: médicos com mais agendamentos no mês

---

## 📄 Regras de negócio importantes:

- Horário de atendimento dos médicos: 08h–18h (segunda a sexta)
- Não deve permitir agendamento fora desse horário ou em fins de semana
- Um paciente só pode ter uma consulta por dia

---

## 📄 Extras desejáveis (Bônus):

- Testes automatizados (unitários e integração)
- Docker (Dockerfile e/ou docker-compose com banco)
- Documentação com Swagger/OpenAPI
- Cache com Redis para relatórios ou dados de consulta
- Versionamento de API (v1, v2 etc.)
- CI/CD (GitHub Actions ou outro)

---


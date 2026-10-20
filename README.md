# 🏦 Simulador de Sistema Bancário em Java

Aplicação desenvolvida em Java 21 para simulação de operações bancárias, desenhada com foco em **Programação Orientada a Objetos (POO)**, **Clean Architecture** e **Desacoplamento de Camadas**.

---

## 🎯 Objetivo do Projeto

Demostrar a aplicação prática de padrões de arquitetura de software e boas práticas de desenvolvimento em Java, tais como:

- **Clean Architecture & Separação de Responsabilidades:** Separação clara entre domínio, casos de uso e infraestrutura.
- **Padrões de Projeto (Repository Pattern):** Utilização de interface (`ITransacaoRepository`) para isolar a persistência de dados das regras de negócio.
- **Princípios de POO:** Encapsulamento, Herança e Polimorfismo na modelagem de diferentes tipos de conta (`ContaCorrente` e `ContaPoupanca`).
- **Testabilidade & Desacoplamento:** Implementação de repositório em memória (`TransacaoRepositoryInMemory`), permitindo a evolução futura para bases de dados relacionais (ex: PostgreSQL/MySQL) sem impactar as regras de negócio.

---

## 🏗️ Estrutura e Arquitetura do Projeto

O projeto foi organizado segundo os princípios de camadas legíveis e mantCursor:

```text
src
└── main.com.contabancaria
    ├── application          # Ponto de entrada da aplicação e interface CLI
    │   ├── Aplicacao.java
    │   └── Main2.java
    ├── entities             # Domínio: Entidades principais e interfaces de contrato
    │   ├── Cliente.java
    │   ├── Conta.java
    │   ├── ContaCorrente.java
    │   ├── ContaPoupanca.java
    │   ├── Transacao.java
    │   └── ITransacaoRepository.java
    ├── usecases             # Regras de negócio e orquestração de transações
    │   └── TransacaoService.java
    └── infrastructure       # Implementação técnica de dados (In-Memory)
        └── TransacaoRepositoryInMemory.java
```

## Tecnologias utilizadas

- Java 21
- IntelliJ IDEA
- Conceitos: Clean Architecture, POO, Injeção de Dependências/Interfaces, Repository Pattern.


Feito com 💻 e ☕ por Gustavo Alves

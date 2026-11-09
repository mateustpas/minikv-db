# MiniKV — Banco de Dados Concorrente

Projeto sendo desenvolvido como trabalho final da disciplina de Programação Concorrente, cujo objetivo consiste em paralelizar o banco de dados MiniKV, originalmente implementado em C, utilizando a biblioteca Pthreads. A implementação busca permitir o acesso concorrente às estruturas do banco, assegurando a integridade dos dados durante a execução simultânea de transações a partir de um código entregue do professor.

---

# !DISCLAIMER!

A maioria do código implementado não é de autoria dos contribuidores,e sim entrega dos professores. Reflete nosso trabalho os trechos identificados com comentários assinados.

---

## Objetivos de Aprendizado

- Compreender e aplicar conceitos de programação concorrente em uma aplicação previamente desenvolvida.
- Conhecer e utilizar a biblioteca Pthreads para criação e gerenciamento de threads.
- Identificar e tratar condições de corrida (Race Conditions) durante operações simultâneas.
- Garantir a integridade e a consistência dos dados em cenários de acesso concorrente.
- Compreender os desafios de sincronização e compartilhamento de recursos em sistemas multithread.

---

## Padrões Arquiteturais Aplicados

- Concorrência: Paralelização das operações do MiniKV por meio da execução de múltiplas threads.
- Sincronização: Utilização dos mecanismos de sincronização disponibilizados pela biblioteca Pthreads para controlar o acesso simultâneo aos recursos compartilhados.
- Integridade de Dados: Tratamento de operações concorrentes para assegurar que transações não comprometam a consistência das informações armazenadas.
- Exclusão Mútua: Controle de acesso às regiões críticas da aplicação, evitando interferências entre operações executadas simultaneamente.

---

## Tecnologias Utilizadas

- Linguagem: C
- Biblioteca: POSIX Threads (Pthreads)
- Concorrência: Threads, sincronização e exclusão mútua.
- Projeto Base: MiniKV (banco de dados desenvolvido em C).

---

## Mecânicas do Sistema

- Execução Concorrente: Permite a execução de múltiplas operações por diferentes threads.
- Sincronização de Acesso: Controle das operações sobre estruturas compartilhadas para evitar condições de corrida.
- Integridade das Transações: Tratamento de acessos simultâneos para preservar a consistência dos valores armazenados.
- Gerenciamento de Threads: Criação, execução e sincronização das threads responsáveis pelo processamento das operações.

---

## Desenvolvimento e Implementações

- Paralelização da estrutura original do MiniKV, introduzindo mecanismos de concorrência para permitir o processamento simultâneo de operações. As principais preocupações durante o desenvolvimento englobam:

- Pthreads: Biblioteca utilizada para criação, gerenciamento e sincronização das threads.
- Sincronização: Implementação de mecanismos para controlar o acesso concorrente às estruturas compartilhadas.
- Regiões Críticas: Identificação e proteção de trechos de código que manipulam recursos compartilhados.
- Integridade das Transações: Tratamento de operações simultâneas para evitar inconsistências nos dados armazenados.

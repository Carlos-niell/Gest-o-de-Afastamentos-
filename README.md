# 📊 Gestão de Afastamentos

> **Status do Projeto:** 🚀 Concluído (Ambiente de Estudo/Aprimoramento técnico)

O **Gestão de Afastamentos** é uma aplicação web moderna e responsiva voltada para o setor de Recursos Humanos e lideranças corporativas. O objetivo principal do sistema é centralizar, automatizar e gerenciar com precisão todo o ciclo de vida das solicitações de afastamento de colaboradores, desde a abertura do pedido até a aprovação final e notificação.

Este projeto foi desenvolvido utilizando a plataforma low-code **Oracle APEX** (versão 26.1), aproveitando ao máximo recursos nativos avançados como mecanismos de **Workflow**, **Task Definitions** (Definições de Tarefa de Aprovação) e integrações via Web Services (REST).

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **Plataforma:** [Oracle APEX 26.1](https://apex.oracle.com/) (Compatibilidade de Modo 24.2)
- **Banco de Dados:** Oracle Database
- **Linguagens Procedimentais:** SQL e PL/SQL (Tratamento de dados, automações corporativas e regras de negócio)
- **Componentes Avançados:** APEX Workflow Engine, Task Definitions (Approval Type)
- **Arquitetura de Consumo:** Web Source Modules (Integração REST com APIs externas de Dados Abertos para carga de servidores e estagiários)
- **Recursos de Interface:** Progressive Web Application (PWA) habilitado com notificações Push configuradas

---

## 💡 Principais Funcionalidades

### 👥 Módulos Gerais e Páginas da Aplicação
A aplicação é composta por **21 páginas** dinâmicas estruturadas para diferentes perfis de acesso:
- **Home (Dashboard):** Visão macro e amigável para acompanhamento rápido.
- **Formulário de Solicitação de Afastamento:** Interface simples e intuitiva para o colaborador registrar o tipo de afastamento, data de início e término.
- **Minhas Tarefas (Painel de Autorização):** Caixa de entrada centralizada para gestores e chefias analisarem, aprovarem ou rejeitarem pendências.
- **Acompanhamento do Servidor (Solicitações Salvas):** Relatório analítico interativo para o colaborador verificar o histórico de suas demandas e status em tempo real.
- **Listas de Servidores e Estagiários:** Telas de consulta alimentadas em tempo real por Web Services externos.
- **Módulo de Administração:** Controle de acessos e configurações globais do sistema.

---

## ⚙️ Arquitetura e Engenharia de Automação

O grande diferencial técnico deste projeto está na implementação da lógica server-side e na orquestração de processos baseados no estado do negócio.

### 🔄 Fluxo de Processo (APEX Workflow & Approval Tasks)
A lógica de aprovação foi desacoplada das páginas e implementada de forma nativa através do **APEX Workflow Engine**. O modelo segue o seguinte fluxo automatizado:

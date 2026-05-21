# 🏥 OmniCare HIS — Hospital Information System

[cite_start]Este repositório contém uma aplicação web completa desenvolvida em **Python** com **Streamlit** e **SQLite3** para a gestão e auditoria de faturamento hospitalar[cite: 1, 3]. [cite_start]O projeto foi construído com base nos requisitos do **Problema 04** da unidade curricular de **Programação Biomédica (Informática em Saúde)**[cite: 1, 2].

## 📊 Estrutura do Modelo de Dados (MER)
[cite_start]A aplicação implementa rigorosamente o modelo relacional proposto pela Engenharia de Dados, cobrindo as seguintes entidades[cite: 4, 5]:
- [cite_start]**Pacientes**: Controlo cadastral e dados biométricos (CPF, Sexo, Peso, Altura, Data de Nascimento)[cite: 5].
- [cite_start]**Atendimentos**: Registos de episódios de urgência integrados ao Protocolo de Triagem de Manchester e CID10[cite: 5, 38].
- [cite_start]**Serviços**: Lançamento de procedimentos realizados vinculados à tabela de honorários comerciais[cite: 5, 39].
- [cite_start]**TUSS & CID10**: Tabelas de referência para codificação de procedimentos e diagnósticos[cite: 5].

## 🚀 Funcionalidades Implementadas
[cite_start]O sistema disponibiliza painéis interativos para responder às seguintes consultas de negócio[cite: 43]:
1. [cite_start]💰 **Valor Total de um Atendimento Específico**: Cálculo consolidado com comandos de agrupamento (`GROUP BY`) e soma agregada[cite: 44].
2. [cite_start]👤 **Histórico Financeiro por Paciente**: Totalização de consultas e exames realizados por utente[cite: 45].
3. [cite_start]🔍 **Mecanismo de Busca por Código TUSS**: Rastreabilidade de procedimentos agrupados por atendimento e paciente[cite: 46].
4. [cite_start]📅 **Monitorização Epidemiológica por Data**: Distribuição de serviços prestados segmentados por género e código TUSS[cite: 47].
5. [cite_start]🔒 **Auditoria de Integridade Referencial**: Simulação de travas rígidas de chaves estrangeiras (`ON DELETE RESTRICT`)[cite: 40, 41, 42].

## 🛠️ Como Executar o Projeto Localmente

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/SEU_USUARIO/omnicare-his.git](https://github.com/SEU_USUARIO/omnicare-his.git)
   cd omnicare-his

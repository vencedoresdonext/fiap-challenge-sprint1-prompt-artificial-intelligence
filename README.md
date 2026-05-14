# ChatBot GoodWe - Sprint 1 - 2026

## Integrantes

| Nome | RM |
|---|---|
| Natan Silva da Costa | 573100 |
| Leonardo Scotti Tobias | 573305 |
| Luca Almeida Lucareli | 569061 |
| Henrique Almeida Lucareli | 569183 |
| Enzo Seiji Delgado Tabuchi | 573156 |

---

# Problema

O desafio proposto pela GoodWe no EV Challenge 2026 consiste na criação de sistemas inteligentes integrados capazes de:

- Gerenciar a distribuição de potência elétrica;
- Controlar múltiplos carregadores;
- Realizar faturamento;
- Comunicar dados em tempo real.

Dessa forma, o projeto busca unir eficiência energética, automação e inteligência artificial para melhorar o gerenciamento de ambientes com carregamento de veículos elétricos.

---

# Proposta do Chatbot

O **ChatBot GoodWe** foi desenvolvido como uma ferramenta de apoio operacional, tendo como principais objetivos:

- Explicar o funcionamento do sistema energético;
- Auxiliar na tomada de decisão;
- Simular a distribuição de energia;
- Responder dúvidas técnicas relacionadas ao projeto.

## Persona escolhida
### Operador técnico/comercial

### Justificativa
Esse perfil de usuário precisa tomar decisões rápidas relacionadas à energia, carga e distribuição elétrica. Portanto, torna-se o principal beneficiado por um chatbot técnico e inteligente, capaz de fornecer suporte rápido e contextualizado.

---

# EV Challeng

A proposta armazenada no EV Challeng consiste em uma IA capaz de analisar informações do ambiente onde o sistema foi instalado/localizado e, com base nesses dados, informar o rendimento energético e possíveis riscos existentes no ambiente.

A solução faz ainda mais sentido quando integrada a um sistema inteligente responsável por captar a energia do local e gerar relatórios detalhados para o time da GoodWe por meio da IA, proporcionando maior controle, automação e eficiência operacional.

---

# Tecnologias Utilizadas

- OpenAI API (gpt-4.0-mini)
- Python
- Integração via biblioteca de IA generativa
- Biblioteca para cálculo de horário de pico

## Justificativa Técnica

As tecnologias foram escolhidas devido aos seguintes fatores:

- Alta velocidade;
- Boa compreensão de contexto técnico;
- Facilidade de integração;
- Baixo custo para testes.

---

# Fluxo do Chatbot

1. O usuário realiza uma pergunta;
2. A pergunta é enviada ao sistema;
3. O modelo de IA processa a solicitação com base no prompt definido;
4. A IA gera uma resposta contextualizada;
5. A resposta é exibida ao usuário.

---

# Fluxo do EV Challeng

1. O usuário informa os dados solicitados;
2. As funções analisam possíveis riscos de sobrecarga;
3. O sistema verifica os horários para evitar períodos de pico;
4. A IA gera um relatório final com as análises realizadas.

---

# Modelo de Teste - ChatBot

### 1. A GoodWe é uma empresa de quê?  
**Resposta:** Soluções sustentáveis.

### 2. Qual o desafio do projeto?  
**Resposta:** Gerenciar e distribuir energia entre carregadores.

### 3. Como otimizar o projeto?  
**Resposta:** Organização e divisão de tarefas.

### 4. O que o projeto deve ter?  
**Resposta:** Informações, regras e suporte inteligente.

### 5. Como organizar oferta e demanda de energia?  
**Resposta:** Distribuir energia entre veículos respeitando limites e prioridades.

---

# Prompt Utilizado — CHATBOT

## System Prompt

Você é um especialista em sistemas energéticos e analista de produtos da empresa GoodWe, focada em soluções de energia limpa e infraestrutura para carregamento de veículos elétricos.

## Objetivo

Projetar, explicar e otimizar um sistema inteligente de gerenciamento de energia para carregadores de veículos elétricos em estabelecimentos comerciais.

## Contexto do Sistema

A GoodWe desenvolve soluções que integram geração de energia solar com consumo inteligente, visando:

- Eficiência energética;
- Redução de custos;
- Sustentabilidade.

O sistema deve gerenciar a distribuição de energia elétrica disponível entre múltiplos carregadores de veículos elétricos, respeitando as limitações da infraestrutura elétrica existente.

## Requisitos do Sistema

O sistema deve:

- Distribuir energia de forma inteligente entre os carregadores;
- Evitar sobrecarga da rede elétrica do estabelecimento;
- Minimizar custos com upgrades de infraestrutura elétrica;
- Integrar, quando disponível, geração local de energia (ex: solar).

## Variáveis Dinâmicas

O sistema deve considerar:

- Consumo total do estabelecimento em tempo real;
- Capacidade máxima contratada da rede elétrica;
- Quantidade de veículos conectados;
- Nível de carga (bateria) de cada veículo;
- Prioridade de carregamento (VIP, emergência, tempo de permanência);
- Horário do dia (pico vs fora de pico);
- Geração local de energia (se houver).

## Estratégia de Distribuição de Potência

- O primeiro veículo conectado recebe uma potência base inicial;
- Conforme novos veículos se conectam, a potência é redistribuída entre todos;
- O sistema ajusta automaticamente a potência de cada carregador em tempo real.

## Regras de Controle

- Nunca exceder a capacidade máxima contratada;
- Priorizar a estabilidade da rede elétrica;
- Reduzir potência em horários de pico;
- Aumentar potência quando houver sobra de energia;
- Considerar prioridade dos usuários na redistribuição.

## Comportamento Esperado da IA

- Responder perguntas técnicas sobre o sistema;
- Propor algoritmos e lógica de controle (pseudocódigo ou Python);
- Explicar decisões de forma clara e objetiva;
- Evitar depender de informações externas ou buscas na internet;
- Sugerir melhorias e otimizações.

## Estilo de Resposta

- Ser técnico e direto;
- Utilizar exemplos práticos quando necessário;
- Estruturar respostas com lógica clara (passo a passo, fórmulas ou código).

## Contexto Adicional da GoodWe

A GoodWe é uma empresa focada em soluções de energia solar e eficiência energética, oferecendo sistemas seguros, eficientes e de fácil instalação para residências e comércios, permitindo redução de custos e melhor aproveitamento da energia limpa.

---

# System Prompt — EV CHALLENG

Você é um especialista em sistemas energéticos e analista de produtos da empresa GoodWe, focada em soluções de energia limpa e infraestrutura para carregamento de veículos elétricos.

Seu objetivo é auxiliar no controle inteligente de energia de um ambiente comercial com múltiplos carregadores de veículos elétricos.

O sistema deve:
- Distribuir energia de forma inteligente;
- Evitar sobrecarga da rede elétrica;
- Priorizar estabilidade energética;
- Integrar energia solar quando disponível;
- Redistribuir potência dinamicamente;
- Explicar decisões técnicas;
- Sugerir otimizações.

## Variáveis importantes

- Consumo atual do estabelecimento;
- Capacidade máxima da rede;
- Quantidade de veículos;
- Potência disponível;
- Horário de pico;
- Energia solar disponível;
- Prioridade de carregamento.

As respostas devem ser técnicas, objetivas e claras.

---

# Considerações Finais

O projeto demonstra a aplicação da IA generativa em um cenário real de energia sustentável, evidenciando como a tecnologia pode contribuir para automação, eficiência energética e suporte operacional.

## Benefícios

- Melhor entendimento do sistema;
- Apoio técnico;
- Auxílio na tomada de decisão.

Além disso, o projeto analisa como a utilização da IA pode contribuir diretamente para os relatórios do sistema inteligente solicitado pela GoodWe, trazendo automação, praticidade, conforto ao usuário e um importante diferencial sistêmico para a solução proposta.

---

# Fluxograma

![Fluxograma](fluxograma.png)

---

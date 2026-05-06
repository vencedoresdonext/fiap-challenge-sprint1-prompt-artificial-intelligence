## Integrantes:

- Natan Silva da Costa — RM: 573100  
- Leonardo Scotti Tobias — RM: 573305  
- Luca Almeida Lucareli — RM: 569061  
- Henrique Almeida Lucareli — RM: 569183  
- Enzo Seiji Delgado Tabuchi — RM: 573156  

---

## Projeto - ChatBot GoodWe

O chatbot foi desenvolvido para centralizar e organizar informações essenciais do projeto, permitindo que a equipe tire dúvidas de forma rápida, clara e eficiente.

Ele atua como um assistente inteligente, auxiliando no entendimento das regras e funcionamento do sistema de carregamento de veículos elétricos.

---

### Explicação Detalhada do Código e Variáveis

Este código implementa um chatbot utilizando a API do Google Gemini, configurado para atuar como um analista de produtos da GoodWe, respondendo perguntas com base em um contexto técnico pré-definido.

---

## Escolha da LLM

Foi escolhido o gemini-2.5-flash pela facilidade de integrar o sistema de perguntas e respostas, além de ser acessivel a testes sua chave de API.

## Perguntas

1. A goodwe é uma empresa de que?
Resposta esperada: De soluções sustentaveis

2. Qual o desafio que realizaremos?
Resposta esperada: Definição do desafio abordado anteriormente.

3. Como otimizaremos as etapas do projeto?
Resposta esperada: Organização, controle e separação em equipes.

4. Fale o que o projeto deve ter.
Resposta esperada: Informações das etapas do projeto.

5. Como organizar a oferta e demanda de potencia eletrica do comercio?
Resposta esperada: Formas de otimizar o sistema do comercio.

## Prompt

Você é um especialista em sistemas energéticos e analista de produtos da empresa GoodWe, focada em soluções de energia limpa e infraestrutura para carregamento de veículos elétricos.

Seu objetivo é projetar, explicar e otimizar um sistema inteligente de gerenciamento de energia para carregadores de veículos elétricos em estabelecimentos comerciais.

Contexto do sistema
A GoodWe desenvolve soluções que integram geração de energia solar com consumo inteligente, visando eficiência energética, redução de custos e sustentabilidade.

O sistema deve gerenciar a distribuição de energia elétrica disponível entre múltiplos carregadores de veículos elétricos, respeitando as limitações da infraestrutura elétrica existente.

Requisitos do sistema
O sistema deve:

1. Distribuir energia de forma inteligente entre os carregadores
2. Evitar sobrecarga da rede elétrica do estabelecimento
3. Minimizar custos com upgrades de infraestrutura elétrica
4. Integrar, quando disponível, geração local de energia (ex: solar)

Variáveis que devem ser consideradas (dinamicamente)
- Consumo total do estabelecimento em tempo real
- Capacidade máxima contratada da rede elétrica
- Quantidade de veículos conectados
- Nível de carga (bateria) de cada veículo
- Prioridade de carregamento (ex: cliente VIP, emergência, tempo de permanência)
- Horário do dia (pico vs fora de pico)
- Geração local de energia (se houver)

Estratégia de distribuição de potência
- O primeiro veículo conectado recebe uma potência base inicial
- Conforme novos veículos se conectam, a potência total disponível é redistribuída entre todos
- O sistema deve ajustar automaticamente a potência de cada carregador em tempo real

Regras de controle
- Nunca exceder a capacidade máxima contratada
- Priorizar estabilidade da rede elétrica
- Reduzir potência em horários de pico
- Aumentar potência quando houver sobra de energia
- Considerar prioridade dos usuários na redistribuição

Comportamento esperado da IA
- Responder perguntas técnicas sobre o sistema
- Propor algoritmos e lógica de controle (preferencialmente em pseudocódigo ou Python)
- Explicar decisões de forma clara e objetiva
- Evitar depender de informações externas ou buscas na internet
- Sugerir melhorias e otimizações quando relevante

Estilo de resposta
- Seja técnico e direto
- Use exemplos práticos quando necessário
- Estruture respostas com lógica clara (passo a passo, fórmulas ou código)

Contexto adicional da GoodWe
A GoodWe é uma empresa focada em soluções de energia solar e eficiência energética, oferecendo sistemas seguros, eficientes e de fácil instalação para residências e comércios, permitindo redução de custos e melhor aproveitamento da energia limpa.

---

## 💡 Considerações Finais

Este projeto demonstra, de forma prática, a aplicação de **Inteligência Artificial Generativa** no suporte a soluções de **energia sustentável**, especialmente no contexto de carregamento inteligente de veículos elétricos.

Além de facilitar o acesso à informação para a equipe, o chatbot contribui para:

- Melhor compreensão das regras do sistema  
- Apoio na tomada de decisões técnicas  
- Organização e padronização das informações do projeto  

Como evolução futura, o projeto pode incluir:

- Interface gráfica (web ou mobile)  
- Integração com dados reais de consumo energético  
- Sistema de priorização mais avançado com machine learning  
- Monitoramento em tempo real dos carregadores  

Dessa forma, o Chatbot GoodWe se torna não apenas uma ferramenta de apoio, mas também uma base sólida para soluções mais completas e escaláveis no setor de energia.

---

## Fluxograma

![Fluxograma do Projeto](fluxograma.png)

---

# Case Técnico — Nola | Chatbot com IA para Customer Success

## Sobre o projeto

Este projeto foi desenvolvido como solução para o case técnico da Nola, com o objetivo de criar um chatbot funcional utilizando automação e Inteligência Artificial para apoiar operações de Customer Success.

A solução foi construída utilizando o N8N como ferramenta principal de automação, integrado ao Google Sheets como base de conhecimento e à API da Groq para geração de respostas com IA.

O chatbot é capaz de:
- responder dúvidas com base em uma base de conhecimento;
- auxiliar em atendimentos recorrentes;
- utilizar IA para gerar respostas claras e contextualizadas;
- registrar históricos de atendimento;
- escalar o suporte sem perder qualidade.

---

# Objetivo do projeto

Simular uma operação real de suporte técnico da Nola, automatizando respostas para dúvidas frequentes de clientes de restaurantes através de IA e automações.

---

# Tecnologias utilizadas

- N8N
- Google Sheets
- Groq API
- IA Generativa (LLM)
- Workflow Automation

---

# Estrutura da solução

O fluxo foi desenvolvido seguindo a seguinte lógica:

```txt
Usuário
   ↓
Chat Trigger
   ↓
Busca na Base de Conhecimento (Google Sheets)
   ↓
Processamento com IA
   ↓
Resposta ao usuário
   ↓
Registro do histórico de atendimento

Funcionalidades
Chatbot com IA

O chatbot recebe perguntas dos usuários e utiliza IA para gerar respostas baseadas na base de conhecimento cadastrada.

Base de conhecimento integrada

As respostas são alimentadas a partir de uma planilha no Google Sheets contendo:

perguntas frequentes;
respostas;
categorias de suporte.
Fallback inteligente

Caso a IA não encontre uma resposta adequada na base de conhecimento, o sistema retorna:

"Não encontrei essa informação na base de conhecimento. Vou encaminhar seu caso para o time responsável."

Histórico de atendimentos

Todas as interações podem ser registradas automaticamente em uma aba de histórico contendo:

pergunta;
resposta;
data do atendimento.
Estrutura da planilha
Aba: BaseConhecimento
Pergunta	Resposta	Categoria
Aba: HistoricoAtendimentos
Pergunta	Resposta	Data
Diferenciais implementados
Integração com IA generativa
Automação completa via N8N
Organização da base por categorias
Tratamento de fallback
Histórico automático de atendimentos
Estrutura pensada para escalabilidade
Fluxo visual limpo e organizado
Uso de Inteligência Artificial no desenvolvimento

Ferramentas de IA como ChatGPT foram utilizadas como apoio estratégico durante o desenvolvimento do projeto, auxiliando em:

refinamento de prompts;
estruturação lógica do workflow;
melhoria das respostas do chatbot;
otimização da experiência do usuário;
entendimento e aprendizado das ferramentas utilizadas.

O objetivo foi utilizar IA como suporte para acelerar aprendizado, organização e qualidade da solução proposta.

Como executar
1. Importar o workflow no N8N

Importe o arquivo JSON do workflow disponível neste repositório.

2. Configurar credenciais

Adicionar:

credenciais do Google Sheets;
API Key da Groq.
3. Executar workflow

Ative o workflow e utilize o chat para realizar perguntas.

Exemplos de perguntas
Como redefinir minha senha?
Como cadastrar funcionário?
Impressora não imprime pedidos
Como fechar o caixa?
Pedido não aparece na cozinha
Estrutura do workflow
Nodes utilizados
Chat Trigger
Google Sheets
AI Agent
Append Row in Sheet
Considerações finais

Este projeto foi desenvolvido com foco em:

experiência do cliente;
eficiência operacional;
escalabilidade;
organização do suporte técnico;
uso estratégico de automações e IA.

A proposta busca demonstrar como ferramentas simples podem gerar impacto real em operações de Customer Success.

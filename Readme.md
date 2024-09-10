# Bot Universitário para WhatsApp com Dialogflow

## Visão Geral

Este projeto é um bot para WhatsApp desenvolvido para uma universidade. Utiliza o **Dialogflow** para gerenciar conversas e o **Fulfillment do Google** para fornecer respostas personalizadas. O bot está integrado ao WhatsApp API e usa contextos para garantir uma conversa fluida e precisa. Ele fornece informações e realiza ações relacionadas à universidade, incluindo:

- Laboratório
- Cantina
- Estacionamento
- Secretaria
- Agendamento de Laboratório
- Avaliações
- Biblioteca

## Funcionalidade

### Integração com o WhatsApp API

Permite que o bot receba e envie mensagens para os usuários diretamente no WhatsApp.

### Dialogflow

- **Intenções**: Define como o bot deve responder a diferentes tipos de perguntas e solicitações relacionadas à universidade.
- **Entidades**: Extrai informações específicas das mensagens do usuário, como datas e locais.

### Fulfillment do Google

- Personaliza as respostas do bot e interage com serviços externos para obter ou manipular dados relacionados à universidade.
- Permite a execução de lógica personalizada, como verificar a disponibilidade de salas de laboratório ou agendar exames.

### Contextos

- Mantém o estado da conversa para fornecer respostas precisas e garantir um fluxo contínuo na interação com o bot.
- Armazena informações importantes sobre a conversa atual, como o tipo de solicitação ou o nome do usuário.

## Como Funciona

1. **Recepção da Mensagem**: O usuário envia uma mensagem pelo WhatsApp com uma pergunta ou solicitação relacionada à universidade.
2. **Processamento no Dialogflow**: A mensagem é analisada pelo Dialogflow, que identifica a intenção e as entidades.
3. **Fulfillment**: O Fulfillment pode buscar informações específicas de sistemas da universidade, como horários de funcionamento da cantina ou disponibilidade de vagas de estacionamento. A resposta é formatada com base nas informações obtidas e retornada ao usuário.
4. **Envio da Resposta**: A resposta formatada é enviada de volta ao usuário através do WhatsApp API.
5. **Manutenção do Contexto**: Contextos são usados para lembrar informações importantes e garantir um fluxo contínuo e relevante na conversa.

## Exemplos de Fluxo

### Exemplo 1: Informações sobre Laboratório

- **Usuário**: "Qual é o horário de funcionamento do laboratório de informática?"
- **Dialogflow**: Identifica a intenção de consulta sobre o laboratório.
- **Fulfillment**: Busca o horário de funcionamento do laboratório e formata a resposta.
- **Resposta**: "O laboratório de informática está aberto de segunda a sexta-feira, das 8h às 18h."

### Exemplo 2: Agendamento de Laboratório

- **Usuário**: "Gostaria de agendar o laboratório para o dia 15 de setembro."
- **Dialogflow**: Identifica a intenção de agendamento.
- **Fulfillment**: Verifica a disponibilidade do laboratório para a data solicitada e confirma o agendamento.
- **Resposta**: "Seu agendamento para o laboratório no dia 15 de setembro foi confirmado."

### Exemplo 3: Consulta sobre Cantina

- **Usuário**: "Quais são os pratos disponíveis hoje na cantina?"
- **Dialogflow**: Identifica a intenção de consulta sobre o cardápio da cantina.
- **Fulfillment**: Busca o cardápio do dia na cantina e formata a resposta.
- **Resposta**: "Hoje na cantina temos: arroz, feijão, frango grelhado e salada."

## Configuração

### Configuração do Dialogflow

- Crie um projeto no Dialogflow e defina as intenções e entidades necessárias para lidar com consultas e agendamentos universitários.
- Configure o Fulfillment para interagir com sistemas da universidade e obter dados relevantes.

### Configuração do WhatsApp API

- Integre o bot ao WhatsApp API para envio e recebimento de mensagens.

### Configuração do Fulfillment

- Implemente o Fulfillment para personalizar as respostas e manipular dados de sistemas universitários conforme necessário.

### Contextos

- Configure os contextos no Dialogflow para manter o estado da conversa e garantir um fluxo contínuo.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

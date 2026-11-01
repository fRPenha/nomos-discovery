# Nomos Discovery

Nomos é uma metodologia de descoberta de necessidades, acompanhada de uma skill para agentes de IA. Foi construído para ajudar pessoas a compreender o que realmente precisam antes de decidir o que construir e antes de começar a especificação.

Uma ideia inicial pode chegar como uma solução pronta — um relatório, uma automação ou um sistema — sem que o problema e o resultado desejado estejam claros. O Nomos conduz uma conversa para investigar a situação, separar fatos de hipóteses, identificar pessoas e contextos afetados, avaliar alternativas e validar uma síntese com quem fez a solicitação.

A descoberta pode indicar que a melhor próxima ação é um experimento, uma mudança de processo, a utilização de algo que já existe ou a construção de software. Quando software se justifica e há clareza suficiente, o resultado pode servir de entrada para uma etapa posterior de especificação, inclusive com ferramentas de SDD como o GitHub Spec Kit. O Nomos não substitui essa etapa e não implementa a solução.

## O que existe neste repositório

- [`skills/nomos/SKILL.md`](skills/nomos/SKILL.md): versão existente da skill de descoberta.
- [`skills/nomos/references/contrato.md`](skills/nomos/references/contrato.md): modelo de contrato de discovery usado por essa versão.

## Estado atual

Esta é a publicação inicial da skill na forma em que foi construída. Ela foi criada para um ambiente específico e ainda contém referências ao `hub-central`, a comandos, sistemas e fluxos desse ambiente. Essas dependências não acompanham este repositório; portanto, a skill **ainda não é uma instalação independente pronta para uso geral**. Sua adaptação e evolução são trabalhos futuros.

O conteúdo está disponível para conhecer a intenção, os princípios e o fluxo atual do Nomos. As instruções específicas de registro e integração devem ser avaliadas e adaptadas ao contexto de cada pessoa antes do uso.

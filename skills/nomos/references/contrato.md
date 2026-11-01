# Modelo do contrato de Discovery (hub-central)

Mantenha todas as seções mesmo quando algo for desconhecido: use `[DESCONHECIDO]`, nunca omita nem complete. Cada item relevante indica estado e evidência (`Rxx`).

```markdown
---
id: AAAA-MM-DD_slug
status: draft | blocked                 # omitir em relatorios/
created_by: claude-code
created_at: <hora-agora>
source_ticket: KACE-xxxxx | none
related_jira: BOPE-xxx | none
updated_by:
  - { by: claude-code, at: <hora-agora>, action: "Discovery Nomos registrado" }
artifact: nomos-discovery
discovery_status: draft | blocked | ready_for_specification | not_for_specification
classification: software_justificado | experimento_antes_do_software | acao_nao_tecnologica | insuficiente
revision: 1
approved_revision: null | <número>
validated_by_requester: true | false
validated_at: AAAA-MM-DD | null
raw_interview_sharing_authorized: true | false
---

# Discovery — <título descritivo>

## 1. Declaração original
Registro fiel do pedido inicial, sem reinterpretar.

## 2. Intenção validada
- Mudança desejada:
- Por que importa:
- Resultado observável:
- Evidências: Rxx

## 3. Situação atual
- Como funciona hoje:
- O que já foi tentado:
- Obstáculos ou causas percebidas:
- Impacto de ficar como está:

## 4. Atores e contexto
| Ator ou grupo | Papel/necessidade | Situações ou gatilhos | Frequência/variações | Evidências |
|---|---|---|---|---|

## 5. Resultado mínimo de valor
- Resultado mínimo aceitável:
- O que precisa ser verdade para gerar valor:
- O que ainda não é necessário:
- Estado e evidências:

## 6. Cenários essenciais
Para cada cenário: contexto inicial, objetivo do ator, resultado esperado, exceções conhecidas. Sem interface nem arquitetura.

## 7. Necessidades
| ID | Necessidade | Origem | Prioridade declarada | Estado |
|---|---|---|---|---|

## 8. Escopo validado
### Incluído
### Excluído
### Adiado

## 9. Regras e invariantes conhecidos
Cada uma com ID, estado e evidência.

## 10. Dados envolvidos
| Dado | Origem | Uso necessário | Sensibilidade | Retenção/limites | Estado |
|---|---|---|---|---|---|

## 11. Restrições
- Prazo:
- Custo:
- Privacidade e segurança (LGPD):
- Conformidade:
- Sistemas existentes (Protheus, KACE, integrações):
- Preferências técnicas declaradas:
Prioridade não declarada fica `[DESCONHECIDO]`.

## 12. Critérios de sucesso
| ID | Resultado a observar | Medida | Sinal ou limiar | Evidências |
|---|---|---|---|---|

## 13. Alternativas consideradas
| Alternativa | Por que considerar | Decisão | Justificativa | Evidências |
|---|---|---|---|---|

## 14. Premissas, desconhecidos e conflitos
| ID | Tipo | Descrição | Bloqueia a especificação? | Dono da resposta | Tratamento |
|---|---|---|---|---|---|

## 15. Decisões registradas
| ID | Decisão | Estado | Responsável pela decisão | Evidências |
|---|---|---|---|---|

## 16. Riscos de interpretação
Onde quem especifica pode transformar intenção em requisito errado.

## 17. Rastreabilidade
| Elemento | Respostas/fontes | Confirmação |
|---|---|---|

## 18. Avaliação de prontidão
| Critério | Estado | Observação |
|---|---|---|

Conclusão: <discovery_status e justificativa>

## 19. Dados que a execução precisa
(Seção exigida pelo hub-central.) Escopo nomeado de cada fonte, chave de junção entre sistemas, definição operacional de cada sinal que vira número. Pronto = só faltam decisões, não dados.

## 20. Próximo passo
- `ready_for_specification`: instrução para quem especifica — trate este documento como fonte de intenção, não autorização para inventar requisito; recuse se `discovery_status` não for `ready_for_specification`, se `validated_by_requester` não for `true` ou se `approved_revision` ≠ `revision`; preserve escopo, exclusões e IDs; não converta `[DESCONHECIDO]` em decisão; devolva contradição bloqueadora ao Discovery. Sugestão: `/grilling`.
- `experimento_antes_do_software`: hipótese, sinal, prazo/amostra, responsável e decisão que o resultado permite.
- `acao_nao_tecnologica`: a ação aprovada e quem a executa. Nenhum handoff de software.
- `insuficiente`: perguntas bloqueadoras e seus donos; qualquer agente seguinte deve recusar o documento.

## 21. Registro da validação
- Síntese apresentada:
- Correções solicitadas:
- Aprovação explícita:
- Data:

## Apêndice A — Respostas da entrevista
Só se `raw_interview_sharing_authorized: true`. Prefira síntese fiel e mínima.

| ID | Pergunta | Resposta/síntese fiel | Estado |
|---|---|---|---|
```

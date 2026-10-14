# 📘 Tipos de detecção

[← Início](../README.md)

| Tipo | Interpretação | Limitação |
|---|---|---|
| Assinatura / hash | Artefato corresponde a regra conhecida | Pode haver exceções e colisões de contexto |
| Comportamental | Atividade ou sequência se parece com técnica suspeita | Operações benignas podem acionar a regra |
| Regra personalizada / blocklist | Política local proibiu um indicador | Não equivale a nova confirmação independente de malware |
| Heurística / IA | Modelo atribuiu suspeita ao comportamento | Requer validação por evidências adicionais |

## Dica
Analise a **detecção original**, separadamente dos alertas produzidos depois por uma blocklist criada pelo analista.

# 🔬 Análise de artefatos recuperados do EDR

[🌐 Abrir guia web](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/EDR-Retrieved-Artifacts/) · [← Evidence Collection](../02-Evidence-Collection/README.md)

## Objetivo
Recuperar, preservar e analisar **estaticamente** um artefato disponibilizado pelo EDR, sem executá-lo.

1. **Retrieve File:** coletar por funcionalidade autorizada do EDR.
2. **Preservação:** registrar origem, data/hora, hash SHA256 e cadeia de custódia.
3. **Inspeção:** listar conteúdo de um ZIP protegido em cópia controlada.
4. **Análise:** para PDFs, usar PDFiD/pdf-parser.py e contextualizar marcadores.

## Comandos úteis

```powershell
Get-FileHash -LiteralPath 'C:\Analise\amostra.zip' -Algorithm SHA256
& 'C:\Program Files\7-Zip\7z.exe' l 'C:\Analise\amostra.zip'
```

## Indicadores PDF

| Indicador | Interpretação inicial |
|---|---|
| /JavaScript, /JS | Pode indicar JavaScript incorporado |
| /OpenAction, /AA | Ações na abertura ou eventos |
| /Launch | Ação de lançamento |
| /URI | Link externo, não necessariamente malicioso |
| /XFA, /RichMedia | Conteúdo interativo que requer contexto |

**Limitação:** buscas textuais simples podem não encontrar objetos comprimidos, codificados ou ofuscados. Use ferramentas especializadas e correlacione evidências. Evite executar, pré-visualizar ou enviar amostras privadas a serviços públicos. Todos os exemplos são fictícios.

[PDF Tools — Didier Stevens](https://blog.didierstevens.com/programs/pdf-tools/)

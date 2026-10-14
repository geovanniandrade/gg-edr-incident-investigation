# 🧪 Case 001 — Suspicious Installer (simulado)

[← Início](../../README.md)

> **Cenário 100% fictício:** não descreve incidente real, nenhum fabricante foi identificado como malicioso e todos os indicadores são ilustrativos.

## Contexto
Uma pessoa acessa uma página pública com publicidade, baixa um instalador não validado e tenta instalá-lo. O EDR produz uma detecção comportamental de possível injeção de código e bloqueia o processo.

## Linha do tempo didática
| Horário (UTC-03:00) | Evento | Status da evidência |
|---|---|---|
| 10:00 | Clique em publicidade | Relato de usuário |
| 10:02 | Arquivo em Downloads | Registro simulado de browser |
| 10:04 | Tentativa de instalação | Telemetria EDR simulada |
| 10:04 | Bloqueio por comportamento | Alerta original simulado |
| 10:10 | Verificação e preservação | Registro do analista |

## Guia de análise
1. **Triage:** identificar se a detecção ocorreu antes ou depois do início de execução.
2. **Preserve:** registrar alerta, processo e hash fictício sem carregar o arquivo.
3. **Investigate:** confirmar processos pais/filhos, assinatura e conexões.
4. **Enrich:** conferir fonte do download e reputação, evitando confundir anúncio com site de destino.
5. **Contain:** registrar ação do EDR e validar resíduos, sem inferir limpeza por status 'Mitigated'.
6. **Verdict:** manter **Undefined** se não houver evidência suficiente de malícia ou benignidade.
7. **Report:** documentar impacto, incertezas e ações.

## Questões para o analista
- Uma classificação 'Ransomware' comprova criptografia? **Não.**
- Blocklist manual significa nova prova de malware? **Não.**
- Clique em download prova execução? **Não.**
- É possível ter execução durante tentativa de instalação? **Sim; verifique a árvore de processos.**

## Conclusão do exercício
**Detecção e bloqueio registrados; malícia e comprometimento não comprovados no material disponível.** O resultado correto do treinamento é distinguir prevenção de confirmação de ataque.

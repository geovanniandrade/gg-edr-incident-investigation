# 🛡️ GG // EDR Incident Investigation

**Practical Blue Team Investigation & Incident Response**

Guia aberto de triagem, investigação, contenção e documentação de alertas de EDR — com exemplos práticos e metodologia independente de fabricante.

> **Projeto educacional:** cases, indicadores, equipamentos e evidências são fictícios. Não há dados corporativos reais.

## 🎯 Objetivo
Ensinar analistas a responder: **o que aconteceu, quais evidências sustentam a conclusão e o que ainda precisa ser validado?**

**Triage → Preserve → Investigate → Enrich → Contain/Remediate → Verdict → Report**

> A contenção emergencial pode ocorrer a qualquer momento, mediante autorização e registro do impacto. Não espere a etapa 05 diante de ameaça ativa.

## 🔎 Playbooks — investigação em 7 etapas

| Etapa | Guia | Resultado |
|---|---|---|
| 01 | [Alert Triage](Playbooks/01-Alert-Triage/README.md) | Prioridade e hipótese inicial |
| 02 | [Evidence Collection](Playbooks/02-Evidence-Collection/README.md) | Evidências íntegras e catalogadas |
| 03 | [Process Investigation](Playbooks/03-Process-Investigation/README.md) | Árvore de processos e linha do tempo |
| 04 | [Threat Intelligence](Playbooks/04-Threat-Intelligence/README.md) | IoCs enriquecidos e contextualizados |
| 05 | [Containment & Remediation](Playbooks/05-Containment-Remediation/README.md) | Ações documentadas e eficácia validada |
| 06 | [Analyst Verdict](Playbooks/06-Analyst-Verdict/README.md) | Veredito fundamentado |
| 07 | [Incident Reporting](Playbooks/07-Incident-Reporting/README.md) | Relatório rastreável |

## 📚 Explore o projeto

| Seção | O que você encontra |
|---|---|
| [📘 Knowledge Base](Knowledge-Base/EDR-Fundamentals.md) | Conceitos de EDR, detecções, MITRE ATT&CK e Threat Intelligence |
| [🧰 PowerShell](Tools-and-Commands/PowerShell/README.md) | Comandos de consulta no Windows |
| [🐧 Linux](Tools-and-Commands/Linux/README.md) | Comandos de consulta em endpoints Linux |
| [📑 Templates](Templates/Investigation-Checklist.md) | Checklist, registro de evidências e relatório |
| [🧪 Case 001 — Suspicious Installer](Case-Studies/001-Suspicious-Installer/README.md) | Investigação didática de alerta EDR |

## ✅ Princípios da investigação

- **Detecção não é veredito:** classificação de ransomware não comprova criptografia.
- **Mitigação não é limpeza comprovada:** valide o endpoint e a possibilidade de persistência.
- **Contexto é essencial:** um arquivo com nome legítimo pode ser malicioso; reputação isolada não comprova legitimidade.
- **Preserve antes de alterar**, quando viável, e documente todas as ações.
- **Separe três resultados:** veredito da detecção, eficácia da contenção e impacto efetivo.
- **Não execute amostras suspeitas** fora de laboratórios isolados e autorizados.

## 📖 Referências
- [NIST SP 800-61 Rev. 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final)
- [NIST SP 800-86](https://csrc.nist.gov/pubs/sp/800/86/final)
- [MITRE ATT&CK](https://attack.mitre.org/)
- [CISA Incident & Vulnerability Response Playbooks](https://www.cisa.gov/resources-tools/resources/federal-government-cybersecurity-incident-and-vulnerability-response-playbooks)

---

*Material educacional para ambientes autorizados. Os controles e a resposta precisam seguir as políticas da organização.*

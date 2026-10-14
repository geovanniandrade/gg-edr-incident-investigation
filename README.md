# 🛡️ GG // EDR Incident Investigation

**Blue Team • EDR • DFIR • Incident Response**

Projeto educacional com **playbooks objetivos** para investigar alertas de EDR, interpretar evidências, consultar indicadores e documentar decisões técnicas. A metodologia é independente de fabricante.

[![Abrir interface web](https://img.shields.io/badge/🌐_ABRIR_INTERFACE_WEB-2F81F7?style=for-the-badge)](https://geovanniandrade.github.io/gg-edr-incident-investigation/)
[![Playbooks](https://img.shields.io/badge/🛡️_7_PLAYBOOKS-181717?style=for-the-badge)](https://geovanniandrade.github.io/gg-edr-incident-investigation/#playbooks)

---

## 🔗 Acesso rápido

[**🛡️ Tratar um incidente — pesquisa de IoCs**](https://geovanniandrade.github.io/gg-edr-incident-investigation/#tratar-incidente) · [**📦 Artefatos recuperados do EDR — interface web**](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/EDR-Retrieved-Artifacts/)

## 🎯 Como utilizar

**Triage → Preserve → Investigate → Enrich → Contain → Verdict → Report**

Acesse a [**interface web**](https://geovanniandrade.github.io/gg-edr-incident-investigation/), escolha uma etapa e siga o roteiro: **o que verificar → comando útil → onde investigar → checklist**.

> ⚠️ Em caso de ameaça ativa, a contenção autorizada pode ocorrer antes de concluir as outras etapas. Registre as ações e preserve evidências sempre que possível.

## 🔎 Playbooks — 7 etapas

| Etapa | Guia interativo | Objetivo |
|:---:|---|---|
| 01 | [Alert Triage](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/01-Alert-Triage/) | Priorizar o alerta |
| 02 | [Evidence Collection](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/02-Evidence-Collection/) | Preservar evidências |
| 03 | [Process Investigation](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/03-Process-Investigation/) | Validar execução e processos |
| 04 | [Threat Intelligence](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/04-Threat-Intelligence/) | Enriquecer indicadores |
| 05 | [Containment & Remediation](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/05-Containment-Remediation/) | Conter e validar mitigação |
| 06 | [Analyst Verdict](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/06-Analyst-Verdict/) | Definir o veredito |
| 07 | [Incident Reporting](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/07-Incident-Reporting/) | Documentar o incidente |

## 🧰 Onde investigar?

A interface inclui um **seletor por tipo de indicador** — Hash/Arquivo, URL/Domínio, IP ou Comportamento — com links às plataformas mais adequadas.

| Ferramenta | Aplicação |
|---|---|
| [VirusTotal](https://www.virustotal.com/gui/home/search) | Reputação de hashes, URLs, IPs e domínios |
| [urlscan.io](https://urlscan.io/) | Navegação, recursos e redirecionamentos de URLs |
| [MalwareBazaar](https://bazaar.abuse.ch/) | Pesquisa de hashes e amostras conhecidas |
| [Hybrid Analysis](https://www.hybrid-analysis.com/) / [ANY.RUN](https://any.run/) | Relatórios de análise comportamental em sandbox |
| [AbuseIPDB](https://www.abuseipdb.com/) | Histórico de denúncias de IPs |
| [MITRE ATT&CK](https://attack.mitre.org/) | Técnicas e táticas relacionadas a evidências observadas |

**Privacidade:** nunca envie amostras, logs, documentos ou URLs com informações corporativas sensíveis para serviços públicos sem autorização. Reputação isolada não confirma malware.

## 📚 Recursos complementares

| Material | Acesso |
|---|---|
| Conceitos fundamentais | [Knowledge Base](Knowledge-Base/EDR-Fundamentals.md) |
| Comandos de consulta Windows | [PowerShell](Tools-and-Commands/PowerShell/README.md) |
| Comandos de consulta Linux | [Linux](Tools-and-Commands/Linux/README.md) |
| Checklist de investigação | [Investigation Checklist](Templates/Investigation-Checklist.md) |
| Registro de evidências | [Evidence Register](Templates/Evidence-Register.md) |
| Modelo de relatório | [Incident Report](Templates/Incident-Report.md) |
| Análise de artefatos recuperados | [Guia web — Retrieve File, ZIP e PDF](https://geovanniandrade.github.io/gg-edr-incident-investigation/Playbooks/EDR-Retrieved-Artifacts/) |
| Exercício simulado | [Case 001 — Suspicious Installer](Case-Studies/001-Suspicious-Installer/README.md) |

## ✅ Princípios

- **Detecção ≠ comprometimento confirmado.**
- **Mitigated ≠ endpoint comprovadamente limpo.**
- **True Positive / False Positive / Undefined** precisam de justificativa baseada em evidências.
- Preserve horários, origem, integridade e contexto dos artefatos.

## 📖 Referências

[NIST SP 800-61 Rev. 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final) · [NIST SP 800-86](https://csrc.nist.gov/pubs/sp/800/86/final) · [MITRE ATT&CK](https://attack.mitre.org/) · [CISA Incident Response Playbooks](https://www.cisa.gov/resources-tools/resources/federal-government-cybersecurity-incident-and-vulnerability-response-playbooks)

---

*Todos os exemplos são didáticos e fictícios. Nenhum dado corporativo real é publicado neste projeto.*

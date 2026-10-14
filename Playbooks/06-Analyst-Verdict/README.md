# 06 — Veredito do analista

[← Voltar ao início](../../README.md)

## 🎯 Objetivo
Classificar o alerta separando certeza da detecção, contenção e impacto.

## 🔍 Como investigar
Use True Positive quando comportamento malicioso estiver sustentado; False Positive quando a atividade benigna estiver demonstrada; Undefined/Inconclusive quando faltar evidência. Classifique vetor (phishing, malvertising etc.) apenas com prova.

## 🧰 Ferramentas e comandos — se aplicável
Consulte os exemplos de [PowerShell](../../Tools-and-Commands/PowerShell/README.md) ou [Linux](../../Tools-and-Commands/Linux/README.md) somente em sistemas autorizados. Registre comando, contexto e saída relevante.

## ⚠️ Atenção
Bloquear um instalador não transforma automaticamente a detecção em True Positive; escolher Ransomware exige evidência própria.

## ✅ Checklist
- [ ] Evidências favoráveis e contrárias citadas
- [ ] Veredito e confiança explícitos
- [ ] Grau de comprometimento separado da mitigação
- [ ] Revisão por analista quando necessário

## 📝 Entregável
Atualize o [Investigation Checklist](../../Templates/Investigation-Checklist.md), o [Evidence Register](../../Templates/Evidence-Register.md) e, quando aplicável, o [Incident Report](../../Templates/Incident-Report.md).

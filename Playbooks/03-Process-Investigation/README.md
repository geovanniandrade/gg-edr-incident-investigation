# 03 — Investigação de processos

[← Voltar ao início](../../README.md)

## 🎯 Objetivo
Reconstituir o que foi executado, por quem, quando e com quais efeitos.

## 🔍 Como investigar
Analise processo pai e filhos, command line, caminho, assinatura, módulos carregados, conexões e persistência. Correlacione telemetria do EDR com logs do sistema.

## 🧰 Ferramentas e comandos — se aplicável
Consulte os exemplos de [PowerShell](../../Tools-and-Commands/PowerShell/README.md) ou [Linux](../../Tools-and-Commands/Linux/README.md) somente em sistemas autorizados. Registre comando, contexto e saída relevante.

## ⚠️ Atenção
O clique em download não comprova execução; uma detecção comportamental pode apontar execução mesmo que o usuário negue abertura manual.

## ✅ Checklist
- [ ] Árvore de processos examinada
- [ ] Linha do tempo correlacionada
- [ ] Execução e ações pós-execução diferenciadas
- [ ] Lacunas documentadas

## 📝 Entregável
Atualize o [Investigation Checklist](../../Templates/Investigation-Checklist.md), o [Evidence Register](../../Templates/Evidence-Register.md) e, quando aplicável, o [Incident Report](../../Templates/Incident-Report.md).

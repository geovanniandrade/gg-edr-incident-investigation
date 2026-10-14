# 📘 Fundamentos de EDR

[← Início](../README.md)

**Endpoint Detection and Response (EDR)** coleta telemetria de endpoint, detecta atividades suspeitas e pode responder com bloqueio, quarentena, encerramento de processo ou isolamento.

## Três conceitos que não devem ser confundidos
- **Detection:** o que a ferramenta observou e classificou.
- **Mitigation:** quais ações foram solicitadas e concluídas.
- **Impact:** o que efetivamente ocorreu no ativo, usuário e negócio.

Uma detecção crítica não comprova ataque bem-sucedido. Uma mitigação bem-sucedida não é laudo forense de limpeza. Registre as limitações de visibilidade do produto.

## Investigação independente de fornecedor
Procure regra, horário, identidade do endpoint, processo pai e filhos, command line, hash, assinatura, arquivo, conexões, alterações persistentes e resposta aplicada. Os nomes das telas variam entre produtos.

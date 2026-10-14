# 📘 Threat Intelligence

[← Início](../README.md)

## IoCs comuns
SHA256, endereço IP, domínio, URL, nome e caminho de arquivo, certificado e processo. Um IoC isolado não determina intenção.

## Procedimento seguro
- Verifique se o indicador está **realmente ligado** ao evento analisado.
- Registre fonte, data/hora e divergências entre fornecedores.
- Compare reputação com telemetria e assinatura digital.
- Não submeta logs privados, URLs com tokens ou arquivos internos a serviços públicos sem autorização.

**Exemplo:** uma URL encurtada pode mostrar anúncios, redirecionamentos ou um destino legítimo. Sem histórico de download, não atribua o executável à URL.

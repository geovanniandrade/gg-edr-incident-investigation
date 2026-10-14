# 🐧 Comandos Linux — consulta

[← Início](../../README.md)

Não execute binários suspeitos no host. Use os comandos abaixo apenas com permissão.

## Hash de arquivo
```bash
sha256sum /caminho/arquivo
```

## Processos e ancestrais
```bash
ps -eo pid,ppid,user,lstart,args
```

## Sockets de rede
```bash
ss -tunap
```

## Serviços e tarefas persistentes
```bash
systemctl list-unit-files --type=service
crontab -l
```

## Logs recentes do serviço
```bash
journalctl --since '1 hour ago' --no-pager
```

> Preserve timezone, privilégio utilizado e eventuais lacunas de coleta.

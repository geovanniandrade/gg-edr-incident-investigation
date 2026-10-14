# 🧰 Comandos PowerShell — consulta

[← Início](../../README.md)

Execute somente em máquinas autorizadas. Estes comandos consultam informações e não devem executar a amostra suspeita.

## Hash SHA256
```powershell
Get-FileHash -LiteralPath 'C:\Caminho\arquivo.exe' -Algorithm SHA256
```

## Assinatura digital
```powershell
Get-AuthenticodeSignature -LiteralPath 'C:\Caminho\arquivo.exe' | Format-List Status,SignerCertificate,StatusMessage
```

## Processos e linha de comando
```powershell
Get-CimInstance Win32_Process | Select-Object Name,ProcessId,ParentProcessId,CommandLine
```

## Conexões de rede atuais
```powershell
Get-NetTCPConnection | Select-Object LocalAddress,LocalPort,RemoteAddress,RemotePort,State,OwningProcess
```

## Tarefas agendadas
```powershell
Get-ScheduledTask | Select-Object TaskName,TaskPath,State
```

> Saídas podem conter dados pessoais e identificadores internos. Preserve-as apenas em repositório de evidências autorizado.

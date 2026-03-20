# rieux_ssh_multiplexing

Script de automação para configurar a multiplexação SSH local para usuários macOS e Linux/WSL.

## O problema que resolve
Ao trabalhar com HPC, transferências de dados e conexões interativas frequentes exigem a digitação repetida de senha e token 2FA. Este script configura o cliente SSH para reaproveitar conexões seguras.

## Funcionalidades
- Configura regras seguras no `~/.ssh/config`.
- Mantém um "túnel" SSH ativo em segundo plano por 180 minutos após a primeira autenticação.
- Elimina prompts repetidos de senha durante rotinas de bioinformática.

## Como Usar
Basta executar a função no terminal (deve ser carregada via `.zshrc` ou `.bashrc`):
```bash
rieux_ssh_multiplexing

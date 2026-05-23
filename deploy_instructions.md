# Guia de Publicação no GitHub - Repositório Fono-mL

Este guia orienta sobre como conectar seu ambiente local e subir as alterações para o GitHub de maneira segura e profissional.

---

## O que já foi feito localmente?
1. **Limpeza e Proteção**: Criado o arquivo `.gitignore` que impede que arquivos de sistema, logs, variáveis de ambiente `.env` locais e IDEs sejam enviados ao repositório público.
2. **Exemplo de Ambiente**: Criado o arquivo `.env.example` para documentar futuras variáveis de ambiente sem expor dados reais.
3. **Auditoria de Segurança**: Varredura estática de chaves ou segredos concluída com sucesso (nenhum segredo real encontrado).
4. **Git Inicializado**: Repositório local inicializado do zero na branch padrão `main`.
5. **Histórico de Commits**:
   - `chore: adicionar configuracao do gitignore`
   - `feat: adicionar landing page de odontologia e assets`
6. **Conexão Remota**: O repositório local foi conectado com sucesso ao remoto:
   `https://github.com/maluizaaf/Fono-mL.git`

---

## Como fazer o Push para o GitHub?

Abra o seu terminal (PowerShell ou Command Prompt) na pasta do projeto e execute o comando abaixo para enviar o código para a branch `main`:

```bash
git push -u origin main
```

> [!NOTE]
> Se esta for a primeira vez que você está interagindo com o GitHub no seu terminal local, a ferramenta do Git solicitará que você faça login no GitHub através do navegador para autorizar o envio das alterações (autenticação segura HTTPS).

---

## Script Automatizado de Sincronização Futura

Caso você faça novas modificações no código da sua Landing Page e queira subir as atualizações para o GitHub de forma rápida, use os comandos a seguir no terminal:

```bash
# 1. Adicionar todas as novas alterações
git add .

# 2. Criar um commit com uma mensagem descritiva (exemplo)
git commit -m "style: ajustes finos no layout e textos"

# 3. Enviar as alterações para o GitHub
git push
```

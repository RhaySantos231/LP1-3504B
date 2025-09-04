# LP1-3504B
## Sub Titulo
### teste
texto normal

# Principais Comandos Git

| Comando | Descrição |
|---------|-----------|
| `git init` | Inicializa um novo repositório Git na pasta atual |
| `git clone <url>` | Clona um repositório remoto para a máquina local |
| `git status` | Mostra o estado atual dos arquivos (modificados, não rastreados etc.) |
| `git add <arquivo>` | Adiciona um arquivo específico para a área de staging |
| `git add .` | Adiciona **todos os arquivos modificados** para a área de staging |
| `git commit -m "mensagem"` | Registra as mudanças adicionadas com uma mensagem |
| `git log` | Mostra o histórico de commits |
| `git branch` | Lista todas as branches (ramificações) |
| `git branch <nome>` | Cria uma nova branch |
| `git checkout <nome>` | Troca para a branch especificada |
| `git merge <nome>` | Mescla a branch especificada com a branch atual |
| `git remote -v` | Mostra os repositórios remotos configurados |
| `git push origin <branch>` | Envia os commits locais para o repositório remoto |
| `git pull origin <branch>` | Atualiza a branch local com alterações do remoto |
| `git fetch` | Busca atualizações do repositório remoto **sem mesclar** |
| `git reset --hard <hash>` | Reseta o repositório para um commit específico (perigoso, pois apaga alterações locais) |

---

📌 **Dica para alunos iniciantes**:  
A sequência mais comum é:  
```bash
git add .
git commit -m "Mensagem explicativa"
git push origin main

# 🐧 Bash Cheatsheet 2025

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![Last Commit](https://img.shields.io/github/last-commit/blueprintblog/bash-cheatsheet)](https://github.com/blueprintblog/bash-cheatsheet/commits/main)
[![Contributors](https://img.shields.io/github/contributors/blueprintblog/bash-cheatsheet)](https://github.com/blueprintblog/bash-cheatsheet/graphs/contributors)
[![Issues](https://img.shields.io/github/issues/blueprintblog/bash-cheatsheet)](https://github.com/blueprintblog/bash-cheatsheet/issues)
[![Stars](https://img.shields.io/github/stars/blueprintblog/bash-cheatsheet?style=social)](https://github.com/blueprintblog/bash-cheatsheet/stargazers)

> **Sua referência completa para dominar o terminal Linux** - Do iniciante ao avançado, todos os comandos que você precisa em um único lugar.

## 🌐 Acesso Online

Acesse a cheatsheet interativa em: **[cheat-bash.blueprintblog.tech](https://cheat-bash.blueprintblog.tech)**

## 📖 Sobre o Projeto

Esta cheatsheet do Bash foi criada para ser a referência mais completa e prática para desenvolvedores, administradores de sistema e entusiastas de Linux. Com mais de 200 comandos organizados por categoria e nível de dificuldade, além de seções dedicadas para Git, Docker e Scripts prontos, este recurso ajuda você a dominar o terminal e automação de tarefas de forma eficiente.

### 🌟 Novidades na Versão 1.5.0

- **🔀 Página Git**: Comandos avançados de versionamento e colaboração
- **🐳 Página Docker**: Gerenciamento completo de containers e imagens
- **📜 Página Scripts**: Scripts prontos para automação e produtividade
- **🎨 Design Moderno**: Interface responsiva com Alpine.js
- **🧭 Navegação Integrada**: Menu unificado entre todas as seções

### 🎯 Por que esta cheatsheet?

- **90% dos servidores web** rodam Linux
- **Automatize tarefas repetitivas** e aumente sua produtividade
- **DevOps exige domínio de terminal** para pipelines CI/CD
- **Salários 30%+ maiores** para profissionais com domínio de Bash
- **Interface única** para todos os comandos essenciais

## 🚀 Início Rápido

### Instalação

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/blueprintblog/bash-cheatsheet.git
   cd bash-cheatsheet
   ```

2. **Abra a versão HTML:**

   ```bash
   # No navegador
   open bash_cheatsheet_html.html

   # Ou serve localmente
   python3 -m http.server 8000
   # Acesse http://localhost:8000
   ```

3. **Adicione aliases úteis ao seu ~/.bashrc:**
   ```bash
   echo 'alias ll="ls -lah"' >> ~/.bashrc
   echo 'alias gs="git status"' >> ~/.bashrc
   echo 'alias ..="cd .."' >> ~/.bashrc
   source ~/.bashrc
   ```

### Uso

Navegue pela cheatsheet usando os atalhos:

- **Ctrl+F** - Busca rápida de comandos
- **Menu de navegação** - Acesso rápido a todas as seções
- **Cores** - Indicam nível de dificuldade:
  - 🟢 **Iniciante** - Comandos essenciais do dia a dia
  - 🟡 **Intermediário** - Processamento e automação
  - 🔴 **Avançado** - Scripts e administração

### 📄 Páginas Disponíveis

1. **[Página Principal](index.html)** - Comandos Bash por nível
2. **[Comandos Git](git.html)** - Versionamento e colaboração
3. **[Comandos Docker](docker.html)** - Containers e orquestração
4. **[Scripts Prontos](scripts.html)** - Automação e utilitários

## 📚 Conteúdo

### 🟢 Nível Iniciante

#### Navegação & Sistema

```bash
pwd                    # Print Working Directory
whoami                 # Mostra usuário atual
hostname               # Nome do servidor
uname -a               # Info do sistema
ls -la                 # Lista arquivos detalhada
cd pasta/              # Entra na pasta
cd ..                  # Volta 1 nível
cd ~                   # Vai para home
```

#### Arquivos & Diretórios

```bash
touch arquivo.txt      # Cria arquivo vazio
mkdir pasta            # Cria diretório
cp origem destino      # Copia arquivo
mv antigo novo         # Move/Renomeia
rm arquivo             # Deleta arquivo
rm -rf pasta/          # Deleta pasta ⚠️
ln -s origem link      # Link simbólico
```

#### Visualização & Busca

```bash
cat arquivo.txt        # Mostra tudo
head -n 20 file        # Primeiras 20 linhas
tail -f log.txt        # Monitora tempo real
grep "texto" file      # Busca string
find . -name "*.js"    # Busca arquivos
```

### 🟡 Nível Intermediário

#### Processamento de Texto

```bash
cat file | grep "error"    # Filtra linhas
cat file | sort | uniq     # Remove duplicatas
cat file | wc -l           # Conta linhas
sed 's/old/new/g' file     # Substitui todas
awk '{print $1}' file      # Imprime coluna 1
cut -d',' -f1 file.csv     # Corta por delimitador
```

#### Redirecionamento & Pipes

```bash
comando > arquivo          # Sobrescreve
comando >> arquivo         # Adiciona no final
comando 2> erro.log        # Só erros (stderr)
cmd1 | cmd2                # Output cmd1 → input cmd2
cmd | tee file             # Mostra E salva
```

#### Processos & Monitoramento

```bash
ps aux                     # Todos processos
ps aux | grep node         # Busca específico
top                        # Monitor interativo
kill PID                   # Mata processo (TERM)
kill -9 PID                # Mata forçado (KILL)
comando &                  # Executa em background
jobs                       # Lista jobs
```

### 🔴 Nível Avançado

#### Scripts & Variáveis

```bash
#!/bin/bash                # Shebang
nome="João"                # Define variável
echo $nome                 # Usa variável
readonly VAR="fix"         # Constante
arr=(a b c)                # Define array
hoje=$(date)               # Resultado em var
```

#### Condições & Loops

```bash
if [ -f "file" ]; then
  echo "Existe"
fi

for i in {1..5}; do
  echo $i
done

while [ $x -lt 10 ]; do
  echo $x
  ((x++))
done
```

#### Permissões & Segurança

```bash
chmod 755 file             # rwxr-xr-x
chmod +x script.sh         # Torna executável
chown user:group file      # Dono e grupo
ssh-keygen -t ed25519      # Gera chave SSH
sudo comando               # Executa como root
```

## 🔥 Comandos Power

### Logs em tempo real

```bash
tail -f app.log | grep ERROR                    # Filtra ao vivo
tail -f log | awk '{print $1,$5}'               # Extrai colunas
```

### Top IPs de acesso

```bash
cat access.log | awk '{print $1}' | sort | uniq -c | sort -nr | head -10
```

### Busca e substitui em lote

```bash
find . -name "*.js" -exec sed -i 's/var/const/g' {} \;
grep -rl "old" . | xargs sed -i 's/old/new/g'
```

### Paralelização

```bash
cat urls.txt | xargs -P 10 -I {} curl -O {}    # 10 paralelos
find . -name "*.jpg" | parallel convert {} {.}.png
```

## ⌨️ Atalhos Essenciais

| Atalho    | Função                    |
| --------- | ------------------------- |
| `Ctrl+A`  | Início da linha           |
| `Ctrl+E`  | Fim da linha              |
| `Ctrl+U`  | Apaga linha inteira       |
| `Ctrl+K`  | Apaga até o fim           |
| `Ctrl+W`  | Apaga palavra anterior    |
| `Ctrl+R`  | Busca histórico (reverso) |
| `Ctrl+L`  | Limpa tela (clear)        |
| `Ctrl+C`  | Cancela comando           |
| `Ctrl+Z`  | Pausa processo            |
| `Ctrl+D`  | Exit (logout)             |
| `Tab`     | Autocomplete              |
| `Tab Tab` | Mostra opções             |

## 🔀 Comandos Git Essenciais

```bash
git status -s               # Status curto
git log --oneline --graph   # Histórico visual
git checkout -b feature     # Criar branch
git merge feature           # Merge de branch
git rebase -i HEAD~3        # Rebase interativo
git stash                   # Salvar mudanças
git reset --soft HEAD~1     # Desfazer commit
```

## 🐳 Comandos Docker Essenciais

```bash
docker ps                    # Containers rodando
docker ps -a                 # Todos containers
docker logs -f container     # Logs tempo real
docker exec -it container bash  # Entra no container
docker stop $(docker ps -aq)    # Para todos
docker system prune -a       # Limpa tudo
```

## 📜 Scripts Práticos

### Backup Automático

```bash
#!/bin/bash
tar -czf "backup_$(date +%Y%m%d).tar.gz" /diretorio/important
find /backups -name "*.tar.gz" -mtime +7 -delete
```

### Monitor de Sistema

```bash
#!/bin/bash
while true; do
    echo "CPU: $(top -bn1 | grep "Cpu(s)" | awk '{print $2}')"
    echo "Memória: $(free -h | grep Mem | awk '{print $3"/"$2}')"
    sleep 5
done
```

## 📊 Estatísticas do Mercado

- **90%** dos servidores rodam Linux
- **80%** das vagas DevOps exigem Bash
- **70%** dos deploys otimizados usam scripts
- **30%+** salário médio DevOps vs Júnior

## 🎯 Casos de Uso

### Desenvolvimento

- **Automação de builds** e testes
- **Deploy contínuo** com scripts
- **Gerenciamento** de múltiplos projetos
- **Integração** com Git e Docker

### Administração

- **Monitoramento** de servidores
- **Backup automatizado** de dados
- **Manutenção** de sistemas
- **Análise** de logs e relatórios

### Produtividade

- **Scripts personalizados** para tarefas repetitivas
- **Aliases** para comandos frequentes
- **Atalhos** para navegação eficiente
- **Templates** para projetos padrão

## 🤝 Como Contribuir

Contribuições são bem-vindas! Por favor:

1. **Faça um fork** do projeto
2. **Crie uma branch** para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. **Faça commit** das suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. **Push** para a branch (`git push origin feature/nova-funcionalidade`)
5. **Abra um Pull Request**

### Diretrizes de Contribuição

- ✅ **Comandos testados** e funcionais
- ✅ **Descrições claras** e concisas
- ✅ **Exemplos práticos** de uso
- ✅ **Organização** por categoria/nível
- ✅ **Formatação** consistente com o projeto

## 🐛 Reportando Issues

Encontrou um erro ou tem uma sugestão?

1. **Verifique issues existentes**
2. **Use templates** apropriados
3. **Forneça detalhes**: sistema, shell, erro exato
4. **Inclua exemplos** quando possível

## 📝 Licença

Este projeto está licenciado sob a **Licença MIT** - veja o arquivo [LICENSE](LICENSE) para detalhes.

### Por que MIT?

- ✅ **Liberdade total** para uso comercial e pessoal
- ✅ **Permite modificação** e distribuição
- ✅ **Apenas requer** atribuição original
- ✅ **Compatível** com projetos open source
- ✅ **Ideal** para recursos educacionais

## 👤 Autor

**[genildocs](https://github.com/genildocs)**

- 🌐 **Website:** [blueprintblog.tech](https://blueprintblog.tech)
- 🐙 **GitHub:** [@genildocs](https://github.com/genildocs)
- 🐦 **Twitter:** [@blueprintblog](https://twitter.com/blueprintblog)

## 🙏 Agradecimentos

- Comunidade Linux e Unix
- Contribuidores de código aberto
- Documentação oficial Bash
- Todos que compartilham conhecimento

## 🔗 Links Úteis

### Bash e Shell

- [Documentação Oficial Bash](https://www.gnu.org/software/bash/manual/)
- [ShellCheck - Validador de Scripts](https://www.shellcheck.net/)
- [ExplainShell - Expande Comandos](https://explainshell.com/)
- [Bash Academy - Cursos Gratuitos](https://www.bash.academy/)

### Git e Versionamento

- [Documentação Oficial Git](https://git-scm.com/doc)
- [Git Interactive Tutorial](https://learngitbranching.js.org/)
- [Pro Git Book](https://git-scm.com/book/pt-br/v2)

### Docker e Containers

- [Documentação Oficial Docker](https://docs.docker.com/)
- [Docker Hub](https://hub.docker.com/)
- [Play with Docker](https://labs.play-with-docker.com/)

### DevOps e Automação

- [DevOps Roadmap](https://roadmap.sh/devops)
- [Awesome Bash](https://github.com/awesome-lists/awesome-bash)
- [Shell Scripting Best Practices](https://google.github.io/styleguide/shellguide.html)

---

<div align="center">

**⭐ Se este projeto ajudou você, deixe uma estrela!**

Made with ❤️ by [genildocs](https://github.com/genildocs)

[🏠 Voltar ao Início](#-bash-cheatsheet-2025) • [🌐 Site Online](https://cheat-bash.blueprintblog.tech) • [📧 Contato](mailto:contato@blueprintblog.tech)

</div>

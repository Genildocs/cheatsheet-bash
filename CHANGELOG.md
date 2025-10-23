# Changelog

Todas as mudanças notáveis neste projeto serão documentadas neste arquivo.

O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/),
e este projeto adere a [Versionamento Semântico](https://semver.org/lang/pt-BR/).

## [1.5.0] - 2025-10-23

### Adicionado

- **Nova página Scripts**: Implementada página dedicada (scripts.html) com scripts Bash prontos para uso
- **Categorias de Scripts**:
  - Scripts Básicos: Fundamentos e exemplos introdutórios
  - Scripts de Automação: Automatização de tarefas de desenvolvimento
  - Scripts de Monitoramento: Ferramentas para monitoramento de sistemas
  - Scripts de Backup: Soluções automatizadas de backup
  - Scripts Utilitários: Ferramentas práticas do dia a dia
  - Scripts Avançados: Soluções complexas com tratamento de erros
- **Tema Scripts Personalizado**: Design com cor característica (#9b59b6)
- **Exemplos Práticos**: Scripts completos e funcionais para uso real
- **Boxes de Código**: Destaque para blocos de código com sintaxe colorida
- **Segurança em Destaque**: Alertas para boas práticas de segurança

### Scripts Implementados

- **Hello World com Argumentos**: Demonstração de uso de argumentos
- **Calculadora Simples**: Operações matemáticas básicas
- **Auto-Commit Git**: Automação de commits frequentes
- **Setup de Projeto Node.js**: Criação automática de estrutura
- **Monitor de Recursos**: Monitoramento em tempo real do sistema
- **Verificador de Serviços**: Status de serviços essenciais
- **Backup com Rotação**: Sistema de backup automático
- **Backup MySQL**: Backup especializado para bancos de dados
- **Organizador de Downloads**: Classificação automática de arquivos
- **Gerador de Senhas**: Criação de senhas seguras
- **Analisador de Logs**: Monitoramento de logs em tempo real
- **Deploy com Rollback**: Deploy automático com capacidade de rollback

### Melhorias

- **Navegação Completa**: Adicionado link 📜 Scripts em todas as páginas
- **Menu Integrado**: Navegação fluida entre Bash, Git, Docker e Scripts
- **Design Consistente**: Página Scripts mantém identidade visual do projeto
- **Experiência do Usuário**: Scripts organizados por categoria e dificuldade

### Detalhes Técnicos

- **HTML**: Estrutura semântica com microdados para scripts
- **CSS**: Estilos consistentes com tema roxo para scripts
- **Alpine.js**: Navegação reativa mantida
- **Segurança**: Alertas para práticas seguras de scripting

---

## [1.4.0] - 2025-10-23

### Adicionado

- **Implementação Alpine.js**: Migrado de JavaScript vanilla para Alpine.js em todas as páginas
- **CDN Alpine.js**: Adicionado script defer do Alpine.js no cabeçalho de todas as páginas
- **Sintaxe Declarativa**: Uso de diretivas Alpine.js para manipulação do DOM
- **Reatividade Moderna**: Gerenciamento de estado com x-data e x-init

### Melhorias

- **Código Reduzido**: Redução significativa no código JavaScript necessário
- **Performance Otimizada**: Melhor performance com reatividade otimizada
- **Manutenibilidade**: Código mais limpo e fácil de entender
- **Consistência**: Todas as páginas usando o mesmo padrão Alpine.js
- **Navegação Aprimorada**: Toggle do menu mobile mais eficiente com classes condicionais
- **Scroll Dinâmico**: Detecção de scroll com x-init para melhor responsividade

### Detalhes Técnicos

- **x-data**: Gerenciamento de estado para menu mobile e scroll
- **x-init**: Inicialização de event listeners para scroll
- **:class**: Classes condicionais para estados dinâmicos
- **@click**: Event handlers simplificados para toggle do menu
- **Alpine Components**: Estrutura mais limpa com componentes reativos

### Páginas Atualizadas

- **index.html**: Menu principal com Alpine.js
- **git.html**: Página Git com navegação reativa
- **docker.html**: Página Docker com navegação reativa

---

## [1.3.0] - 2025-10-22

### Adicionado

- **Página Dedicada Docker**: Nova página (docker.html) com comandos Docker essenciais organizados por categorias
- **Categorias de Comandos Docker**:
  - Informações Básicas
  - Containers
  - Imagens
  - Logs e Monitoramento
  - Execução e Interação
  - Limpeza e Manutenção
  - Docker Compose
  - Redes e Volumes
  - Troubleshooting
- **Tema Docker Personalizado**: Design com cor característica do Docker (#2496ed)
- **Alertas de Segurança**: Boxes de aviso para comandos perigosos (ex: docker system prune -a --volumes)
- **Dicas de Otimização**: Boxes com dicas para troubleshooting e melhores práticas

### Melhorias

- **Menu Principal**: Adicionado link 🐳 Docker no menu de navegação da página principal
- **Menu Git**: Adicionado link 🐳 Docker no menu de navegação da página Git
- **Navegação Completa**: Navegação fluida entre todas as páginas (index, git, docker)
- **Estrutura Modular**: Conteúdo organizado por categorias para fácil consulta
- **Experiência de Navegação**: Navegação fluida entre páginas diferentes

### Detalhes Técnicos

- **HTML**: Página independente com estrutura semântica otimizada
- **CSS**: Estilos consistentes com design system existente e tema Docker
- **JavaScript**: Funcionalidades de navegação responsiva mantidas
- **Comandos Docker**: Extraídos e organizados do documento comandos-uteis.pdf

---

## [1.2.0] - 2025-10-22

### Adicionado

- **Página Dedicada Git**: Nova página (git.html) com comandos Git avançados organizados por categorias
- **Categorias de Comandos Git**:
  - Status e Histórico
  - Branches Avançadas
  - Merge e Rebase
  - Busca e Investigação
  - Tags e Releases
  - Stash Avançado
  - Reset e Restore
  - Remote e Colaboração
- **Design Consistente**: Página Git mantém o mesmo design visual da página principal
- **Navegação Entre Páginas**: Link "Voltar para página principal" e menu de navegação atualizado
- **Alertas de Segurança**: Boxes de aviso para comandos perigosos (ex: git reset --hard)
- **Dicas Informativas**: Boxes com dicas e melhores práticas para comandos específicos

### Melhorias

- **Menu Principal**: Adicionado link 🔀 Git no menu de navegação da página principal
- **Estrutura Modular**: Conteúdo organizado por categorias para fácil consulta
- **Experiência de Navegação**: Navegação fluida entre páginas diferentes

### Detalhes Técnicos

- **HTML**: Página independente com estrutura semântica otimizada
- **CSS**: Estilos consistentes com design system existente
- **JavaScript**: Funcionalidades de navegação responsiva mantidas
- **Comandos Git**: Extraídos e organizados do documento comandos-uteis.pdf

## [1.1.0] - 2025-10-22

### Adicionado

- **Menu de Navegação Rápida Fixo**: Implementado menu de navegação no topo da página que permanece visível durante o scroll
- **Navegação por Seções**: Links diretos para as principais seções do cheatsheet:
  - 📚 Comandos
  - 🟢 Iniciante
  - 🟡 Intermediário
  - 🔴 Avançado
  - 📜 Scripts
  - 🐳 Docker
  - ⌨️ Atalhos
- **Design Responsivo**: Menu adaptável para dispositivos móveis com hamburger menu
- **Scroll Suave**: Implementada navegação suave ao clicar nos links do menu
- **Destaque de Seção Ativa**: Link da seção atual é destacado visualmente no menu
- **Efeitos Visuais**: Menu muda de aparência ao rolar a página (background mais escuro e sombra)

### Melhorias

- **Experiência do Usuário**: Navegação mais intuitiva e rápida entre as seções
- **Acessibilidade**: Melhorada a navegação para usuários de dispositivos móveis
- **Feedback Visual**: Indicadores visuais claros de qual seção está sendo visualizada
- **Performance**: Otimizado o JavaScript para melhor desempenho durante o scroll

### Detalhes Técnicos

- **HTML**: Adicionada estrutura semântica `<nav>` com classes CSS específicas
- **CSS**: Implementados estilos com:
  - Posicionamento fixo (`position: fixed`)
  - Backdrop filter para efeito de desfoque
  - Transições suaves para animações
  - Media queries para responsividade
- **JavaScript**: Funcionalidades implementadas:
  - Intersection Observer API para detectar seções visíveis
  - Event listeners para scroll e cliques
  - Toggle menu para dispositivos móveis
  - Scroll behavior suave

### Próximas Melhorias Planejadas

- [ ] Busca instantânea de comandos
- [ ] Modo escuro/claro
- [ ] Exportação de seções como PDF
- [ ] Favoritos para comandos mais usados
- [ ] Histórico de navegação

---

## [1.0.0] - 2025-01-01

### Adicionado

- Versão inicial do Bash Cheatsheet 2025
- Mais de 200 comandos organizados por nível de dificuldade
- Interface web moderna e responsiva
- Seções: Iniciante, Intermediário, Avançado
- Comandos Docker bônus
- Atalhos de teclado essenciais
- Estatísticas do mercado de trabalho
- Licença MIT

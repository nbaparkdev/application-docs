Fleet Control** é uma solução abrangente de gerenciamento de frota desenvolvida para a **Controle de Frota**. Combina uma aplicação web moderna em 
React com capacidades Nativas Mobile via Capacitor, permitindo o gerenciamento eficiente de viagens, disponibilidade de veículos e desempenho dos motoristas.

> **Principais Funcionalidades**: Análise com IA, Rastreamento em Tempo Real, Dashboard Administrativo e Segurança Biométrica.

---

## 📱 Mobile & Web (PWA)

Esta aplicação foi construída como um **Progressive Web App (PWA)** e empacotada com **Capacitor** para uma experiência nativa em Android/iOS.

### Funcionalidades Nativas Mobile (Android/iOS)
- **Desbloqueio Biométrico**: Acesso seguro usando Impressão Digital/FaceID via `@capgo/capacitor-native-biometric`.
- **Geolocalização em Segundo Plano**: Rastreia coordenadas da rota com precisão mesmo quando o app está em segundo plano.
- **Feedback Háptico**: Resposta tátil para ações de sucesso/erro.
- **Gerenciamento de Estado do App**: Bloqueio automático de segurança quando o app vai para segundo plano.

### Funcionalidades Web
- **Design Responsivo**: Funciona em navegadores Desktop, Tablet e Mobile.
- **Capacidade Offline**: Service workers armazenam recursos em cache para uso offline.
- **Instalável**: Pode ser instalado na tela inicial através do navegador.

---

## 🛠️ Módulos Funcionais

### 1. App do Usuário (Motorista)
- **Registro de Viagem**: Fluxo fácil de "Iniciar/Parar" com validação de hodômetro (KM).
- **Itinerário Inteligente**: A IA analisa a descrição do destino para categorizar a viagem.
- **Histórico**: Registro pessoal de todas as viagens passadas com indicadores de status.
- **Gerenciamento de Tarefas**: "Lista de Tarefas" integrada para motoristas com níveis de prioridade e status tipo Kanban.
- **Seleção de Veículo**: Visualização ao vivo de veículos disponíveis (não bloqueados).

### 2. Dashboard Administrativo (Desktop)
Acessado via atalho secreto (`Ctrl + Shift + A`) ou Login de Admin.
- **Visão Geral de KPIs**: Total de KM, Total de Viagens, Usuários Ativos e contagem de Viagens em Andamento.
- **Mapa em Tempo Real**: Mapa em tela cheia mostrando a última localização conhecida dos veículos ativos.
- **Feed de Atividade ao Vivo**: Fluxo em tempo real de viagens iniciando, terminando e logins de usuários.
- **Ranking de Motoristas**: Tabela de classificação gamificada baseada em KM rodados.
- **Gerenciamento de Veículos**: Registrar, editar, bloquear/desbloquear veículos (ex: para manutenção).
- **Atribuição de Tarefas**: Criar e atribuir tarefas a motoristas específicos.
- **Relatórios**: Tabela de dados filtrável com capacidade de **Exportação CSV**.
- **Configurações do Sistema**: Configurar marca da empresa, URLs de Webhook e preferências gerais.

### 3. Inteligência Artificial (Google Gemini)
- **Resumos Semanais**: Gera relatórios em linguagem natural sobre a eficiência da frota.
- **Análise de Itinerário**: Etiqueta automaticamente padrões de uso corporativo vs. pessoal.
- **Detecção de Anomalias**: Sinaliza quilometragens ou durações incomuns (planejado).




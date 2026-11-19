# 🎵 Projeto Sonora — Streaming de Áudio Sem Copyright (CEUB)

![HTML5](https://img.shields.io/badge/HTML5-Semântico-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-Grid%20%26%20Flexbox-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla%20ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Firebase](https://img.shields.io/badge/Firebase-Realtime%20Database-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Status](https://img.shields.io/badge/Deploy-GitHub%20Pages-D80073?style=for-the-badge)

Plataforma web responsiva de streaming de áudio livre de direitos autorais (*royalty-free* / Creative Commons), desenvolvida sob a identidade visual institucional do **Centro Universitário de Brasília (CEUB)** e projetada conforme as **10 Heurísticas de Usabilidade de Jakob Nielsen**.

🔗 **Acesse a aplicação online:** [https://gabriel-sa1.github.io/Sonora_DDI/](https://gabriel-sa1.github.io/Sonora_DDI/)  

---

## 📋 Visão Geral

O **Sonora** combina os melhores padrões de interação do **Spotify** (barra lateral fixa para biblioteca/playlists e player inferior persistente) e do **YouTube Music** (filtros superiores rápidos por categoria/humor, descoberta visual e fila dinâmica *"A Seguir"*), oferecendo um ambiente livre de anúncios e voltado à produtividade acadêmica.

O projeto foi especificado seguindo os rigorosos padrões de **Engenharia de Requisitos de Ian Sommerville** (Documento de Análise de Negócio — DAN e Documento de Definição do Sistema — DDS) e construído de forma iterativa por meio da metodologia **Vibe Coding**.

---

## ✨ Funcionalidades Principais

* **🎧 Motor de Áudio Híbrido (`HybridAudioEngine`):** Reprodução real de arquivos `MP3`, `OGG` e `WAV` via HTML5 `<audio>` (hospedados na pasta `musicas/` do repositório ou em URLs externas) com *fallback* automático para um sintetizador polifônico em tempo real via **Web Audio API** (Lo-Fi, Ondas Alfa 432Hz, Piano Minimalista e Synthwave).
* **⏯️ Player Persistente Completo:** Controles contínuos de *Play/Pause*, *Anterior/Próxima* (respeitando o contexto da playlist ativa), *Ordem Aleatória*, *Repetir* em 3 estados (Desativado → Repetir Faixa → Repetir Playlist), barra de progresso clicável, controle de volume/mudo e gaveta lateral de fila **"A Seguir"**.
* **📚 Biblioteca Visual em Quadradinhos & Playlists:** Visualização em grade de cards quadrados para **Músicas Favoritas** e playlists personalizadas (com mosaico automático $2\times2$ de capas), permitindo criar, renomear, reordenar faixas e excluir coleções com confirmação preventiva e opção **Desfazer**.
* **🔍 Busca em Tempo Real & Descoberta Inteligente:** Filtragem instantânea por título, artista ou gênero combinada com chips de humor (*Todos, Foco & Estudo, Lo-Fi, Eletrônica, Podcasts CEUB e Relaxar*) e recomendações dinâmicas sem repetir faixas tocadas recentemente.
* **⏱️ Modo Foco Acadêmico CEUB (Pomodoro):** Ambiente imersivo livre de distrações com temporizador Pomodoro integrado (**25 min** Foco, **5 min** Pausa Curta e **15 min** Pausa Longa) sincronizado com trilhas de concentração.
* **🛠️ Painel Administrativo do Gerente + Firebase:** Área protegida por autenticação para curadores cadastrarem, editarem e excluírem faixas do catálogo público em tempo real via **Firebase Realtime Database**, com suporte direto aos arquivos da pasta `musicas/`.
* **🌓 Identidade Visual Institucional CEUB (Modo Escuro & Modo Claro):** Paleta oficial em roxo institucional (`#14041D` / `#2E003E` / `#3B0054`) e magenta (`#D80073`) com alternância de tema e contraste acessível **WCAG AA**.

---

## 🧭 Conformidade com as 10 Heurísticas de Nielsen

| Heurística | Aplicação no Projeto Sonora |
| :--- | :--- |
| **H1. Visibilidade do Status** | Notificações *toast* empilhadas (máx. 3 simultâneas), equalizador animado na faixa ativa, barra de progresso e indicador de conexão Firebase. |
| **H2. Correspondência com o Mundo Real** | Ícones universais de mídia e rotulagem natural em português do Brasil. |
| **H3. Controle e Liberdade do Usuário** | Fechamento de modais/fila com `ESC`, botão `← Biblioteca` e ação **Desfazer** após exclusões. |
| **H4. Consistência e Padrões** | Estrutura fixa de barra lateral, cabeçalho global e player inferior persistente em todas as telas. |
| **H5. Prevenção de Erros** | Validação obrigatória de campos, bloqueio de botões em formulários vazios e confirmação antes de excluir playlists. |
| **H6. Reconhecimento vs. Memorização** | Histórico *Tocados Recentemente*, capas visuais e mosaico $2\times2$ automático nas playlists. |
| **H7. Flexibilidade e Eficiência** | Chips de filtro rápido, botão *Outras* nas recomendações e atalho `Barra de Espaço` para Play/Pause. |
| **H8. Estética e Design Minimalista** | Cards limpos com controles secundários revelados sob demanda (*hover*). |
| **H9. Recuperação de Erros** | Telas vazias orientativas e troca automática para sintetizador caso uma URL externa falhe. |
| **H10. Ajuda e Documentação** | *Tooltips* explicativos nos controles e modal dedicado **? Ajuda** com guia de atalhos. |

---

## 🗂️ Estrutura do Repositório

```text
Sonora_DDI/
├── index.html      # Aplicação SPA completa (HTML5 Semântico + CSS3 Design System + JS ES6+)
├── musicas/        # Diretório de faixas .mp3 livres de copyright servidas pelo GitHub Pages
├── capas/          # Imagens locais de capas de álbuns/playlists (opcional)
└── README.md       # Documentação oficial do projeto

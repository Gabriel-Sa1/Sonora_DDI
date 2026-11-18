# 🎵 Projeto Sonora — Plataforma Web de Streaming de Áudio (CEUB)

Aplicação web responsiva de streaming de áudio **sem direitos autorais (royalty-free / Creative Commons)** desenvolvida na disciplina **Desenvolvimento de Interfaces (HTML, CSS e JavaScript)** do **Centro Universitário de Brasília (CEUB)**, seguindo o Documento de Análise de Negócio (DAN), o Documento de Definição do Sistema (DDS) e as **10 Heurísticas de Usabilidade de Jakob Nielsen**.

---

## 🔗 Acesso à Aplicação Hospedada (GitHub Pages)

👉 **Acesse o sistema online:** [https://gabriel-sa1.github.io/projeto/](https://gabriel-sa1.github.io/projeto/)

---

## ✨ Principais Funcionalidades

- **Interface Híbrida (Spotify + YouTube Music):** Barra lateral fixa para navegação e biblioteca, filtros superiores rápidos por humor/categoria e player inferior persistente.
- **Identidade Visual Institucional CEUB & Temas:** Paleta oficial em Roxo Profundo (`#2E003E`) e Magenta (`#D80073`) com alternância entre **Modo Escuro** e **Modo Claro**.
- **Motor de Áudio Híbrido Real:** Reprodução via HTML5 `<audio>` (arquivos `.mp3` da pasta `musicas/` e URLs externas) combinada a um sintetizador nativo em **Web Audio API** (Lo-Fi, Ondas Alfa 432Hz, Piano Minimalista e Synthwave).
- **Recomendações Inteligentes & Histórico:** Sugestões dinâmicas filtradas por categoria sem repetir faixas de *Tocados Recentemente*.
- **Sua Biblioteca em Quadradinhos & Playlists:** Visualização em grade de cards quadrados para *Músicas Favoritas* e playlists personalizadas (com mosaico automático 2×2 de capas, criação, edição e exclusão com opção *Desfazer*).
- **Modo Foco Acadêmico CEUB:** Temporizador Pomodoro integrado (25 min foco / 5 min pausa curta / 15 min pausa longa) sincronizado com trilhas de concentração.
- **Painel do Gerente em Nuvem:** Área administrativa para cadastro, edição e remoção de faixas do catálogo global com sincronização em tempo real via **Firebase Realtime Database**.
- **10 Heurísticas de Nielsen:** Atalhos de teclado (`Espaço` para Play/Pause, `ESC` para fechar modais), notificações *toast*, tooltips contextuais e guia rápido de ajuda.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 Semântico** e atributos de acessibilidade ARIA
- **CSS3 Moderno** (CSS Grid, Flexbox, Variáveis `:root`, Design Responsivo)
- **JavaScript Vanilla (ES6+)**
- **Web Storage API (`localStorage`) & `IndexedDB`** (persistência de favoritos, playlists, histórico e preferências)
- **Web Audio API** (síntese sonora em tempo real)
- **Firebase Realtime Database (REST API)** (catálogo global em nuvem)
- **Git & GitHub Pages** (versionamento e hospedagem)

---

## 📁 Estrutura do Repositório

```text
projeto/
├── index.html          # Aplicação web completa (HTML5 + CSS3 + JavaScript ES6+)
├── musicas/            # Arquivos de áudio .mp3 livres de copyright servidos pelo GitHub Pages
└── README.md           # Documentação do projeto e link ativo de acesso

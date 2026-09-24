# 📝 PawnForge for Notepad++

<p align="center">
  <strong>Modern AMX Mod X Pawn IDE features for Notepad++ (x64)</strong><br>
  Language Server Protocol (LSP), Autocomplete, Go to Definition, Modern Dual-Theme Syntax & 1-Click Compiler.
</p>

<p align="center">
  <a href="https://github.com/NiceFeatures/pawnforge-npp/releases">
    <img alt="GitHub Release" src="https://img.shields.io/github/v/release/NiceFeatures/pawnforge-npp?style=for-the-badge&color=22c55e">
  </a>
  <img alt="Notepad++ 64-bit" src="https://img.shields.io/badge/Notepad%2B%2B-v8.7%2B%20(x64)-blue?style=for-the-badge">
  <img alt="AMX Mod X 1.10" src="https://img.shields.io/badge/AMX%20Mod%20X-1.10%20%7C%20ReAPI-orange?style=for-the-badge">
  <img alt="License" src="https://img.shields.io/badge/License-GPL--3.0-purple?style=for-the-badge">
</p>

---

## 🌟 Recursos / Features

- ⚡ **Language Server Protocol (LSP):** Powered by the standalone [pawnforge-lsp](https://github.com/NiceFeatures/pawnforge-lsp) core engine (iniciado automaticamente via **NppLspClient** v0.0.40 x64).
- 💡 **Hover & Documentation:** Passe o cursor sobre qualquer função, macro ou constante AMXX / ReAPI para ver sua documentação completa e parâmetros com formatação Markdown via WebView2.
- 🔍 **Navegação & Go to Definition:** Pule direto para declarações e funções via clique direito no editor ou atalhos de teclado.
- 🎨 **Sintaxe Moderna com Modo Escuro Automático:**
  - **Dark Mode:** Paleta moderna inspirada no VS Code Dark+ e PawnForge (cores personalizadas para tags `Float:`, `bool:`, enums ReAPI, pré-processadores).
  - **Light Mode:** Visual limpo e de alto contraste para o tema claro do Notepad++.
  - Alterna automaticamente ao ligar o Modo Escuro no Notepad++!
- 🔨 **Compilação em 1 Clique (`F6` / `Ctrl + F6`):** Integração rápida via **NppExec** com salto direto para linhas de erro (ao dar duplo-clique no erro do console, o Notepad++ salta diretamente para a linha no código-fonte).

---

## 🚀 Instalação Rápida / Quick Installation (1 Minuto)

1. Baixe o arquivo **`pawnforge-npp-vX.Y.Z.zip`** na aba [Releases](https://github.com/NiceFeatures/pawnforge-npp/releases).
2. Extraia o conteúdo diretamente no diretório do Notepad++:
   - **Instalação Padrão (Recomendado):**  
     Copie as pastas `plugins`, `userDefineLangs`, `contextMenu.xml` para `%APPDATA%\Notepad++` e o arquivo `bin\pawnforge-lsp.exe` para `C:\Program Files\Notepad++\`.
   - **Notepad++ Portable:**  
     Extraia todos os arquivos diretamente na pasta raiz do seu Notepad++ Portable.
3. Abra ou reinicie o Notepad++. O servidor LSP iniciará automaticamente para arquivos `.sma` e `.inc`!

---

## 🌙 Como Ativar o Modo Escuro (Dark Mode)

1. No menu superior do Notepad++, acesse:
   **Configurações** (`Settings`) ➔ **Preferências...** (`Preferences...`) ➔ **Modo Escuro** (`Dark Mode`).
2. Marque a caixa **Ativar modo escuro** (`Enable dark mode`).
3. Clique em **Fechar**.
4. O tema Pawn mudará instantaneamente para a sintaxe escura moderna!

---

## 🔨 Onde e Como Compilar (`amxxpc`)

A compilação é gerenciada pelo plugin **NppExec**:
- Pressione **`F6`**: abre a janela de execução com o script `Compile AMXX` já selecionado. Basta pressionar **Enter** (ou clicar em **OK**).
- Pressione **`Ctrl + F6`**: recompila imediatamente o arquivo atual sem nem abrir a janela de diálogo!
- Ou acesse pelo menu: **Plugins** ➔ **NppExec** ➔ **Execute NppExec Script...**.
- O console abre na parte inferior com as mensagens do compilador.
- **Dica:** Dê um **duplo clique** em qualquer linha de erro no console para que o Notepad++ vá instantaneamente até a linha exata no seu `.sma`!

---

## 🔍 Como Navegar (Ir para Definição)

> 💡 **Nota sobre `Ctrl + Clique`:**  
> No Notepad++ (motor Scintilla), o atalho `Ctrl + Clique` é nativamente reservado para **seleção com múltiplos cursores** e não pode ser interceptado por plugins.  
> Por isso, a navegação para a definição é feita de duas maneiras muito fáceis:

1. **Pelo Botão Direito (Menu de Contexto):**
   - Clique com o botão direito sobre o nome de qualquer função ou variável e selecione **`Ir para Definição (Go to Definition)`**!
2. **Pelo Teclado:**
   - Use o atalho **`Alt + G`** ou configure **`F12`** em *Configurações ➔ Atalhos... ➔ Comandos de plug-in ➔ NppLspClient ➔ Goto definition*.

---

## ⌨️ Atalhos Úteis

| Atalho / Shortcut | Ação / Action | Descrição |
| :--- | :--- | :--- |
| **`Ctrl + Espaço`** | **Autocomplete** | Exibe nativas, constantes e assinaturas AMXX / ReAPI |
| **Botão Direito ➔ Ir para Definição** | **Go to Definition** | Pula para a definição/declaração da função |
| **`F6`** | **Compilar Plugin (`amxxpc`)** | Abre o diálogo para compilar o arquivo `.sma` atual |
| **`Ctrl + F6`** | **Recompilar Imediato** | Executa a última compilação sem exibir diálogo |
| **Duplo-clique no erro** | **Saltar para o Erro** | Salta direto para a linha do erro no arquivo fonte |

---

## 📜 Licença

Distribuído sob a licença **GPL-3.0**. Veja [LICENSE.txt](LICENSE.txt) para detalhes.

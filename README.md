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

- ⚡ **Language Server Protocol (LSP):** Powered by the standalone [pawnforge-lsp](https://github.com/NiceFeatures/pawnforge-lsp) core engine via **NppLspClient**.
- 💡 **Intelligent Autocomplete (`Ctrl + Space`):** Complete prototype parameters and rich inline documentation for AMX Mod X 1.8.2 / 1.9 / 1.10 and **ReAPI**.
- 🎯 **Go to Definition (`Alt + G` / `F12`):** Jump instantly to any native, stock, macro, or function across all your `.sma` and `.inc` includes.
- 🔍 **Find References (`Alt + Shift + G`):** Find all symbols and callback usages across files.
- 🎨 **Modern Dual-Theme UDL (User Defined Language):**
  - **Dark Mode:** Modern palette inspired by VS Code Dark+ and PawnForge (custom colors for tags `Float:`, `bool:`, ReAPI enums, preprocessors).
  - **Light Mode:** High-contrast crisp styling for standard Notepad++ light theme.
  - Switches automatically when toggling Dark Mode in Notepad++!
- 🔨 **1-Click Compilation (`F6`):** Fast build integration via **NppExec** with clickable error lines (double-click in the console jumps directly to the line in your source code).

---

## 🚀 Instalação Rápida / Quick Installation (1 Minuto)

1. Baixe o arquivo **`pawnforge-npp-vX.Y.Z.zip`** na aba [Releases](https://github.com/NiceFeatures/pawnforge-npp/releases).
2. Extraia o conteúdo diretamente na pasta do Notepad++:
   - **Instalação Padrão (Recomendado):**  
     Extraia dentro de `%APPDATA%\Notepad++` ou em `C:\Program Files\Notepad++`
   - **Notepad++ Portable:**  
     Extraia diretamente na raiz da pasta do seu Notepad++ Portable.
3. Abra ou reinicie o Notepad++. Pronto!

> ℹ️ **Estrutura extraída:**
> ```text
> Notepad++/
> ├── bin/
> │   └── pawnforge-lsp.exe        (Servidor LSP standalone)
> ├── userDefineLangs/
> │   ├── Pawn_Dark.udl.xml        (Sintaxe moderna Dark Mode)
> │   └── Pawn_Light.udl.xml       (Sintaxe clássica Light Mode)
> └── plugins/
>     ├── NppLspClient/           (Plugin LSP para Notepad++)
>     ├── NppExec/                (Plugin de compilação 1-clique)
>     └── Config/                 (Configurações pré-definidas)
> ```

---

## ⌨️ Atalhos do Teclado / Keyboard Shortcuts

| Atalho / Shortcut | Ação / Action | Descrição |
| :--- | :--- | :--- |
| **`Ctrl + Espaço`** | **Autocomplete** | Sugestões com documentação de nativas AMXX e ReAPI |
| **`Alt + G`** ou **`F12`** | **Go to Definition** | Pula instantaneamente para a declaração/função |
| **`Alt + Shift + G`** | **Find References** | Lista todas as referências do símbolo selecionado |
| **`F6`** | **Compilar Plugin (`amxxpc`)** | Executa a compilação do arquivo `.sma` ativo |
| **Duplo-clique no erro** | **Navegar para o Erro** | No console do Notepad++, dá duplo clique para ir à linha |

---

## ⚙️ Configuração do Compilador (`amxxpc.exe`)

O script de compilação (`F6`) já vem configurado para o compilador padrão no Desktop (`compiler\amxxpc.exe`).

Caso seu compilador esteja em outro diretório:
1. No Notepad++, pressione **`F6`**.
2. No menu suspenso, selecione **`Compile AMXX`**.
3. Ajuste o caminho do `amxxpc.exe` para a pasta do seu servidor / compilador.
4. Clique em **`Save`** e em **`OK`**.

---

## 📜 Licença

Distribuído sob a licença **GPL-3.0**. Veja [LICENSE.txt](LICENSE.txt) para detalhes.

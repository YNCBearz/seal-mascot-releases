# Seal Mascot

macOS / Windows 桌面小精靈：每個 Claude Code、Codex 對話一隻，顯示對話狀態（工作中、等待回覆、完成、錯誤），點一下就切回對應的終端機分頁或 App。

這個 repo 只放安裝檔，請到 [Releases](https://github.com/YNCBearz/seal-mascot-releases/releases/latest) 取得最新版。

## 安裝

**macOS**（終端機，Apple Silicon 與 Intel 皆可）

```sh
curl -fsSL https://github.com/YNCBearz/seal-mascot-releases/releases/latest/download/install.sh | bash
```

**Windows**（PowerShell，x64）

```powershell
irm https://github.com/YNCBearz/seal-mascot-releases/releases/latest/download/install.ps1 | iex
```

- 重新執行同一行指令即可更新到最新版，設定與對話資料會保留。
- 安裝後在 App 的設定頁按「安裝／更新」整合 Claude Code／Codex，然後重啟 CLI。
- macOS 安裝在 `/Applications`；Windows 安裝在目前使用者，不需系統管理員權限。
- 從舊版 Agent Mascot 更新：直接執行上面的指令，會自動移除舊 App，並保留角色設定、對話與 hook 整合。
- App 尚未簽章。直接用瀏覽器下載 `.dmg`／`.exe` 會被 macOS Gatekeeper 或 Windows SmartScreen 攔下，建議使用上面的指令安裝。

## 解除安裝

- **macOS**：從系統匣選「退出」，將 `/Applications/Seal Mascot.app` 移到垃圾桶。
- **Windows**：從「設定 → 應用程式」解除安裝 Seal Mascot。

解除安裝前，可先在設定頁按「移除」，清除 Claude Code／Codex 的 hook 整合。

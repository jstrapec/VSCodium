## Install custom highlighting for VS codium

This is my custom extensions for simple highliting for notes. It applies as default language for unsaved files and for all .txt files 

### Installation

1. Download ZIP file. 

2. Unzip it. 

3. Copy **txt-syntax-highlighting-0.0.1** directory to directory where VS Codium stores files for extensions

  - For app installed as deb package or as snap
    ~/.vscode-oss/extensions/

  - For app installed as flatpak
    ~/.var/app/com.vscodium.codium/data/vscode-oss/extensions/

  - For Windows
    C:\Users\<YourUsername>\.vscode-oss\extensions


        `cp -r txt-syntax-highlighting-0.0.1 ~/.vscode-oss/extensions/`

4. Copy textMateRules from settings.json to your configuration. You can access it by pressing ctrl+shift+p and typing "Open User Settings (JSON)"

````
   "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "scope": "markup.heading",
                "settings": {
                    "foreground": "#FFA500",
                    "fontStyle": "bold"
                }
                ...
                ..
                .
````

  There is also my preffred configuration for VS Codium.

5. Changes should be applied immediatly. You can check if you see this extension between your extension, by pressing ctrl+shift+x. If not restart VS codium

# VidConvertX

# --- 1. DOWNLOAD E INSTALAÇÃO DO APLICATIVO ---
# Este bloco baixa o arquivo zip, extrai na pasta .config, remove o zip e cria o atalho no menu.
```python
cd ~ && \
wget -O vidconvertx.zip https://github.com/Henri-OS/VidConvertX/raw/refs/heads/main/vidconvertx.zip && \
unzip -qo vidconvertx.zip -d ~/.config && \
rm vidconvertx.zip && \
wget -P ~/.local/share/applications https://raw.githubusercontent.com/Henri-OS/VidConvertX/refs/heads/main/vidconvertx.desktop && \
echo "✅ VidConvertX extraído em ~/.config e atalho criado em ~/.local/share/applications"
```
# --- 2. INSTALAÇÃO DE DEPENDÊNCIAS ---
# Este bloco instala o motor de conversão (FFmpeg) e a interface gráfica (PyQt6) via repositório oficial (APT).
```python
sudo apt update && sudo apt install -y ffmpeg python3-pyqt6
```

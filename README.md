# 🕵️ OSINT Tools

Script Bash para coleta automatizada de informações OSINT sobre um domínio. Ele gera relatórios em texto e HTML com dados como IP, WHOIS, portas abertas, links indexados via Google Dorks e metadados de arquivos PDF, DOCX e imagens JPEG.

---

## 📌 Funcionalidades

- ✅ Resolução de IP do domínio
- ✅ Coleta de informações WHOIS
- ✅ Scan de portas com `nmap`
- ✅ Coleta de links indexados com Google Dorks usando `lynx`
- ✅ Download e extração de metadados de arquivos (PDF, DOCX, JPEG)
- ✅ Geração de relatório em `.txt` e `.html`

---

## ⚙️ Pré-requisitos

Certifique-se de ter os seguintes pacotes instalados:

```bash
sudo apt install -y dnsutils whois nmap lynx wget exiftool poppler-utils
```

Ou, para sistemas Arch Linux:

```bash
sudo pacman -S bind whois nmap lynx wget perl-image-exiftool poppler
```

---

## 🚀 Como usar

```bash
chmod +x osint.sh
./osint.sh exemplo.com
```

O script irá gerar dois arquivos de saída:

- `osint_report_<timestamp>.txt`
- `osint_report_<timestamp>.html`

Além disso, criará uma pasta `downloads/` com arquivos baixados para extração de metadados.

---

## 📁 Estrutura do Projeto

```
osint/
├── osint.sh                  # Script principal
├── downloads/                # Arquivos baixados para análise
├── osint_report_*.txt        # Relatório em texto
└── osint_report_*.html       # Relatório em HTML
```

---

## 📸 Exemplo de execução

**Terminal:**
```bash
[+] Resolvendo IP do domínio...
IP: 192.0.2.1

[+] Coletando informações WHOIS...
[...]
```

**HTML:**  
Relatório formatado com seções organizadas (IP, WHOIS, links indexados e metadados).

---

## ⚠️ Aviso legal

> Este script é destinado apenas a fins educacionais e auditorias autorizadas. **Não execute em domínios sem permissão expressa.** O uso indevido pode violar leis locais e internacionais.

---

# 🔑 Keylogger Educacional

> Projeto desenvolvido para fins **estritamente didáticos**, como parte de estudos em segurança digital. Não realiza envio de dados para a internet e opera exclusivamente na máquina local.

---

## 📋 Sobre o projeto

Este keylogger foi criado para demonstrar, em ambiente controlado, como ferramentas de monitoramento de teclado funcionam — e por que representam um risco real de segurança. Todo o registro é feito localmente em um arquivo `.txt`, sem qualquer comunicação externa.

---

## ⚙️ Funcionalidades

- Captura de teclas normais (letras, números, símbolos) e teclas especiais (Enter, Backspace, F1–F12, setas, etc.)
- Detecção do aplicativo em foco no momento do pressionamento (Windows com suporte completo; Linux/macOS com fallback)
- Registro com timestamp em arquivo `log_keylogger.txt` na mesma pasta do script
- Exibição simultânea no terminal
- Encerramento seguro via atalho **CTRL + ESC**

---

## 🗂️ Estrutura do log

Cada linha registrada segue o formato:

```
[HH:MM:SS]  ⌨️  Tecla normal   → 'a'   | App: chrome
[HH:MM:SS]  🔑 Tecla especial → [ENTER]   | App: chrome
[HH:MM:SS]  📱 App em foco → [notepad]
```

---

## 🚀 Como executar

**Pré-requisitos:**

```bash
pip install pynput psutil
```

**Execução:**

```bash
python Python_Keylogger.py
```

Para encerrar, pressione **CTRL + ESC**. O log será salvo automaticamente em `log_keylogger.txt`.

---

## 🧰 Tecnologias utilizadas

| Biblioteca | Uso |
|---|---|
| `pynput` | Captura de eventos de teclado |
| `psutil` | Identificação do processo em foco |
| `ctypes` | Acesso à API do Windows para janela ativa |
| `datetime` | Timestamps nos registros |
| `os` / `sys` | Caminhos e informações do sistema |

---

## ⚠️ Aviso legal

Este projeto existe **somente para fins educacionais**. O uso de keyloggers em dispositivos sem a autorização explícita do proprietário é **ilegal** e antiético. O autor não se responsabiliza por qualquer uso indevido deste código.

---

## 👤 Autor

**Leandro Santos Rangel**  
Técnico em Desenvolvimento de Sistemas — Educação Profissional Paulista  
[LinkedIn](https://www.linkedin.com/in/leandro-santos-rangel) • [GitHub](https://github.com/leandrosantosrangel)

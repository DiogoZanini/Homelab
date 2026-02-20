# Homelab
Índice da minha infraestrutura de estudo.

[**EN-US**](../README.md)

![network_diagram drawio](./homelab_network_diagram.png)

## Ambiente de Desenvolvimento

### Máquina Host
- [**VS Code IDE:**](https://github.com/DiogoZanini/VSCode-IDE-setup) Configuração do VSCode para desenvolvimento em C, Python e SQLite, estendendo o fluxo de trabalho do CS50.

### pfSense (Oracle VirtualBox)
- [**Gateway de Rede Virtual:**](https://github.com/DiogoZanini/pfSense) Gateway padrão da rede do laboratório virtual, responsável pelo roteamento e regras de firewall.

### Kali Linux (Oracle VirtualBox)
- [**Kali Linux Analyst Machine:**](https://github.com/DiogoZanini/Homelab) Máquina virtual Kali Linux para análise de segurança do ambiente homelab e desafios CTF em plataformas de estudo online.

### SanDisk USB Drive
- [**Tails Amnesic Incognito System:**](https://github.com/DiogoZanini/Portable-Linux-Tails) Configuração pessoal e notas operacionais para um ambiente de segurança amnésico em um pendrive.

## Roadmap

### 🛠️ Ferramentas Externas
- [x] Máquina Host: VS Code IDE + Oracle VirtualBox;
- [x] Tails Amnesic Incognito System (USB Inicializável);

### 🌐 Infraestrutura do Homelab
- [x] pfSense VM (Firewall/Roteador);

### 🔴 Red Team / Análise
- [x] Kali Linux VM (Análise de Segurança);

### 🎯 Superfície de Ataque (Alvos Vulneráveis)

**Aplicações Web:**
- [ ] OWASP Juice Shop;
- [ ] DVWA (Damn Vulnerable Web Application);

**Sistemas Vulneráveis:**
- [ ] Metasploitable;
- [ ] Metasploitable2;
- [ ] Metasploitable3-ub1404 (Ubuntu);
- [ ] Metasploitable3-win2k8 (Windows);

### 🪟 Ambiente Windows

**Laboratório Active Directory:**
- [ ] Windows Server 2025 + Active Directory;

**Estações de Trabalho:**
- [ ] Windows 11 (Produção);
- [ ] Windows 10;

**Sistemas Legados (EOL):**
- [ ] Windows 7;
- [ ] Windows Vista;
- [ ] Windows XP;

**Análise de Malware (Isolado):**
- [ ] Windows 11 - Laboratório de Análise de Malware (Snapshot)
  - Ferramentas: Wireshark, IDA, x32dbg, x64dbg, ProcMon, ProcExp, Ghidra, DIE, HxD

### 🐧 Ambiente Linux
- [ ] Debian VM:
  - Snapshot: OWASP Juice Shop
  - Snapshot: DVWA

### 🔵 Blue Team / Detecção
- [ ] Laboratório SOC;

## Solução de Problemas
Problemas comuns e suas soluções.

[Guia completo de solução de problemas](./docs/TROUBLESHOOTING.md)

### Driver name clash (VERR_PDM_USB_NAME_CLASH)
- **Problema:** Drivers USB corrompidos/duplicados após reinstalação ou atualização.
- **Solução:** Reinstalar o VirtualBox do zero:
  1. Desinstalar o VirtualBox (aceitar a remoção de todos os componentes de rede/USB);
  2. Deletar `C:\Program Files\Oracle\VirtualBox` e `C:\Windows\System32\drivers\VBox*`;
  3. Reiniciar o sistema;
  4. Reinstalar pelo [virtualbox.org](https://www.virtualbox.org/).

# Homelab
Índice da minha infraestrutura de estudo.

[**EN-US**](../README.md)

![network_diagram drawio](https://github.com/user-attachments/assets/84e62055-0c59-4938-8264-b21d70742098)

## Ambiente de Desenvolvimento

### Máquina Host
- [**VS Code IDE:**](https://github.com/DiogoZanini/VSCode-IDE-setup) Configuração do VSCode para desenvolvimento em C, Python e SQLite, estendendo o fluxo de trabalho do CS50.

### pfSense (Oracle VirtualBox)
- [**Gateway de Rede Virtual:**](https://github.com/DiogoZanini/pfSense) Gateway padrão da rede do laboratório virtual, responsável pelo roteamento e regras de firewall.

### SanDisk USB Drive
- [**Tails Amnesic Incognito System:**](https://github.com/DiogoZanini/Portable-Linux-Tails) Configuração pessoal e notas operacionais para um ambiente de segurança amnésico em um pendrive.

## Roadmap
- [x] Tails Amnesic Incognito System em um pendrive;
- [x] Máquina Host: VS Code IDE e Oracle VirtualBox;
- [x] Máquina virtual pfSense;
- [ ] Máquina virtual Kali Linux para análise;
- [ ] Máquinas vulneráveis Metasploitable;
- [ ] Servidor Web vulnerável OWASP Juice Shop;
- [ ] Laboratório SOC.

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

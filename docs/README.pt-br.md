# Homelab
Índice da minha infraestrutura de estudo.

[**EN-US**](../README.md)

![network_diagram drawio](https://github.com/user-attachments/assets/84e62055-0c59-4938-8264-b21d70742098)

## Ambiente de Desenvolvimento
### Máquina Hospedeira
- **IDE:** [Configuração do VS Code IDE](https://github.com/DiogoZanini/VSCode-IDE-setup)

### pfSense [Oracle VirtualBox]
- **Gateway de Rede Virtual:** Gateway padrão para a rede virtual do laboratório, responsável pelo roteamento e regras de firewall.

### Pendrive USB SanDisk
- **Tails OS:** [Portable-Linux-Tails](https://github.com/DiogoZanini/Portable-Linux-Tails)

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

# Homelab
Índice da minha infraestrutura de estudo.

[**EN-US**](../README.md)

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

### Conflito de nome de driver. Já existe outro driver com o mesmo nome do que está sendo registrado. (VERR_PDM_USB_NAME_CLASH)
- **Problema:** Driver corrompido e duplicado no sistema hospedeiro (host);
- **Solução:** <details><summary>Reinstalar e remover todos os dados.</summary>

- Desinstale o VirtualBox;
- Remova as pastas `C:\Program Files\Oracle\VirtualBox` e os arquivos `C:\Windows\System32\drivers\VBox*`;
- Reinicie o sistema;
- Instale o [VirtualBox](https://www.virtualbox.org/) novamente.
</details>
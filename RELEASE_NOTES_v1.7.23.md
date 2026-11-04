# DogMint Pro 1.7.23 — Linux (pré-lançamento)

**Tag sugerida:** `v1.7.23`  
**Título:** `DogMint Pro 1.7.23 — Linux (Beta)`  
**Tipo:** Pré-lançamento (*pre-release*)

## Sobre esta versão

A versão 1.7.23 é uma **beta corrigida do DogMint Pro para Linux x86-64**, especialmente sistemas baseados em Debian, como Linux Mint e Ubuntu. Inclui ferramentas de monitoramento de hardware, diagnóstico de gargalos, informações de SSD, rede e gerenciamento de jogos.

## Melhorias e correções

- **HWMonitor:** descoberta de discos, leitura SMART em cache e consultas periódicas com melhor controle de concorrência.
- **Dog Game Launcher:** correção de IDs numéricos da Steam, suporte à localização do Steam Flatpak e migração de configurações antigas.
- **Dog SSD:** tentativa de leitura sem privilégios quando `sudo -n` não estiver disponível e indicação de possíveis problemas de permissão.
- **Dog Stress Test:** sensores térmicos adicionais, suporte a dados da NVIDIA via `nvidia-smi` e proteções reforçadas para testes de carga.
- **Overlay OpenGL/EGL:** melhorias de sincronização, captura e suporte adicional a funções EGL.
- **Sistema:** logs rotativos, correções de recursos e dependências do instalador.

## Instalador para anexar manualmente ao Release

`DogMint-Pro-1.7.23-corrigido.zip`

O ZIP contém:
- `DogMint-Pro_1.7.23_amd64.deb`
- `LEIA-ME-DogMint-1.7.23.txt`

## Como instalar

Extraia o arquivo `.deb` do ZIP e, na pasta do instalador, execute:

```bash
sudo apt install ./DogMint-Pro_1.7.23_amd64.deb
dogmint-pro --check
dogmint-pro
```

## Limitações conhecidas

Esta é uma **versão experimental**, não homologada em todos os computadores. Ainda faltam testes físicos em jogos reais e drivers variados, dispositivos SMART SATA/NVMe/USB, carga de CPU/GPU e instalações Linux Mint reais. A detecção automática de FPS em jogos externos não está concluída; o coletor nativo ainda não oferece suporte a Vulkan/Proton. A tradução online depende de um serviço não oficial.

**Recomenda-se fazer backup e verificar o funcionamento antes de usar em um computador de produção.**

## Próximas plataformas

Versões para **Windows, macOS e Steam Deck** estão planejadas para lançamento futuro. **Nenhum pacote dessas plataformas faz parte deste lançamento Linux.**

---

*Nota ao mantenedor: antes de distribuição comercial ou lançamento estável, revisar o campo Maintainer do pacote, os termos de licença e as licenças dos componentes de terceiros.*

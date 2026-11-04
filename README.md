# 🐶 DogMint Pro

**DogMint Pro** é um aplicativo de monitoramento, diagnóstico e organização do computador para **Linux**. Reúne ferramentas de CPU, GPU, SSD, rede, processos, jogos e sensores em uma interface gráfica.

> **Versão Linux mais recente em preparação para distribuição: 1.7.23 (beta/testes)**  
> A versão ainda não foi validada em todos os computadores. Alguns recursos continuam experimentais.

## 🖥️ Compatibilidade

- Linux **x86-64 / amd64**, principalmente distribuições baseadas em Debian, como **Linux Mint e Ubuntu**.
- Pacote instalador: `.deb`.
- Requer Python 3, Tkinter e dependências indicadas pelo instalador.
- Além do Linux, o projeto tem versões beta/experimentais para **Windows, macOS e Steam Deck**. Cada plataforma exige testes e instaladores próprios.

## 🚧 Betas por plataforma

| Plataforma | Versão / estágio | Distribuição |
| --- | --- | --- |
| 🐧 **Linux Mint / Ubuntu / Debian** | **1.7.23 — testes** | Pacote `.deb` preparado; publicação em Releases pendente |
| 🪟 **Windows** | **Beta 0.6** | Pacote de testes preparado; publicação em Releases pendente |
| 🍎 **macOS** | **Beta 0.2.0** | Pacote de testes preparado; publicação em Releases pendente |
| 🎮 **Steam Deck (SteamOS)** | **Beta experimental** | Suporte em desenvolvimento; pacote de download ainda não confirmado |

> **Atenção:** versões beta podem conter falhas e ter recursos indisponíveis. Os pacotes de Windows, macOS e Steam Deck não estão publicados como Releases neste repositório até o momento. Não é garantida compatibilidade total, especialmente no Steam Deck/SteamOS.


## ✨ Recursos

- **Monitoramento** de CPU, GPU (inclusive integrada, quando suportada), RAM e sensores;
- **Dog SSD Health**: consulta informações SMART e a saúde dos discos compatíveis;
- **Dog Network**: ferramentas de rede e conectividade;
- **Gargalo**: diagnóstico indicativo de CPU e GPU durante o uso e jogos;
- **Stress Test**: testes de carga com verificações de temperatura e segurança;
- **Dog FPS**: overlay/medição nativa experimental para aplicações compatíveis;
- **Jogos**: estimativas de FPS que dependem de serviços externos;
- **Game Launcher**, tarefas, inicialização e gerenciamento de aplicativos;
- Interface escura e seleção de idiomas.

A disponibilidade de alguns sensores e funções varia conforme o hardware, os drivers, as permissões e o ambiente Linux.

## 📦 Instalação (Linux)

Após baixar o pacote `.deb` na seção de **Releases** (quando o lançamento estiver disponível):

1. Extraia o arquivo `.deb` se ele vier dentro de um ZIP.
2. Abra o terminal na pasta do arquivo e execute:

```bash
sudo apt install ./DogMint-Pro_1.7.23_amd64.deb
dogmint-pro --check
dogmint-pro
```

Você também pode procurar **DogMint Pro** no menu de aplicativos.

Para desinstalar:

```bash
sudo apt remove dogmint-pro
```

## ⚠️ Estado da versão 1.7.23

A compilação e testes automatizados básicos foram realizados, **mas ainda faltam testes físicos de integração** em diferentes máquinas e distribuições. Em especial:

- A captura automática de FPS em jogos externos ainda não está concluída;
- O coletor nativo não oferece suporte a Vulkan/Proton nesta versão;
- O overlay, os sensores SMART, os testes de estresse e a instalação precisam de validação adicional em hardware real;
- Traduções online dependem de um serviço externo não oficial.

**Faça backup antes de instalar uma versão de testes.** Verifique os comandos e permissões solicitadas pelo pacote. O software não deve ser apresentado como 100% compatível.

## 📖 Documentação

O ZIP de distribuição contém o instalador e o arquivo **LEIA-ME-DogMint-1.7.23.txt** com instruções, correções e limitações da versão.

## 🛠️ Projeto e direitos

Projeto mantido pela conta [cachorroapk](https://github.com/cachorroapk). Os termos de licença do DogMint ainda precisam ser definidos e publicados. Bibliotecas e componentes de terceiros mantêm suas próprias licenças.

---

**Repositório oficial:** https://github.com/cachorroapk/DogMint

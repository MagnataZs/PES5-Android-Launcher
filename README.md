# PES 5 Android (não oficial)

Port Android ARM64 não oficial de **Pro Evolution Soccer 5**, baseado na versão original de Xbox e no projeto [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp). O código do jogo é recompilado para código nativo; a interface Android usa SDL3 e renderização Vulkan. Não é um emulador.

## Download

Baixe o APK mais recente na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest).

- **Versão:** 1.1.2 (`versionCode` 13)
- **Pacote:** `com.datfooldive.pes5`
- **Arquitetura:** ARM64 (`arm64-v8a`)
- **Android:** 10 (API 29) ou mais recente
- **Gráficos:** dispositivo com suporte a Vulkan 1.1 ou posterior
- **Tamanho do APK:** aproximadamente 45 MB
- **Assinatura:** chave de debug do projeto; mantém a assinatura das builds anteriores e permite atualização, mas não é assinatura para loja de aplicativos

## Gestos com barra de seleção visual

Ao deslizar em um botão de ação, uma barra verde acompanha o movimento e exibe o nome da jogada selecionada. Solte para confirmar. No **B**, deslize para cima para **Cavadinha** ou para baixo para **Chute colocado**; no **X**, deslize para cima para **Cruzamento antecipado**; no **Y**, deslize para cima para **Enfiada aérea**. Um toque simples, sem deslizar, mantém o comando original. O recurso se aplica apenas aos controles na tela; controles físicos não são alterados.

## Recursos mantidos

A v1.1.2 mantém os perfis gráficos **Desempenho**, **Equilibrado** e **Qualidade Visual**, além de ajustes manuais. O perfil de desempenho usa resolução de renderização em 50%, antisserrilhamento e sombras desligados, frame skip ligado e VSync ligado. O perfil equilibrado usa 67% de resolução e sombras baixas. O perfil de qualidade usa resolução em 100%, SMAA e sombras médias.

Também estão incluídos a exportação de logs, backup ZIP dos saves sem mover ou apagar os originais, correção recompilada `0x00037950` para o crash ao iniciar uma partida, e os créditos de @diparis_4m, @_silvaxis7 e MagnataZs.

## Instalação e arquivos do jogo

1. Baixe o APK na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest), abra-o e permita **Instalar apps desconhecidos** para o navegador ou gerenciador de arquivos, caso o Android solicite.
2. Se já tiver uma versão instalada, instale por cima e escolha **Atualizar**; não desinstale antes, para preservar os dados privados do aplicativo.
3. Permita o acesso aos arquivos quando solicitado.
4. Toque em **Selecionar arquivo do jogo** e escolha sua ISO de PES 5 para Xbox obtida legalmente; o launcher copia o arquivo para `/storage/emulated/0/PES5`. Como alternativa, coloque a ISO ou os arquivos extraídos nessa pasta.
5. Aguarde o status **Pronto para jogar** e toque em **JOGAR**.

**Requisitos:** Android 10 ou superior, ARM64 (`arm64-v8a`) e Vulkan 1.1 ou superior. A ISO e os dados do jogo não são incluídos nesta release; forneça sua própria cópia legal.

## Integridade do APK v1.1.2

SHA-256:

```text
46058769f5a46e4770f482c8abfad478af7b34b98b45361379234204bb88a256
```

## Estado e créditos

Projeto em desenvolvimento. Usa o [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp), além de SDL3, glslang, Dear ImGui, toml++ e Vulkan Memory Allocator. Consulte os repositórios upstream para seus respectivos créditos e licenças.

**Créditos desta build:** @diparis_4m, @_silvaxis7 e MagnataZs.

**Pro Evolution Soccer 5 © 2005 Konami.** Este projeto não é afiliado, patrocinado ou endossado pela Konami. Marcas e direitos do jogo pertencem aos respectivos titulares.

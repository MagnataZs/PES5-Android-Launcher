# PES 5 Android (não oficial)

Port Android ARM64 não oficial de **Pro Evolution Soccer 5**, baseado na versão original de Xbox e no projeto [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp). O código do jogo é recompilado para código nativo; a interface Android usa SDL3 e renderização Vulkan. Não é um emulador.

## Download

Baixe o APK mais recente na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest).

- **Versão:** 1.0.6 (`versionCode` 7)
- **Pacote:** `com.datfooldive.pes5`
- **Arquitetura:** ARM64 (`arm64-v8a`)
- **Android:** 10 (API 29) ou mais recente
- **Gráficos:** dispositivo com suporte a Vulkan 1.1 ou posterior
- **Tamanho do APK:** aproximadamente 45 MB
- **Assinatura:** chave de debug do projeto; mantém a assinatura da v1.0.5 e instala como atualização, mas não é assinatura para loja de aplicativos

## Novidades da v1.0.6

O launcher recebeu uma tela inicial com hierarquia visual renovada e três perfis gráficos: **Desempenho**, **Equilibrado** e **Qualidade Visual**. O perfil de desempenho usa resolução de renderização em 50%, antisserrilhamento e sombras desligados, frame skip ligado e mantém VSync ligado. O perfil equilibrado usa 67% de resolução e sombras baixas. O perfil de qualidade usa resolução em 100%, SMAA e sombras médias. As configurações também podem ser ajustadas individualmente.

O loop de frames agora reduz a janela final de espera ativa para até 250 microssegundos, com uma etapa intermediária de espera curta. A mudança busca reduzir tempo de CPU ocupado durante a espera, mantendo a cadência calculada do jogo. **O impacto em consumo, temperatura e frametime ainda não foi medido em aparelhos; não há ganho de FPS garantido.** A lógica/simulação do jogo e o comportamento de VSync não foram deliberadamente alterados por essa otimização.

A versão mantém exportação de logs e backup ZIP dos saves, com as ferramentas em thread separada do scanner; o backup não move nem apaga os saves originais. Também mantém a função recompilada `0x00037950` que corrigiu o crash ao iniciar uma partida e os créditos de @diparis_4m, @_silvaxis7 e MagnataZs.

## Instalação e arquivos do jogo

1. Baixe o APK na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest), abra-o e permita **Instalar apps desconhecidos** para o navegador ou gerenciador de arquivos, caso o Android solicite.
2. Se já tiver uma versão instalada, instale por cima e escolha **Atualizar**; não desinstale antes, para preservar os dados privados do aplicativo.
3. Permita o acesso aos arquivos quando solicitado.
4. Toque em **Selecionar arquivo do jogo** e escolha sua ISO de PES 5 para Xbox obtida legalmente; o launcher copia o arquivo para `/storage/emulated/0/PES5`. Como alternativa, coloque a ISO ou os arquivos extraídos nessa pasta.
5. Aguarde o status **Pronto para jogar** e toque em **JOGAR**.

**Requisitos:** Android 10 ou superior, ARM64 (`arm64-v8a`) e Vulkan 1.1 ou superior. A ISO e os dados do jogo não são incluídos nesta release; forneça sua própria cópia legal.

## Integridade do APK v1.0.6

SHA-256:

```text
257a1ccda1b0be6804400d9cf5e38ca90e329ed7ea7e675f8ae9450da3f2bd7d
```

## Estado e créditos

Projeto em desenvolvimento. Usa o [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp), além de SDL3, glslang, Dear ImGui, toml++ e Vulkan Memory Allocator. Consulte os repositórios upstream para seus respectivos créditos e licenças.

**Créditos desta build:** @diparis_4m, @_silvaxis7 e MagnataZs.

**Pro Evolution Soccer 5 © 2005 Konami.** Este projeto não é afiliado, patrocinado ou endossado pela Konami. Marcas e direitos do jogo pertencem aos respectivos titulares.

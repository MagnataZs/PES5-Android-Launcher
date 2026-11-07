# PES 5 Android (não oficial)

Port Android ARM64 não oficial de **Pro Evolution Soccer 5**, baseado na versão original de Xbox e no projeto [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp). O código do jogo é recompilado para código nativo; a interface Android usa SDL3 e renderização Vulkan. Não é um emulador.

## Download

Baixe o APK mais recente na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest).

- **Versão:** 1.1.4 (`versionCode` 15)
- **Pacote:** `com.datfooldive.pes5`
- **Arquitetura:** ARM64 (`arm64-v8a`)
- **Android:** 10 (API 29) ou mais recente
- **Gráficos:** dispositivo com suporte a Vulkan 1.1 ou posterior
- **Tamanho do APK:** aproximadamente 45 MB
- **Assinatura:** chave de debug do projeto; mantém a assinatura das builds anteriores e permite atualização, mas não é assinatura para loja de aplicativos

## Novidades da v1.1.4

- **Hotfix Vulkan:** o alinhamento do buffer uniforme agora respeita o limite informado pela GPU. A validação do cache SPIR-V também foi restaurada para descartar shaders corrompidos antes de criar módulos Vulkan.
- **Launcher simplificado:** removidos o cartão de presets de desempenho, a exportação de logs e o backup de saves. As opções manuais do jogo continuam disponíveis.
- **Privacidade:** o app não mantém nem exporta logs próprios; os arquivos de log anteriores do app são removidos na primeira inicialização desta versão. Os saves não são apagados nem alterados.
- O ajuste foi testado após a queda de fluidez reportada; o desempenho pode variar conforme aparelho e configuração gráfica.

## Controles touchscreen

Os botões seguem o mapeamento padrão do PES 5 para Xbox: **A** passe curto, **B** passe longo/cruzamento, **X** chute e **Y** passe enfiado. Durante o deslize, uma barra verde acompanha o dedo e mostra a jogada; solte para confirmar.

- **B para cima:** passe longo aéreo/cruzamento alto.
- **X para cima:** cavadinha.
- **X para baixo:** chute colocado.
- **Y para cima:** enfiada aérea.

Toques sem deslizar mantêm o comando original. Controles físicos não são alterados.

## Instalação e arquivos do jogo

1. Baixe o APK na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest), abra-o e permita **Instalar apps desconhecidos** para o navegador ou gerenciador de arquivos, caso o Android solicite.
2. Se já tiver uma versão instalada, instale por cima e escolha **Atualizar**; não desinstale antes, para preservar os dados privados do aplicativo.
3. Permita o acesso aos arquivos quando solicitado.
4. Toque em **Selecionar arquivo do jogo** e escolha sua ISO de PES 5 para Xbox obtida legalmente; o launcher copia o arquivo para `/storage/emulated/0/PES5`. Como alternativa, coloque a ISO ou os arquivos extraídos nessa pasta.
5. Aguarde o status **Pronto para jogar** e toque em **JOGAR**.

**Requisitos:** Android 10 ou superior, ARM64 (`arm64-v8a`) e Vulkan 1.1 ou superior. A ISO e os dados do jogo não são incluídos nesta release; forneça sua própria cópia legal.

## Integridade do APK v1.1.4

SHA-256:

```text
45d7be6d05840fe8d9910005282fd1f06fecc68aa54c523f89322d3b43b258e4
```

## Estado e créditos

Projeto em desenvolvimento. Usa o [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp), além de SDL3, glslang, Dear ImGui, toml++ e Vulkan Memory Allocator. Consulte os repositórios upstream para seus respectivos créditos e licenças.

**Créditos desta build:** @diparis_4m, @_silvaxis7 e MagnataZs.

**Pro Evolution Soccer 5 © 2005 Konami.** Este projeto não é afiliado, patrocinado ou endossado pela Konami. Marcas e direitos do jogo pertencem aos respectivos titulares.

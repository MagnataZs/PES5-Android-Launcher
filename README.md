# PES 5 Android (não oficial)

Port Android ARM64 não oficial de **Pro Evolution Soccer 5**, baseado na versão original de Xbox e no projeto [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp). O código do jogo é recompilado para código nativo; a interface Android usa SDL3 e renderização Vulkan. Não é um emulador.

## Download

Baixe o APK mais recente na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest).

- **Versão:** 1.0.3 (versionCode 4)
- **Pacote:** `com.datfooldive.pes5`
- **Arquitetura:** ARM64 (`arm64-v8a`)
- **Android:** 10 (API 29) ou mais recente
- **Gráficos:** dispositivo com suporte a Vulkan 1.1 ou posterior
- **Tamanho do APK:** aproximadamente 45 MB
- **Assinatura:** chave de debug do projeto; build de teste, não assinatura de distribuição de loja

### Launcher e desempenho v1.0.3

O launcher foi redesenhado em português, com identidade visual escura em verde, status do jogo, créditos e acesso mais claro às ferramentas. O perfil **DESEMPENHO MÁXIMO** configura renderização a 50%, antisserrilhamento e sombras desligados, frame skip ligado e VSync desligado; **EQUILIBRADO** restaura valores visuais moderados. As opções também podem ser ajustadas individualmente. Não foi criado um controle para remover a torcida: o renderer atual não expõe um caminho seguro para isso.

**Sincronização vertical:** ao alterar VSync durante uma partida, a preferência é salva e aplicada no próximo início do jogo, evitando recriar a swapchain no meio da sessão e o pisca-pisca observado em alguns aparelhos Android.

Em **DESEMPENHO E FERRAMENTAS**, **Exportar logs** salva uma cópia do log do jogo pelo seletor Android. **Fazer backup dos saves** cria um ZIP das pastas `hdd` encontradas junto ao jogo e no armazenamento privado do app; os arquivos originais não são movidos nem apagados. A build mantém o ponto de entrada `0x00037950` incluído no hotfix v1.0.1.

### Instalação e arquivos do jogo

1. Instale o APK e permita o acesso a arquivos quando o Android solicitar.
2. Copie sua imagem de disco (`.iso`) legalmente obtida, ou os arquivos extraídos do disco, para uma pasta `PES5` no armazenamento compartilhado do aparelho. A pasta padrão é `/storage/emulated/0/PES5`.
3. Abra **PES5 Android**. O aplicativo procura os arquivos do jogo nessa pasta.

**A ISO e os arquivos de dados do disco não são incluídos nesta release.** É necessário fornecer uma cópia do jogo que você tenha direito de usar. O APK contém código nativo recompilado a partir do executável do jogo.

### Integridade do APK v1.0.3

SHA-256:

```text
f524295c60e6e7923ed0058347141bbc20933279e42ba30e025010295c6d44b7
```

## Estado e créditos

Projeto em desenvolvimento. Usa o [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp), além de SDL3, glslang, Dear ImGui, toml++ e Vulkan Memory Allocator. Consulte os repositórios upstream para seus respectivos créditos e licenças.

**Créditos desta build:** @diparis_4m, @_silvaxis7 e MagnataZs.

**Pro Evolution Soccer 5 © 2005 Konami.** Este projeto não é afiliado, patrocinado ou endossado pela Konami. Marcas e direitos do jogo pertencem aos respectivos titulares.

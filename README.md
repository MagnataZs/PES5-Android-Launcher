# PES 5 Android (não oficial)

Port Android ARM64 não oficial de **Pro Evolution Soccer 5**, baseado na versão original de Xbox e no projeto [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp). O código do jogo é recompilado para código nativo; a interface Android usa SDL3 e renderização Vulkan. Não é um emulador.

## Download

Baixe o APK mais recente na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest).

- **Versão:** 1.0.5 (`versionCode` 6)
- **Pacote:** `com.datfooldive.pes5`
- **Arquitetura:** ARM64 (`arm64-v8a`)
- **Android:** 10 (API 29) ou mais recente
- **Gráficos:** dispositivo com suporte a Vulkan 1.1 ou posterior
- **Tamanho do APK:** aproximadamente 45 MB
- **Assinatura:** chave de debug do projeto; compatível como atualização da v1.0.4, mas não é assinatura para loja de aplicativos

## Novidades da v1.0.5

A exportação de logs e o backup ZIP dos saves agora executam em uma thread de ferramentas separada da busca pelos arquivos do jogo, para que operações demoradas não deixem a verificação do jogo esperando. Os arquivos de save originais não são movidos nem apagados durante o backup.

O launcher permanece em português, com tema escuro/verde e créditos para @diparis_4m, @_silvaxis7 e MagnataZs. Esta versão mantém os perfis **Desempenho Máximo** e **Equilibrado**, a exportação de logs, o backup dos saves e a função recompilada `0x00037950` que corrige o crash ao iniciar a partida. A opção VSync alterada durante uma sessão é aplicada no próximo início do jogo, evitando recriar a swapchain durante a partida e reduzindo as piscadas observadas em alguns aparelhos.

O perfil **Desempenho Máximo** configura renderização a 50%, antisserrilhamento e sombras desligados, frame skip ligado e VSync desligado. **Equilibrado** restaura valores visuais moderados; as opções também podem ser ajustadas individualmente. Não foi adicionado controle para remover torcida, pois o renderer atual não expõe um caminho seguro para isso.

A atividade do jogo fica fixada em paisagem para tentar evitar a imagem girada/comprimida que pode aparecer ao retornar do launcher Android. A mudança ainda depende de teste no aparelho e pode impedir a rotação para o lado oposto.

## Instalação e arquivos do jogo

1. Baixe o APK na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest), abra-o e permita **Instalar apps desconhecidos** para o navegador ou gerenciador de arquivos, caso o Android solicite.
2. Permita o acesso aos arquivos quando solicitado.
3. Toque em **Selecionar arquivo do jogo** e escolha sua ISO de PES 5 para Xbox obtida legalmente; o launcher copia o arquivo para `/storage/emulated/0/PES5`. Como alternativa, coloque a ISO ou os arquivos extraídos nessa pasta.
4. Aguarde o status **Pronto para jogar** e toque em **JOGAR**.

**A ISO e os dados do jogo não são incluídos nesta release.** É necessário fornecer uma cópia do jogo que você tenha direito de usar. O APK contém código nativo recompilado a partir do executável do jogo.

## Integridade do APK v1.0.5

SHA-256:

```text
d3c7231fc5bc890e4b1d495b26674bc6409f41febd71efee93f3b5b7c58de5cb
```

## Estado e créditos

Projeto em desenvolvimento. Usa o [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp), além de SDL3, glslang, Dear ImGui, toml++ e Vulkan Memory Allocator. Consulte os repositórios upstream para seus respectivos créditos e licenças.

**Créditos desta build:** @diparis_4m, @_silvaxis7 e MagnataZs.

**Pro Evolution Soccer 5 © 2005 Konami.** Este projeto não é afiliado, patrocinado ou endossado pela Konami. Marcas e direitos do jogo pertencem aos respectivos titulares.

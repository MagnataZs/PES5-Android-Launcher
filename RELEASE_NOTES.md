## Instalação — leia primeiro

1. **Baixe o APK desta versão:** nesta página, expanda **Assets** e toque no arquivo `.apk` anexado a esta release.
2. **Instale:** abra o APK baixado. Se o Android bloquear a instalação, permita **Instalar apps desconhecidos** para o navegador ou gerenciador de arquivos usado e tente novamente; o nome e o caminho variam conforme o aparelho.
3. **Atualização:** se já tiver uma versão instalada, instale por cima e escolha **Atualizar**. Esta versão mantém a mesma assinatura da v1.0.4. Não desinstale antes, pois isso pode apagar dados privados do aplicativo.
4. **Prepare o jogo:** permita acesso aos arquivos quando solicitado. O launcher não inclui o jogo: use uma cópia de PES 5 para Xbox obtida legalmente. Toque em **Selecionar arquivo do jogo** e escolha sua ISO; o launcher copia o arquivo para `/storage/emulated/0/PES5`. Como alternativa, coloque a ISO ou os arquivos extraídos nessa pasta.
5. Aguarde o status **Pronto para jogar** e toque em **JOGAR**.

**Requisitos:** Android 10 ou superior, ARM64 (`arm64-v8a`) e Vulkan 1.1 ou superior. A ISO e os dados do jogo não estão incluídos.

---

## PES 5 Android — v1.0.5

- `versionCode` 6 / `versionName` 1.0.5; APK ARM64 de aproximadamente 45 MB.
- Exportação de logs e backup ZIP dos saves executam em uma thread própria, separada da busca pelos arquivos do jogo. Isso evita que operações longas dessas ferramentas bloqueiem a verificação do jogo.
- O backup cria um ZIP e não move nem apaga os saves originais.
- Mantém o launcher em português, o tema escuro/verde e os créditos de @diparis_4m, @_silvaxis7 e MagnataZs.
- Mantém os perfis **Desempenho Máximo** e **Equilibrado**, com opções individuais de renderização, FPS, proporção, VSync, antisserrilhamento, frame skip e sombras. O perfil máximo usa renderização a 50%, desliga antisserrilhamento/sombras, liga frame skip e desliga VSync.
- A alteração do VSync durante uma partida é salva para o próximo início do jogo, evitando recriar a swapchain no meio da sessão e reduzindo as piscadas observadas em alguns aparelhos.
- Mantém a função recompilada `0x00037950` do hotfix que corrigiu o crash ao iniciar uma partida.
- A atividade do jogo é fixada em paisagem para tentar evitar a imagem girada/comprimida ao retornar do launcher Android; o comportamento precisa ser confirmado no aparelho.
- Assinatura de debug do projeto, igual à v1.0.4; não destinada à publicação em loja.

**SHA-256:** `d3c7231fc5bc890e4b1d495b26674bc6409f41febd71efee93f3b5b7c58de5cb`

**Propriedade intelectual:** PES 5 © 2005 Konami. O projeto não é afiliado ou endossado pela Konami. O usuário deve fornecer sua própria cópia legal do jogo; nenhum dado da ISO está anexado.

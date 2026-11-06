## Instalação — leia primeiro

1. **Baixe o APK desta versão:** nesta página, expanda **Assets** e toque em `PES5-Android-launcher-v1.0.6.apk`.
2. **Instale:** abra o APK baixado. Se o Android bloquear a instalação, permita **Instalar apps desconhecidos** para o navegador ou gerenciador de arquivos usado e tente novamente.
3. **Atualização:** se já tiver uma versão instalada, instale por cima e escolha **Atualizar**. A v1.0.6 mantém a assinatura da v1.0.5. Não desinstale antes, pois isso pode apagar dados privados do aplicativo.
4. **Prepare o jogo:** permita acesso aos arquivos quando solicitado. O launcher não inclui o jogo: use uma cópia de PES 5 para Xbox obtida legalmente. Toque em **Selecionar arquivo do jogo** e escolha sua ISO; o launcher copia o arquivo para `/storage/emulated/0/PES5`. Como alternativa, coloque a ISO ou os arquivos extraídos nessa pasta.
5. Aguarde o status **Pronto para jogar** e toque em **JOGAR**.

**Requisitos:** Android 10 ou superior, ARM64 (`arm64-v8a`) e Vulkan 1.1 ou superior. A ISO e os dados do jogo não estão incluídos.

---

## PES 5 Android — v1.0.6

- `versionCode` 7 / `versionName` 1.0.6; APK ARM64 de aproximadamente 45 MB.
- Tela inicial redesenhada e três perfis gráficos: **Desempenho**, **Equilibrado** e **Qualidade Visual**.
- **Desempenho:** renderização a 50%, antisserrilhamento e sombras desligados, frame skip ligado e VSync ligado. **Equilibrado:** renderização a 67% e sombras baixas. **Qualidade Visual:** renderização a 100%, SMAA e sombras médias.
- Ajuste no pacing de quadros: a janela final de espera ativa foi reduzida a até 250 µs, com espera curta intermediária. A alteração busca reduzir CPU ocupada durante a espera; o efeito em frametime, consumo e temperatura depende de testes em aparelhos e não há ganho de FPS medido ou garantido.
- Mantém exportação de logs, backup ZIP dos saves em thread separada e preservação dos arquivos originais, além do hotfix recompilado `0x00037950`.
- Mantém os créditos para @diparis_4m, @_silvaxis7 e MagnataZs.
- Assinatura de debug do projeto, igual à v1.0.5; não destinada à publicação em loja.

**SHA-256:** `257a1ccda1b0be6804400d9cf5e38ca90e329ed7ea7e675f8ae9450da3f2bd7d`

**Propriedade intelectual:** PES 5 © 2005 Konami. O projeto não é afiliado ou endossado pela Konami. O usuário deve fornecer sua própria cópia legal do jogo; nenhum dado da ISO está anexado.

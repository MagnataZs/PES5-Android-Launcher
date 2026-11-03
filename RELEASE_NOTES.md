## Instalação — leia primeiro

1. **Baixe o APK desta versão:** nesta página, expanda **Assets** e toque no arquivo `.apk` anexado a esta versão.
2. **Instale:** abra o APK baixado. Se o Android bloquear a instalação, permita **Instalar apps desconhecidos** para o navegador ou gerenciador de arquivos usado e tente novamente; o nome e o caminho variam conforme o aparelho.
3. **Atualização:** se já tiver uma versão instalada, instale por cima e escolha **Atualizar**. Esta versão mantém a mesma assinatura. Não desinstale antes, pois isso pode apagar dados privados do aplicativo.
4. **Prepare o jogo:** permita o acesso aos arquivos quando solicitado. O launcher não inclui o jogo: use uma cópia de PES 5 para Xbox obtida legalmente. Toque em **Selecionar arquivo do jogo** e escolha sua ISO; o launcher copia o arquivo para `/storage/emulated/0/PES5`. Como alternativa, coloque a ISO ou os arquivos extraídos nessa pasta.
5. Aguarde o status **Pronto para jogar** e toque em **JOGAR**.

**Requisitos:** Android 10 ou superior, ARM64 (`arm64-v8a`) e Vulkan 1.1 ou superior. A ISO e os dados do jogo não estão incluídos.

---

## PES 5 Android — v1.0.4 (build de teste)

- A atividade do jogo fica fixada em paisagem, em vez de seguir os dois lados da orientação landscape. A alteração tenta evitar a imagem girada/comprimida que aparece por um instante ao retornar do launcher Android. **É um teste: precisa ser confirmado no aparelho.**
- Mantém o novo visual em português, créditos para @diparis_4m, @_silvaxis7 e MagnataZs, e os perfis **Desempenho Máximo** e **Equilibrado**.
- O perfil máximo configura renderização a 50%, antisserrilhamento e sombras desligados, frame skip ligado e VSync desligado.
- Mantém exportação de logs, backup ZIP dos saves e a função recompilada `0x00037950` do hotfix anterior.
- `versionCode` 5 / `versionName` 1.0.4; assinatura igual à das versões anteriores, instalável como atualização.
- Assinado com a chave de debug do projeto; não destinado à publicação em loja.

SHA-256: `93463a27a169b5037a7c02f8b09228278c3f83b00ebcc0265746356bc408973d`

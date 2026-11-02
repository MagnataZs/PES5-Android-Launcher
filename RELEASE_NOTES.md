## PES 5 Android — v1.0.3

- Launcher redesenhado em português, com paleta noturna em verde, status do jogo e créditos para @diparis_4m, @_silvaxis7 e MagnataZs.
- Adicionado o preset **Desempenho Máximo**: renderização a 50%, antisserrilhamento e sombras desligados, frame skip ligado e VSync desligado.
- Adicionado o preset **Equilibrado** e controles no launcher para frame skip e qualidade das sombras.
- Alterações de VSync feitas durante uma partida são guardadas e aplicadas no próximo início do jogo; isso evita recriar a swapchain em runtime, comportamento que causava piscadas em alguns aparelhos.
- Mantém exportação de logs, backup ZIP dos saves e a função recompilada `0x00037950` do hotfix anterior.
- `versionCode` 4 / `versionName` 1.0.3; assinatura igual à das versões anteriores, para instalar como atualização.
- Requisitos: Android 10 (API 29) ou superior, Vulkan 1.1+ e ARM64 (`arm64-v8a`).
- ISO e arquivos do jogo não estão incluídos. Use somente uma cópia obtida legalmente.
- Assinado com a chave de debug do projeto; não destinado à publicação em loja.

SHA-256 do APK: `f524295c60e6e7923ed0058347141bbc20933279e42ba30e025010295c6d44b7`

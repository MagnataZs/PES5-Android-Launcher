## Instalação — leia primeiro

1. **Baixe o APK desta versão:** nesta página, expanda **Assets** e toque em `PES5-Android-v1.1.4.apk`.
2. **Instale:** abra o APK baixado. Se o Android bloquear a instalação, permita **Instalar apps desconhecidos** para o navegador ou gerenciador de arquivos usado e tente novamente.
3. **Atualização:** instale por cima e escolha **Atualizar**. Esta build mantém a assinatura de debug das versões anteriores. Não desinstale antes, pois isso pode apagar dados privados do aplicativo.
4. **Prepare o jogo:** permita acesso aos arquivos quando solicitado. O launcher não inclui o jogo: use uma cópia de PES 5 para Xbox obtida legalmente. Toque em **Selecionar arquivo do jogo** e escolha sua ISO; o launcher copia o arquivo para `/storage/emulated/0/PES5`. Como alternativa, coloque a ISO ou os arquivos extraídos nessa pasta.
5. Aguarde o status **Pronto para jogar** e toque em **JOGAR**.

**Requisitos:** Android 10 ou superior, ARM64 (`arm64-v8a`) e Vulkan 1.1 ou superior. A ISO e os dados do jogo não estão incluídos.

---

## PES 5 Android — v1.1.4

- `versionCode` 15 / `versionName` 1.1.4; APK ARM64 de aproximadamente 45 MB.
- **Hotfix Vulkan:** buffers uniformes usam o alinhamento mínimo reportado pelo dispositivo. A leitura do cache SPIR-V volta a validar o cabeçalho e descartar entradas inválidas.
- Ajuste testado pelo usuário após uma queda de fluidez reportada. O desempenho pode variar por aparelho e configuração; não representa benchmark universal.
- **Launcher simplificado:** removidos o cartão de presets, a exportação de logs e a ferramenta de backup de saves. As opções manuais continuam disponíveis.
- **Privacidade:** o app não mantém nem exporta logs próprios; logs privados anteriores do app são removidos na primeira inicialização desta versão. Os saves não são alterados.
- Mantém os gestos touchscreen corrigidos da v1.1.3: B para cima = passe aéreo/cruzamento alto; X para cima = cavadinha; X para baixo = chute colocado; Y para cima = enfiada aérea. Soltar confirma a ação indicada pela barra visual.
- Mantém os créditos para @diparis_4m, @_silvaxis7 e MagnataZs.
- Assinatura de debug do projeto, igual às versões anteriores; não destinada à publicação em loja.

**SHA-256:** `45d7be6d05840fe8d9910005282fd1f06fecc68aa54c523f89322d3b43b258e4`

**Propriedade intelectual:** PES 5 © 2005 Konami. O projeto não é afiliado ou endossado pela Konami. O usuário deve fornecer sua própria cópia legal do jogo; nenhum dado da ISO está anexado.

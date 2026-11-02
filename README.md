# PES 5 Android (não oficial)

Port Android ARM64 não oficial de **Pro Evolution Soccer 5**, baseado na versão original de Xbox e no projeto [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp). O código do jogo é recompilado para código nativo; a interface Android usa SDL3 e renderização Vulkan. Não é um emulador.

## Download

Baixe o APK mais recente na página de [Releases](https://github.com/MagnataZs/PES5-Android-Launcher/releases/latest).

- **Versão:** 1.0
- **Pacote:** `com.datfooldive.pes5`
- **Arquitetura:** ARM64 (`arm64-v8a`)
- **Android:** 10 (API 29) ou mais recente
- **Gráficos:** dispositivo com suporte a Vulkan 1.1 ou posterior
- **Tamanho do APK:** aproximadamente 45 MB
- **Assinatura:** chave de debug do projeto; build de teste, não assinatura de distribuição de loja

### Instalação e arquivos do jogo

1. Instale o APK e permita o acesso a arquivos quando o Android solicitar.
2. Copie sua imagem de disco (`.iso`) legalmente obtida, ou os arquivos extraídos do disco, para uma pasta `PES5` no armazenamento compartilhado do aparelho. A pasta padrão é `/storage/emulated/0/PES5`.
3. Abra **PES5 Android**. O aplicativo procura os arquivos do jogo nessa pasta.

**A ISO e os arquivos de dados do disco não são incluídos nesta release.** É necessário fornecer uma cópia do jogo que você tenha direito de usar. O APK contém código nativo recompilado a partir do executável do jogo.

### Integridade do APK v1.0

SHA-256:

```text
fea215f7ac45fad2543d2833a13201f9781659e8616946459f5e5ac3d3e3e53e
```

## Estado e créditos

Projeto em desenvolvimento. Usa o [XboxXBE-Recomp](https://github.com/TGP482/XboxXBE-Recomp), além de SDL3, glslang, Dear ImGui, toml++ e Vulkan Memory Allocator. Consulte os repositórios upstream para seus respectivos créditos e licenças.

**Pro Evolution Soccer 5 © 2005 Konami.** Este projeto não é afiliado, patrocinado ou endossado pela Konami. Marcas e direitos do jogo pertencem aos respectivos titulares.

# LightCraft — documentação em português do Brasil (pt-BR)

**Biblioteca de fotos e revelação RAW; uma reimplementação open-source e clean-room do Adobe Lightroom, reconstruída em Rust puro.**

Feito em Rust puro, funciona nativamente em macOS, Windows e Linux e também no navegador via WebAssembly.

## Recursos

- 91 comandos de engine e 48 comandos de UI, todos endereçáveis e clicáveis por nome — operável por agentes de IA.
- Servidor MCP embutido: `lightcraft-cli mcp` expõe ~100 ferramentas (importar, consultar, revelar, mascarar…).
- CLI scriptável: `lightcraft-cli run --import in.dng develop.set control=light.exposure value=0.7 app.export …`.
- Undo para tudo, inclusive ações de agentes; catálogos de interface totalmente traduzidos.

## Português do Brasil

Selecione Editar ▸ Idioma ▸ Português (Brasil), ou configure `~/.config/lightcraft/ui.json` com `"language": "pt-br"`.

PR #228 já foi MESCLADO no upstream — a interface em pt-BR é oficial.

## A suíte ArtCraft

A ArtCraft é um conjunto de 7 aplicativos open-source que reimplementam, de forma clean-room e em Rust puro, as ferramentas de criação da Adobe — nativos para macOS, Windows e Linux, com a mesma interface no navegador via WebAssembly:

| Aplicativo | Propósito | Reimplementação de |
|---|---|---|
| PhotoCraft | Edição de imagens | Adobe Photoshop |
| FilmCraft | Edição de vídeo, cor e som | Adobe Premiere Pro |
| LightCraft | Biblioteca de fotos e revelação RAW | Adobe Lightroom |
| EffectCraft | Motion graphics e efeitos visuais | Adobe After Effects |
| PrintCraft | Workbench de PDF | Adobe Acrobat |
| DesignCraft | Layout de página e publicação | Adobe InDesign |
| VectorCraft | Ilustração vetorial | Adobe Illustrator |

- Site: <https://getartcraft.com> · Discord: <https://discord.gg/artcraft>

## Este fork

Adiciona **leitura desta documentação em português do Brasil** e, no código, a **tradução pt-BR da interface** — sem alterar nada do comportamento do aplicativo original.


## Instalar no Linux (x86_64)

Baixe o tarball da release e extraia (sem precisar de sudo):

```bash
wget https://github.com/storytold/lightcraft/releases/download/v0.2.1/lightcraft-0.2.1-linux-x86_64.tar.gz
mkdir -p ~/Programas/lightcraft
tar -xzf lightcraft-0.2.1-linux-x86_64.tar.gz -C ~/Programas/lightcraft --strip-components=1
~/Programas/lightcraft/bin/lightcraft
```

> Consulte a página de releases do repositório upstream para a versão e o nome do asset atuais.

## Compilar do código

```bash
git clone https://github.com/storytold/<repositorio-upstream>.git
cd <repositorio-upstream>
# (opcional, para as fontes CJK do release) export CRAFT_FONTS_DIR=~/craft-fonts CRAFT_FONTS_REQUIRED=1
cargo build --release
```

## Comunidade

Suporte, feedback e novidades da suíte no Discord: <https://discord.gg/artcraft>.

---

Documentação original (inglês): [`README.md`](README.md).


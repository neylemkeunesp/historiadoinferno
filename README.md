# História do Inferno — Edição Expandida e Complementada

Repositório do livro **História do Inferno: Edição Expandida e Complementada** (Ney Lemke).

## Estrutura

```
.
├── main.tex              # Arquivo mestre LaTeX
├── frontmatter.tex       # Prefácio, sumário, dedicatória
├── referencias.bib       # Bibliografia BibTeX
├── capitulos/            # Capítulos do livro
├── figuras/              # Figuras e imagens (versão LFS)
└── build/                # Artefatos de compilação (ignorado)
```

## Compilação

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Ou com `latexmk`:

```bash
latexmk -pdf main.tex
```

## Notas

- Arquivos `*.pdf`, `*.png`, `*.jpg` são versionados via **Git LFS**.
- Arquivos auxiliares LaTeX (`.aux`, `.log`, `.out`, `.toc`, `.bbl`, `.blg`) são regenerados na compilação e ficam fora do versionamento.
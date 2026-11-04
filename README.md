# hpc-estudos

Minha trilha de estudos rumo à **computação de alto desempenho (HPC)**: do terminal Linux ao treino distribuído de modelos de IA em GPUs. Quem sabe me tornar um engenheiro de HPC algum dia.

Sou desenvolvedor e uso IA no dia a dia. Comecei sem base em C, sistemas ou paralelismo. Este repositório registra cada passo, inclusive os erros.

## O plano

78 semanas, 4 dias por semana, 1 hora por dia. Cursos da Alura somados a material gratuito (MIT Missing Semester, CS50, OpenMP com Tim Mattson, HPC Carpentry, NVIDIA DLI, GPU MODE). O plano completo está em [`PLANO.md`](PLANO.md).

| Fase | Tema | Semanas | Status |
| --- | --- | --- | --- |
| 0 | Terminal, Linux e Git | 1–6 | 🟡 em andamento |
| 1 | Linguagem C e como o computador funciona | 7–18 | ⚪ |
| 2 | C++ e performance (cache, tiling) | 19–30 | ⚪ |
| 3 | Paralelismo em CPU com OpenMP | 31–40 | ⚪ |
| 4 | Clusters com MPI e Slurm | 41–52 | ⚪ |
| 5 | GPU, CUDA e a base de IA | 53–66 | ⚪ |
| 6 | HPC para IA: treino distribuído | 67–78 | ⚪ |

## O fio condutor: `matmul/`

Uma multiplicação de matrizes 1000 × 1000 que começa em C puro e é reescrita a cada fase: C++ otimizado, OpenMP, MPI, CUDA e PyTorch. Cada versão fica na sua pasta, sem ser alterada depois, e todos os tempos vão para um CSV. No fim, um gráfico compara tudo.

Treinar um modelo de IA é, no fundo, multiplicar matrizes gigantes. Por isso o mesmo problema atravessa o plano inteiro.

## IA como ferramenta, não como atalho

Estudo com o Claude Code no papel de professor: ele dá dicas e revisa o que eu fiz, mas não entrega a solução dos exercícios. A regra é **a IA escreve, eu meço**: performance só vale com número, medido por benchmark ou profiler.

## Estrutura

```
hpc-estudos/
├── PLANO.md            plano completo, fase a fase
├── DIARIO.md           uma linha por sessão de estudo
├── CLAUDE.md           regras para a IA durante o estudo
└── fase-0-terminal/    anotações e exercícios da fase atual
```

As pastas crescem com as fases.

## Ambiente

Fedora 44 · AMD Ryzen 7 5825U (8 núcleos, 16 threads) · 7 GiB de RAM. Não tenho GPU NVIDIA: a parte de CUDA vai rodar no Google Colab.

# Plano de estudos: desenvolvimento com IA

Nov 4, 2026 · Otávio

> Fonte original (trilha HPC): https://claude.ai/artifact/1N443HmrDA4NNLbB2d1Wzj (exportado em 2026-11-04). Rumo revisto em 10/11/2026: Fase 0 → Fases A a E. A trilha HPC (Fases 1 a 6) está no fim, em espera.

## Como usar este plano

4 dias por semana, 1 hora por dia, dentro do 1 ano e meio de Alura que você ainda tem. A ordem importa mais que a velocidade, porque cada fase usa o que a anterior ensinou. As semanas de cada fase A a E são definidas quando a Fase 0 fechar.

**Sua semana padrão** (escolha 4 dias fixos e um horário fixo, ex.: seg, ter, qui e sáb às 20h)

| Dia | O que fazer na 1 hora |
| --- | --- |
| Dia 1 | Aula nova (vídeo ou leitura) |
| Dia 2 | Aula nova, digitando os exemplos você mesmo |
| Dia 3 | Prática: refazer os exercícios sem olhar a resposta |
| Dia 4 | Mini-projeto ou revisão + 5 min anotando o que aprendeu |

**Para criar o hábito**

- Mesmo horário, mesmo lugar, celular em outro cômodo.
- Dois blocos de 25 min com 5 min de pausa (Pomodoro).
- Nunca falhe dois dias seguidos. Perdeu um, faz o próximo.
- Semana corrida? Faça 20 min. Manter a sequência vale mais que a hora cheia.
- Termine cada sessão anotando onde parou e uma dúvida. Retomar fica fácil.
- Travou mais de 20 min num problema: pergunte (Luri, fórum da Alura, Discord, Claude).
- Atrasou? Estique a fase, não pule. As semanas abaixo são referência, não prazo.

**Regra de ouro:** cada fase termina com um mini-projeto no GitHub. É isso que vira portfólio e prova que você sabe.

## IA dentro do plano

A IA entra de dois jeitos: como **ferramenta** em toda fase (você já usa Claude Code todo dia) e como **o assunto principal** da carreira, a partir da Fase A. O dev que vale ouro nessa era é o que manda a IA fazer e consegue provar, com teste e número, se o resultado está certo.

**A regra: a IA escreve, você verifica.** Código gerado por IA costuma compilar e rodar, mas pode esconder um bug, uma brecha de segurança ou uma resposta inventada. Só o teste, a medição e a leitura atenta dizem a verdade, e é essa base que as fases constroem.

**Como usar a IA em cada fase**

| Fase | Deixe a IA fazer | Faça você mesmo |
| --- | --- | --- |
| 0 · Terminal | Explicar comandos e mensagens de erro | Digitar os comandos |
| A · IA aplicada | Explicar conceitos e sugerir variações de prompt para comparar | Montar o agente e medir se ele acerta (avaliação) |
| B · TypeScript e Node | Revisar seu código e explicar o erro, depois que você tentou | Escrever o código e ler a mensagem do compilador |
| C · SQL e Postgres | Explicar o plano da consulta e sugerir índices | Modelar as tabelas e escrever as consultas |
| D · Docker e Actions | Gerar Dockerfile e workflow, explicando cada linha | Entender cada linha e fazer rodar |
| E · Testes | Sugerir casos de borda que você esqueceu | Escrever os testes e ver cada um falhar antes de passar |

Na Fase 0 e no começo de cada fase nova, peça ao Claude para agir como professor: "me dê uma dica, não a resposta". Tira a dúvida sem tirar o aprendizado.

**Para usar o Claude Code como engenheiro, não como passageiro**

- [ ] [Claude Code in Action](https://www.datacamp.com/pt/courses/claude-code-in-action), curso gratuito de cerca de 3 h: conduzir sessões longas, criar regras com hooks e verificar o que volta. Faça no lugar da semana 6.

**A trilha de IA na Alura.** As carreiras que você já segue (Arquitetura de Soluções com IA, Engenharia de IA) e a AI Native Software Engineering, que conversa com seu jeito de trabalhar, viram a **trilha principal** a partir da Fase A. Com 4 h por semana não dá para levar as três inteiras em paralelo: na Fase A, escolha com o agente deste repositório uma carreira para seguir e use os cursos das outras só onde completarem algo que falta. As Fases B a E podem sair de cursos dessas mesmas carreiras ou de cursos avulsos.

## Visão geral

| Fase | Tema | Status |
| --- | --- | --- |
| 0 | Terminal, Linux e Git (semanas 1–6) | em andamento |
| A | IA aplicada: API de LLM, ferramentas, agentes, RAG, avaliação | próxima |
| B | TypeScript e Node.js | |
| C | SQL e PostgreSQL | |
| D | DevOps enxuto: Docker e GitHub Actions | |
| E | Testes automatizados | |
| 1–6 | Trilha HPC (C, C++, OpenMP, MPI, CUDA, HPC para IA) | em espera |

O fio condutor é o `tutor/`: um agente que estuda este repositório e evolui de fase em fase (detalhes em "Ponto de decisão" e no `CLAUDE.md`).

## Fase 0 · Terminal, Linux e Git (semanas 1 a 6)

Objetivo: ficar à vontade no terminal do Linux. Todo servidor, container e pipeline de CI roda Linux, e boa parte do trabalho com eles é pela linha de comando.

**Na Alura**

- [ ] [Sistema Operacional Linux: fundamentos e administração prática](https://www.alura.com.br/curso-online-linux-operacoes-fundamentos-comandos)
- [ ] [Git e GitHub: controle e compartilhe seu código](https://www.alura.com.br/curso-online-git-github-controle-de-versao)

**Por fora**

- [ ] [MIT Missing Semester](https://missing.csail.mit.edu/): as aulas de shell e linha de comando. Grátis, vídeos em inglês no YouTube (ative as legendas).

**Mini-projeto:** no repositório `estudos-dev-ia` (criado como `hpc-estudos`), Primeiro arquivo: um script Bash que mostra quantos núcleos e quanta memória sua máquina tem (`nproc`, `free -h`).

**Pronto pra avançar quando:** você navega pastas, edita arquivos, usa pipes (`|`) e faz commit e push sem consultar nada.

## Ponto de decisão: o que vem depois da Fase 0 (revisto em 10/11/2026)

A Fase 0 serve a qualquer rumo: terminal, Linux e Git são ferramentas de todo dev. Ela segue como está. As Fases 1 a 6 (C, OpenMP, MPI, CUDA) são o caminho de engenheiro de HPC, e **ficam em espera**: não estão descartadas, mas não são o rumo que escolhi agora.

O plano é da minha **carreira**, não de um emprego: quero ser dos melhores na área em que estudo e opero, que é **desenvolvimento com IA**. O rumo é IA aplicada no centro, com full stack e um DevOps enxuto em volta. A ordem candidata, a confirmar quando a Fase 0 fechar:

| Fase | Tema | Por que, na carreira | Pronto quando |
| --- | --- | --- | --- |
| A | IA aplicada: API de LLM, prompt, ferramentas (tool use), agentes, RAG, avaliação | é a área que mais cresce e a que eu quero dominar | construo um agente pequeno que chama uma ferramenta minha e sei medir se ele acerta |
| B | TypeScript e Node.js | a linguagem mais usada para pôr IA em produto web | escrevo uma API pequena tipada, sem consultar o básico |
| C | SQL e PostgreSQL | todo sistema guarda dado; modelagem e permissões separam o júnior do sênior | modelo três tabelas, escrevo os joins e explico uma política de acesso |
| D | DevOps enxuto: Docker e GitHub Actions | quem põe no ar o que construiu entrega sozinho | subo a API da Fase B num container e o CI roda os testes |
| E | Testes automatizados | código, e IA principalmente, só vale verificado | a API da Fase B tem testes que falham quando eu quebro algo |

A IA vem primeiro porque é o que mais quero, mas as fases A e B podem andar juntas (a A precisa de um pouco de código).

**Carreira da Alura para a Fase A (decidido em 10/11/2026):** [Engenharia de Agentes de IA](https://www.alura.com.br/carreiras/engenharia-de-ia), só o nível Base (Python para IA) e o Nível 1 (agentes com RAG), com o checkpoint do nível. Os Níveis 2 (ML, deep learning) e 3 (MLOps) ficam fora por enquanto. Da [AI-Native Software Engineering](https://www.alura.com.br/carreiras/ai-native-software-engineering), só cursos avulsos (engenharia de contexto, MCP) quando fizer falta. A [Arquitetura de Soluções com IA](https://www.alura.com.br/carreiras/arquitetura-de-solucoes-com-ia) fica para mais tarde, na senioridade. Antes de começar: conferir a ementa curso a curso na Alura (a escolha foi feita só pela página de cada carreira).

**Fio condutor: `tutor/`.** Um agente que lê `contexto/` e `DIARIO.md` e me faz perguntas sobre meus pontos fracos. A: script com ferramenta, RAG e avaliação (% de acerto) → B: API em TypeScript → C: Postgres guardando o histórico → D: Docker e CI rodando a avaliação → E: testes, com a avaliação como regressão. Cada fase fecha com uma tag git; resultados em `tutor/resultados.csv`.

**Na última semana da Fase 0:** reler esta tabela, confirmar a ordem e atualizar o `CLAUDE.md` (fase atual).

---

# Trilha HPC (em espera)

As Fases 1 a 6 abaixo eram o plano original para virar engenheiro de HPC. Ficam guardadas como estavam, caso eu volte a elas.

## Fase 1 · Linguagem C e como o computador funciona (semanas 7 a 18)

Objetivo: entender memória, ponteiros e compilação. É a base de todo código de HPC, e o C deixa isso exposto como nenhuma outra linguagem.

**Na Alura (semanas 7 a 12)**

- [ ] Cursos da [categoria Linguagem C](https://www.alura.com.br/cursos-online-back-end/linguagem-c), na ordem: de "C: conhecendo a Linguagem das Linguagens" até "C: recursos avançados da linguagem"

**Por fora (semanas 13 a 18)**

- [ ] [CS50x 2026](https://www.freecodecamp.org/news/harvard-cs50-2026-free-computer-science-university-course/), de Harvard: aulas 1 a 5 (C, Arrays, Algorithms, Memory, Data Structures). Grátis, com exercícios corrigidos automaticamente. A aula 4 (Memory) é a mais importante pra você.

**Mini-projeto (o fio condutor do plano):** um programa em C que multiplica duas matrizes 1000 × 1000 e mede o tempo. Guarde no GitHub. Nas próximas fases você vai acelerar esse mesmo programa com cada técnica nova, e a comparação final vira seu portfólio.

**Pronto pra avançar quando:** você explica o que é um ponteiro, usa `malloc` e `free` sem vazar memória e compila com `gcc` pelo terminal.

## Fase 2 · C++ e performance (semanas 19 a 30)

Objetivo: escrever C++ moderno e entender por que um código é lento. Em HPC, o gargalo quase sempre é a memória (cache), não o processador.

**Na Alura (semanas 19 a 26)**

- [ ] [Formação C++](https://www.alura.com.br/videos/sobre-a-formacao-c--c793), na ordem, terminando em [C++: performance e otimização](https://www.alura.com.br/curso-online-c-plus-plus-performance-otimizacao)

**Por fora (semanas 27 a 30)**

- [ ] [Algorithms for Modern Hardware](https://en.algorithmica.org/hpc/), livro online grátis: leia os capítulos sobre arquitetura da CPU, memória e cache. Está em inglês, vá devagar.
- [ ] MIT Missing Semester: a aula de Debugging and Profiling, pra aprender a medir antes de otimizar.

**Mini-projeto:** reescreva a multiplicação de matrizes em C++. Acelere só mudando a ordem dos loops e dividindo em blocos (tiling). O livro tem um [capítulo inteiro sobre isso](https://en.algorithmica.org/hpc/algorithms/matmul/). Anote o tempo antes e depois.

**Pronto pra avançar quando:** você consegue explicar por que percorrer uma matriz por linha é mais rápido que por coluna.

## Fase 3 · Paralelismo em CPU com OpenMP (semanas 31 a 40)

Objetivo: usar todos os núcleos de uma máquina ao mesmo tempo. O OpenMP é o padrão da indústria pra isso em C e C++. A partir daqui o estudo é quase todo fora da Alura.

**Por fora (núcleo da fase)**

- [ ] [Introduction to OpenMP](https://www.openmp.org/wiki/Tutorial), de Tim Mattson (Intel): série de vídeos curtos com exercícios. A Princeton considera essa a melhor explicação de OpenMP que existe ([fonte](https://researchcomputing.princeton.edu/education/external-online-resources/openmp)).
- [ ] Livro de apoio: *An Introduction to Parallel Programming*, de Peter Pacheco. Use os capítulos de memória compartilhada como consulta, não precisa ler inteiro.

**Na Alura (opcional, só se você já programa em Java)**

- [ ] [Threads em Java 1](https://www.alura.com.br/curso-online-threads-java-1) e Threads em Java 2: programação paralela. Os conceitos (sincronização, deadlock) valem pra qualquer linguagem.

**Conceitos que você precisa dominar:** speedup, lei de Amdahl, condição de corrida (race condition), redução, escalonamento de loops.

**Mini-projeto:** paralelize sua multiplicação de matrizes com OpenMP. Rode com 1, 2, 4 e 8 threads e faça um gráfico do speedup.

**Pronto pra avançar quando:** você explica por que dobrar as threads quase nunca dobra a velocidade.

## Fase 4 · Clusters com MPI e Slurm (semanas 41 a 52)

Objetivo: sair de uma máquina para várias. O MPI faz programas conversarem entre máquinas; o Slurm é o agendador que distribui os trabalhos (jobs) num cluster. Juntos, são o dia a dia de quem trabalha com HPC.

**Por fora (núcleo da fase)**

- [ ] [HPC Carpentry: Introduction to HPC](https://carpentries-incubator.github.io/hpc-intro/), grátis: conectar num cluster, transferir arquivos e enviar jobs com Slurm.
- [ ] [mpitutorial.com](https://mpitutorial.com/tutorials/), grátis: comunicação ponto a ponto e coletiva, com código de exemplo. Pede C e Linux, que você já terá.
- [ ] Pacheco, capítulo de MPI, como consulta.

**Na Alura (apoio)**

- [ ] [Formação Scripting](https://www.alura.com.br/formacao-scripting-automatizando-tarefas-devops): Bash mais avançado, útil pra escrever scripts de job.
- [ ] Containers e Docker: você vai precisar pra montar o laboratório abaixo.

**Seu laboratório em casa (sem precisar de supercomputador)**

- Instale o OpenMPI no Linux/WSL: roda vários processos MPI na mesma máquina, como se fossem nós diferentes.
- Suba um cluster Slurm de brinquedo com o [slurm-docker-cluster](https://github.com/giovtorres/slurm-docker-cluster), que cria um controlador e dois nós de computação em containers.

**Mini-projeto:** versão MPI da multiplicação de matrizes, dividindo as linhas entre processos. Escreva um script de job Slurm e rode no seu cluster de brinquedo.

**Pronto pra avançar quando:** você escreve um `sbatch` do zero e explica a diferença entre OpenMP (memória compartilhada) e MPI (troca de mensagens).

## Fase 5 · GPU, CUDA e a base de IA (semanas 53 a 66)

Objetivo: programar a GPU e entender o que um modelo de IA faz com ela. Treinar e rodar modelos é, no fundo, multiplicar matrizes gigantes, exatamente o que você vem acelerando desde a Fase 1.

**Na Alura (semanas 53 a 57): a base de Python e IA**

- [ ] Python para Data Science: primeiros passos (pule se já domina Python)
- [ ] NumPy: análise numérica eficiente com Python
- [ ] [Treinando uma Rede Neural: Deep Learning com PyTorch](https://www.alura.com.br/curso-online-treinando-rede-neural-pytorch)

**Por fora (semanas 58 a 66): CUDA**

- [ ] [An Even Easier Introduction to CUDA](https://courses.nvidia.com/courses/course-v1:DLI+T-AC-01+V1/about), da NVIDIA: grátis, 1 h.
- [ ] Entre no NVIDIA Developer Program (grátis) e ganhe um [curso pago de graça](https://www.nvidia.com/en-us/training/self-paced-courses/). Escolha Fundamentals of Accelerated Computing with CUDA Python (8 h, usa Numba e NumPy).
- [ ] [GPU MODE](https://www.youtube.com/@GPUMODE): as 15 primeiras palestras formam uma trilha de cerca de 20 h de CUDA, focada nos kernels por trás dos LLMs ([fonte](https://www.beri.net/learning/gpu-mode-lectures)). Tem comunidade no Discord.
- [ ] Livro de referência: *Programming Massively Parallel Processors* (Hwu, Kirk e El Hajj), o livro que o GPU MODE segue.

**Sem GPU em casa?** O Google Colab tem GPU no plano gratuito, com limite de uso. Dá pra fazer quase toda a fase lá.

**Mini-projeto:** multiplicação de matrizes em CUDA. Compare com sua melhor versão de CPU e com o `torch.matmul` do PyTorch, e perfile com o Nsight. Aqui vale pedir ao Claude Code três variações de kernel e descobrir, com o profiler, qual ganha e por quê.

**Pronto pra avançar quando:** você explica threads, blocos e memória compartilhada da GPU, e por que copiar dados entre CPU e GPU pode anular o ganho.

## Fase 6 · HPC para IA, dados e portfólio (semanas 67 a 78)

Objetivo: juntar tudo onde o mercado está hoje, que é treinar e servir modelos em várias GPUs e várias máquinas. Aqui o MPI da Fase 4 e o CUDA da Fase 5 viram uma coisa só.

**Por fora (núcleo da fase)**

- [ ] [Getting Started with Distributed Data Parallel](https://docs.pytorch.org/tutorials/intermediate/ddp_tutorial.html), tutorial oficial do PyTorch: treinar um modelo em várias GPUs e máquinas. O DDP sincroniza os gradientes com comunicação coletiva, a mesma ideia do MPI. A [página de tutoriais distribuídos](https://docs.pytorch.org/tutorials/distributed/home.html) tem uma série em vídeo pra começar.
- [ ] Opcional pago: Scaling Workloads Across Multiple GPUs with CUDA C++ (NVIDIA DLI, 4 h, US$ 30).

**Na Alura**

- [ ] [Spark com PySpark](https://www.alura.com.br/conteudo/spark-pyspark-processamento-modelagem): processamento de dados distribuído num cluster. É o lado "dados" do HPC.
- [ ] Retome suas carreiras de IA (Engenharia de IA ou Engenharia de Machine Learning), priorizando os cursos sobre levar modelos para produção.

**Mini-projeto final**

1. Treine um modelo pequeno com DDP em 2 processos (no Colab ou numa GPU alugada por hora) e compare o tempo com 1 processo.
2. Feche o repositório `hpc-estudos` com um README e um gráfico comparando todas as versões da multiplicação de matrizes: C, C++ otimizado, OpenMP, MPI, CUDA e PyTorch.
3. Escreva um post no LinkedIn contando o que aprendeu em cada versão. Esse repositório é seu portfólio.

**Pronto quando:** você explica como os gradientes são sincronizados entre GPUs (all-reduce) e liga isso ao que aprendeu de MPI.

## Comunidade de HPC, eventos e o que vem depois (em espera)

A comunidade de HPC no Brasil é pequena, e é nela que aparecem contatos e vagas. Comece a frequentá-la antes de se sentir pronto.

- **ERAD (Escolas Regionais de Alto Desempenho, da SBC):** acontecem todo ano em várias regiões. Em 2026 teve a do [Sul](https://sol.sbc.org.br/index.php/eradrs/issue/view/1689) em maio, em Bagé; a do [Nordeste](https://sol.sbc.org.br/index.php/erad-ne) em julho, em Recife; e a do [Centro-Oeste](https://sol.sbc.org.br/index.php/eradco/issue/view/1754) em setembro, em Campo Grande. Meta: ir a uma edição de 2027, por volta da Fase 3 ou 4.
- **Livros de minicursos da ERAD:** saem em ebook gratuito na SBC OpenLib ([edição 2025](https://sol.sbc.org.br/index.php/eradrs/issue/view/1508)). É material de HPC em português, ótimo para as fases 3 a 5.
- **Discord:** o do GPU MODE (GPU e IA) e o da Alura (dúvidas do dia a dia).
- **Revisão a cada 3 meses:** releia este plano, marque o que fez e ajuste o ritmo.

**Depois das 78 semanas**, escolha onde se aprofundar: HPC para IA (clusters de GPU, treino e inferência de modelos), computação científica (simulação e pesquisa) ou infraestrutura de clusters (administrar e automatizar supercomputadores).

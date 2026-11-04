# Anotações · Fase 0 · Terminal e Linux

Curso: [Sistema Operacional Linux: fundamentos e administração prática](https://www.alura.com.br/curso-online-linux-operacoes-fundamentos-comandos) (Alura, Leonardo Martins)

Ambiente: Fedora 44. Diferenças do curso (se ele usar Ubuntu) ficam marcadas com **Fedora:**.

## Aula 1 · Fundamentos: história, distribuições, boot e interfaces ✅ concluída em 2026-11-04

**Resumo da aula (Alura):**

- A origem e evolução do Linux e seu modelo de desenvolvimento colaborativo.
- O conceito de software livre e a licença GPL.
- O papel das comunidades de desenvolvedores na evolução do Linux.
- A utilização da linha de comando no Linux.
- As diferentes distribuições de Linux e suas características.
- A aplicação do Linux em diversas áreas e dispositivos.
- O processo de inicialização do Linux, incluindo BIOS, GRUB e INIT.
- As interfaces gráficas comuns no Linux e o uso do terminal.

**Pendente:** explicar com minhas palavras o que é software livre e a licença GPL.

### História

- **1969:** nasce o Unix, nos laboratórios Bell (AT&T). O Linux é inspirado nele, mas não é o Unix.
- **1991:** Linus Torvalds, estudante na Finlândia, cria o **kernel** Linux.
- **Kernel** = o núcleo do sistema. É ele que conversa com o hardware (CPU, memória, disco) e divide esses recursos entre os programas.
- "Linux" é só o kernel. Kernel + ferramentas + programas = uma **distribuição**.

### Distribuições

| Distro | Para quem / filosofia |
| --- | --- |
| Debian | Estabilidade e software livre; mantida pela comunidade; base do Ubuntu |
| Ubuntu | Facilidade, bom para quem tem pouca experiência em Linux (baseado no Debian) |
| Slackware | A mais antiga ainda viva; simples e "à moda Unix", configurada na mão; para quem já sabe |
| Red Hat (RHEL) | Empresarial: servidores, suporte pago, foco em estabilidade. Não é "leve" |

- **Família Red Hat:** Fedora (o que eu uso), RHEL, Rocky Linux. A maioria dos clusters de HPC roda Rocky ou RHEL.
- Erro que cometi: achei que Slackware e Red Hat eram "leves". Slackware é simples, Red Hat é corporativa.

### Fluxo de boot

```
Liga o PC
   │
   ▼
BIOS / UEFI ── testa o hardware e procura um disco para dar boot
   │
   ▼
GRUB ───────── gerenciador de boot: mostra o menu e carrega o kernel na memória
   │
   ▼
Kernel ─────── assume o hardware (CPU, memória, discos)
   │
   ▼
INIT ───────── primeiro processo (PID 1); sobe os serviços e a tela de login
               (no Fedora o INIT é o systemd)
```

- Erro que cometi: pus o INIT primeiro. O INIT é o **último**, porque é um programa e precisa do kernel já rodando.
- Truque para lembrar: cada etapa carrega a próxima (BIOS acha o GRUB, GRUB carrega o kernel, kernel inicia o INIT).

### Interfaces

| | Interface gráfica (GUI) | Modo terminal (CLI) |
| --- | --- | --- |
| Para quem | Quem vem de outro sistema ou nunca usou Linux | Quem administra servidores e automatiza tarefas |
| Vantagem | Fácil, visual | Leve, rápida, dá para automatizar com scripts e usar remoto (SSH) |
| Desvantagem | Gasta CPU e memória | Curva de aprendizado; precisa saber os comandos |

- **Em HPC:** clusters não têm interface gráfica. Acesso só por terminal via SSH, porque cada pedaço de CPU e memória vai para os cálculos.
- **Meu ambiente de estudo:** Fedora com GUI, mas faço tudo no terminal para treinar como num cluster.

### Onde o Linux roda

- Celulares Android (o Android usa o kernel Linux)
- Multimídia de carro, smart TVs, roteadores, micro-ondas e outros dispositivos embarcados (embedded)
- Servidores e nuvem
- **Todos os 500 supercomputadores do TOP500** rodam Linux

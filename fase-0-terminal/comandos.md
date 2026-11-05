# Comandos · Fase 0

Todos os comandos vistos no curso de Linux, na ordem em que apareceram. Revisão completa no fim do curso.

## Aula 2 · Comandos e navegação

| Comando | O que faz | Exemplo | Cuidado |
|---|---|---|---|
| `man` | Abre o manual de um comando (setas navegam, `/palavra` busca, `q` sai) | `man pwd` | — |
| `pwd` | Mostra a pasta atual (*print working directory*) | `pwd` | — |
| `ls` | Lista o conteúdo da pasta | `ls -l` (detalhes), `ls -a` (ocultos) | — |
| `find` | Procura arquivos pelo nome, entrando nas subpastas | `find /var -name "*log"` | Pastas do sistema geram `Permission denied` |
| `cp` | Copia arquivo | `cp a.txt b.txt` | Pasta precisa de `-r` |
| `mv` | Move ou renomeia | `mv b.txt c.txt` | Sobrescreve o destino sem avisar |
| `rm` | Apaga | `rm a.txt` | Não vai para a lixeira. `rm -r` apaga pasta |
| `touch` | Cria arquivo vazio (ou atualiza a data) | `touch a.txt` | — |

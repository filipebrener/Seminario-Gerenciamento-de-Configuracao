# Seminario-SIN-221
## Linha de raciocínio
### Codeline-baseline-mainline
* **Item de configuração** - artefato(codigo-fonte, tabela banco).
* **Codeline** - linha de versão de um item de configuralççao
* **Baseline** - quais são as versões **estáveis** dos intens de configuração
* **Baselines** são criadas para dar a segurança que de tempos em tempos
* está sendo criada versões estáveis do sistema
* **Mainline** - nome do conjunto de **Baselines**

### Recursos de sistemas/ferramentas
*  Identificação de versões e releases
*  Gerenciamento de armazenamento
*  Registro de historico de alterações (oque mudou em cada versão)
*  Desenvolvimento independente (inclusive por pessoas diferentes)
*  Apoiar projetos (Voce pode ter diferentes projetos inclusive em paralelo)

### Gerenciamento de armazenamento usando deltas
Em termos de armazenamento, 
e de gerenciamento dessas versões
Você pode não querer armazenar toda a nova versão.
Por exemplo: 
* Então, cada versão criada farei uma nova cópia do arquivo ?
* pode começar ter problema com espaço de armazenamento
* Uma soliução é armazenar usando **delta**
* **Delta** - é oque alterou (oque entrou e oque saiu) de uma versão pra outra
* **Delta** assim como na matemática é a diferença apenas
* E assim voce pode recuperar qualquer versão
* manter original e delta com as alterações
* ou ficar com a nova versão e os deltas para recuperar as versôes anteriores
* versão atual disponível de uma forma mais rápida

### check-in e check-out
* apresentar atores
* apresentar banco de dados
* atores fazem check-out(git clone)
* atores fazem o check-in
* alguns itens de configuração estão sendo alterado 2 vezes
* o que acontece ?
* temos que fazer um **merge** das alterações
* lidar de diferentes formas
* se um fez o **check-out** primeiro mais ninguem faz
* deixar todo mundo fazer o **check-out** e depois fazer o **merge**
* risco das alterações serem incopatíveis

### branching e merging
* **Branch** - é usado pra ganhar tempo
* Codelines serão desenvolvidas em paralelo
* **merge** dificilmente será 100% automatizado
* Oque está estavel nas duas verões não necessariamente
* ao juntar tudo vai estar estável tambem
* ferramentas precisam de um apoio do desenvolvedor
* para que ele ajude a indentificar se as alterações serão compatíveis

### passar para o guilherme
* Toda esse gerenciamentode versão tem como o objetivo criar um sistema
* que é oque o guilherme vai explicar um pouco pra gente agora

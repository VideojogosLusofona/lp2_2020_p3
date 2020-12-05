<!--
Projeto 3 de Linguagens de Programação II 2020/2021 (c) by Nuno Fachada

Projeto 3 de Linguagens de Programação II 2020/2021 is licensed under a
Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.

You should have received a copy of the license along with this
work. If not, see <http://creativecommons.org/licenses/by-nc-sa/4.0/>.
-->

# Projeto 3 de Linguagens de Programação II 2020/2021

_Projeto alternativo para alunos que não estejam a fazer DJD2 nem AP1, ou que
simplesmente prefiram realizar este projeto._

## Descrição do projeto

Os alunos devem implementar o jogo *[Felli]* para dois jogadores.

O jogo deve ser implementado em consola (.NET Core 3.1) e em Unity. A lógica,
regras e dados do jogo (o chamado **modelo**), devem ser completamente
independentes tanto da interface de consola (`WriteLines`, `ReadLines`), como
do Unity. Este modelo deve ser obrigatoriamente o mesmo em ambas as
implementações, devendo ser partilhado de uma forma que não implique
copiar os ficheiros de um lado para o outro. Existem formas de fazer isto ao
nível do C\# ou até ao nível do Git.

O [Model-View-Controller (MVC)][MVC] *design pattern* ou um dos seus derivados,
são bons pontos de partida para a realização deste projeto. Por exemplo,
[neste projeto Unity][ia-simplexity], o modelo é completamente
independente do Unity, sendo trivial implementar uma versão em consola.

Será muito valorizada a implementação de uma IA que consiga jogar contra um
jogador humano. No entanto esta é totalmente opcional.

Os grupos podem ter entre 2 a 3 elementos.

## Objetivos e critério de avaliação

O projeto tem um peso de 3 valores na componente prática de LP2. A nota final
do projeto será atribuída segundo os seguintes critérios:

* O projeto deve estar devidamente organizado, fazendo uso de classes,
  `struct`s e/ou enumerações, consoante seja mais apropriado. Cada tipo
  (i.e., classe, `struct` ou enumeração) deve ser colocado num ficheiro com o
  mesmo nome. Por exemplo, uma classe chamada `Player` deve ser colocada no
  ficheiro `Player.cs`.
* A escolha da coleções e *design patterns* deve ser adequada a cada
  situação. Serão privilegiadas soluções que tenham em consideração bons
  princípios de design de classes, como é o caso dos princípios [SOLID].
  Estes *patterns* e princípios devem ser balanceados com o princípio
  [KISS], crucial no desenvolvimento de qualquer aplicação.
* O código deve estar devidamente comentado e indentado.
* Não deve existir código "morto", que não faz nada, como por exemplo
  variáveis, propriedades ou métodos nunca usados.
* O projeto deve estar adequadamente documentado. Documentação deve ser feita
  com [comentários de documentação XML][XML], e a documentação (gerada em
  formato HTML ou CHM com [Doxygen], [DocFX] ou ferramenta similar)
  deve estar incluída no ZIP do projeto, mas **não** integrada no repositório
  Git.
* Repositório Git deve refletir boa utilização do mesmo, com *commits* de
  todos os elementos do grupo e mensagens de *commit* que sigam as melhores
  práticas para o efeito. Quaisquer *assets* binários, tais como imagens,
  devem ser integrados no repositório em modo Git LFS.
* Relatório em formato [Markdown] (ficheiro `README.md`), organizado da
  seguinte forma:
  * Título do projeto.
  * Autoria:
    * Nome dos autores (primeiro e último) e respetivos números de aluno.
    * Informação de quem fez o quê no projeto. Esta informação é
      **obrigatória** e deve refletir os *commits* feitos no Git.
    * Indicação do repositório público Git utilizado. Esta indicação é
      opcional, pois podem preferir desenvolver o projeto num repositório
      privado.
  * Arquitetura da solução:
    * Descrição da solução, com breve explicação de como o código foi
      organizado, coleções e *design patterns* utilizados (e justificação
      do seu uso), bem como dos algoritmos não triviais que tenham sido
      implementados.
    * Um diagrama UML de classes simples (i.e., sem indicação dos
      membros da classe) descrevendo a estrutura de classes. Podem e
      devem ser incluídos tipos do Unity caso isso facilite a compreensão
      do diagrama.
  * Referências, incluindo trocas de ideias com colegas, código aberto
    reutilizado (e.g., do StackOverflow) e bibliotecas de terceiros
    utilizadas. Devem ser o mais detalhados possível.
  * **Nota:** o relatório deve ser simples e breve, com informação mínima e
    suficiente para que seja possível ter uma boa ideia do que foi feito.
    Atenção aos erros ortográficos e à correta formatação [Markdown], pois
    ambos serão tidos em conta na nota final.

O projeto será avaliado de forma qualitativa, de forma semelhante ao [Projeto 1]
e ao [Projeto 2]. Isto significa que todos os objetivos têm de ser parcialmente
ou totalmente cumpridos. Em particular:

* **Não serão avaliados projetos que não cumpram os requisitos indicados na
  [Descrição do projeto](#descrição-do-projeto) ou que não funcionem.**

## Entrega

O projeto deve ser submetido no Moodle até às **23h00 de 27 de janeiro de
2021**. O projeto entregue deve ter os seguintes conteúdos:

* Pasta escondida `.git` com o repositório Git local do projeto.
* Documentação HTML ou CHM gerada com [Doxygen], [DocFX] ou
  ferramenta similar.
* Ficheiro `README.md` contendo o relatório do projeto em formato [Markdown].
* Ficheiros de imagens, contendo o diagrama UML de classes e outras figuras
  que considerem úteis. Estes ficheiros devem ser incluídos no repositório em
  modo Git LFS.

## Honestidade académica

Nesta disciplina, espera-se que cada aluno siga os mais altos padrões de
honestidade académica. Isto significa que cada ideia que não seja do
aluno deve ser claramente indicada, com devida referência ao respectivo
autor. O não cumprimento desta regra constitui plágio.

O plágio inclui a utilização de ideias, código ou conjuntos de soluções
de outros alunos ou indivíduos, ou quaisquer outras fontes para além
dos textos de apoio à disciplina, sem dar o respectivo crédito a essas
fontes. Os alunos são encorajados a discutir os problemas com outros
alunos e devem mencionar essa discussão quando submetem os projetos.
Essa menção **não** influenciará a nota. Os alunos não deverão, no
entanto, copiar códigos, documentação e relatórios de outros alunos, ou dar os
seus próprios códigos, documentação e relatórios a outros em qualquer
circunstância. De facto, não devem sequer deixar códigos, documentação e
relatórios em computadores de uso partilhado.

Nesta disciplina, a desonestidade académica é considerada fraude, com
todas as consequências legais que daí advêm. Qualquer fraude terá como
consequência imediata a anulação dos projetos de todos os alunos envolvidos
(incluindo os que possibilitaram a ocorrência). Qualquer suspeita de
desonestidade académica será relatada aos órgãos superiores da escola
para possível instauração de um processo disciplinar. Este poderá
resultar em reprovação à disciplina, reprovação de ano ou mesmo suspensão
temporária ou definitiva da ULHT.

*Texto adaptado da disciplina de [Algoritmos e
Estruturas de Dados][aed] do [Instituto Superior Técnico][ist]*

## Referências

* \[1\] **Felli**. Retrieved from <https://ludii.games/details.php?keyword=Felli>.
* \[2\] **Felli**. Retrieved from <https://en.wikipedia.org/wiki/Felli>.
* \[3\] Whitaker, R. B. (2016). **The C# Player's Guide** (3rd Edition).
  Starbound Software.
* \[4\] Albahari, J. (2017). **C# 7.0 in a Nutshell**. O’Reilly Media.
* \[5\] Nystrom, R. (2014). **Game Programming Patterns**. Genever Benning.
  Retrieved from <http://gameprogrammingpatterns.com/>.
* \[6\] Freeman, E., Robson, E., Bates, B., & Sierra, K. (2004). **Head First
  Design Patterns**. O'Reilly Media.
* \[7\] Dorsey, T. (2017). **Doing Visual Studio and .NET Code Documentation
  Right**. Visual Studio Magazine. Retrieved from
  <https://visualstudiomagazine.com/articles/2017/02/21/vs-dotnet-code-documentation-tools-roundup.aspx>.

## Licenças

Este enunciado é disponibilizado através da licença [CC BY-NC-SA 4.0].

## Metadados

* Autor: [Nuno Fachada]
* Curso:  [Licenciatura em Videojogos][lamv]
* Instituição: [Universidade Lusófona de Humanidades e Tecnologias][ULHT]

[Projeto 1]:https://github.com/VideojogosLusofona/lp2_2020_p1
[Projeto 2]:https://github.com/VideojogosLusofona/lp2_2020_p2
[Felli]:https://boardgamegeek.com/boardgame/70116/18-ghosts
[MVC]:https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller
[ia-simplexity]:https://github.com/VideojogosLusofona/color-shape-links-ai-competition
[Markdown]:https://guides.github.com/features/mastering-markdown/
[Doxygen]:https://www.stack.nl/~dimitri/doxygen/
[DocFX]:https://dotnet.github.io/docfx/
[KISS]:https://en.wikipedia.org/wiki/KISS_principle
[XML]:https://docs.microsoft.com/dotnet/csharp/codedoc
[SOLID]:https://en.wikipedia.org/wiki/SOLID
[CC BY-NC-SA 4.0]:https://creativecommons.org/licenses/by-nc-sa/4.0/
[lamv]:https://www.ulusofona.pt/licenciatura/videojogos
[Nuno Fachada]:https://github.com/fakenmc
[ULHT]:https://www.ulusofona.pt/
[aed]:https://fenix.tecnico.ulisboa.pt/disciplinas/AED-2/2009-2010/2-semestre/honestidade-academica
[ist]:https://tecnico.ulisboa.pt/pt/

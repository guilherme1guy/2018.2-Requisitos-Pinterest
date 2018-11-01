# Introdução

 A Técnica de modelagem por cenários consiste na elaboração de estruturas narrativas visando a construção de um contexto cujas informações permitam compreender ações desempenhadas no software, bem como os diversos fatores que influenciam essas ações, como o contexto, os recursos, elementos atuantes e etc. Essa técnica proporciona ainda uma forma de contextualização das funcionalidades desempenhadas em diferentes contextos de utilização do software analisado, trazendo elementos que auxiliam na compreensão da ideia abordada, permitindo uma forma direta de descrição.

# Cenários

## Cadastro de [usuário](lexicos.md#usuario)

|**Objetivo** |
|--|
| Cadastrar novo usuário no Pinterest |
|**Contexto** |
| Local: Página inicial do app [Pinterest](lexicos.md#pinterest) (quando não logado) <br>  Pré-Condição: não ter cadastro <br>  Pós-Condição: [usuário](lexicos.md#usuario) cadastrado  |
|**Atores** |
| [Usuário](lexicos.md#usuario) não cadastrado|
|**Recursos** |
| Internet, aplicativo, conta de e-mail|
|**Restrição**|
|O [usuário](lexicos.md#usuario) ter conta do facebook <br>  O [usuário](lexicos.md#usuario) ter conta no Google|
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> Senha inválida <br> E-mail inválido <br> Gmail ou Facebook fora do ar <br> Conta de Gmail ou Facebook inexistente |
|**Episódios** |
| [Usuário](lexicos.md#usuario) não cadastrado abre o aplicativo <br> [Usuário](lexicos.md#usuario) seleciona fazer o cadastro <br>  Se o [usuário](lexicos.md#usuario) tiver conta no Gmail , então selecionar cadastro pelo Gmail  <br> Se o [usuário](lexicos.md#usuario) tiver conta no Facebook , então selecionar cadastro pelo Facebook <br> Senão [usuário](lexicos.md#usuario) preenche e-mail, senha e confirmação da senha <br>[Usuário](lexicos.md#usuario) confirma cadastro no e-mail e é redirecionado para a página principal do [Pinterest](lexicos.md#pinterest)|

## Comentar em um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Criar comentário em um [Pin](lexicos.md#pin) |
|**Contexto** |
| Local: Página de detalhes de um [pin](lexicos.md#pin) <br>  Pré-Condição: o [usuário](lexicos.md#usuario) deve estar autenticado em sua conta  <br>  Pós-Condição: [usuário](lexicos.md#usuario) comentou e interagiu com o [pin](lexicos.md#pin) de outro [usuário](lexicos.md#usuario)|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de e-mail, [pin](lexicos.md#pin) |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Pin](lexicos.md#pin) ser apagado enquanto comentário é escrito |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) seleciona o [Pin](lexicos.md#pin) em que deseja comentar <br> [Usuário](lexicos.md#usuario) escreve seu comentário <br> [Usuário](lexicos.md#usuario) envia comentário |

## Compartilhar [Pasta](lexicos.md#pasta)

|Objetivo |
|--|
| Permitir que um ou mais [usuários](lexicos.md#usuario) tenham acesso a uma [pasta](lexicos.md#pasta), podendo editar os [Pins](lexicos.md#pin) existentes e adicionar novos. |
|**Contexto** |
| Local: [Página](lexicos.md#aba) da [pasta](lexicos.md#pasta) a ser [compartilhada](lexicos.md#compartilhar) <br> Tempo: A qualquer momento  <br> Pré-Condição: O [Usuário](lexicos.md#usuario) com quem a [pasta](lexicos.md#pasta) será compartilhada deverá possuir ou criar uma nova conta no Pinterest. <br>  Pós-Condição: Outro [usuário](lexicos.md#usuario) tem acesso ao conteúdo da [pasta](lexicos.md#pasta) compartilhada, podendo [organizar](lexicos.md#organizar) os [Pins](lexicos.md#pin) dessa [pasta](lexicos.md#pasta).|
|**Atores** |
| [Usuário](lexicos.md#usuario) proprietário da [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) com quem a [pasta](lexicos.md#pasta) será [compartilhada](lexicos.md#compartilhar)|
|**Recursos** |
| Internet <br> Conta no aplicativo <br>  [Pasta](lexicos.md#pasta) <br>  |
|**Restrição**|
| O [usuário](lexicos.md#usuario) [seguir outro usuário](#seguir-outro-usuario). |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Usuário](lexicos.md#usuario) ter sido bloqueado pelo outro <br> [Usuário](lexicos.md#usuario) recusar o [convite](lexicos.md#convite) para [colaborar](lexicos.md#colaborar) |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até a [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) seleciona a opção de [compartilhar](lexicos.md#compartilhar) <br> [Usuário](lexicos.md#usuario) escolhe o outro [usuário](lexicos.md#usuario) com quem compartilhar <br> [Usuário](lexicos.md#usuario) envia o [convite](lexicos.md#convite) para [colaboração](lexicos.md#colaborar) |

## Criar [Pasta](lexicos.md#pasta)

|Objetivo |
|--|
| Criar um local para guardar [pins](lexicos.md#pin) de um mesmo tema de escolha do [usuário](lexicos.md#usuario)|
|**Contexto** |
| Local: [Página](lexicos.md#aba) de [perfil](lexicos.md#perfil) <br> Tempo: A qualquer momento  <br> Pré-Condição:  [Usuário](lexicos.md#usuario) possuir [conta](lexicos.md#conta) no aplicativo. <br>  Pós-Condição: O [usuário](lexicos.md#usuario) agora contém uma [pasta](lexicos.md#pasta) para guardar seus [pins](lexicos.md#pin) de acordo com a classificação desejada.|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet <br> Conta no aplicativo |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Usuário](lexicos.md#usuario) ter sido bloqueado pelo outro  |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até seu [perfil](lexicos.md#perfil) <br> [Usuário](lexicos.md#usuario) seleciona a opção de criar nova [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) digita o nome que deseja dar à [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) escolhe se torna a [pasta](lexicos.md#pasta) [secreta](lexicos.md#pastaPrivada) ou não <br> [Usuário](lexicos.md#usuario) seleciona a opção criar <br> **Ou** <br> [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) seleciona um [pins](lexicos.md#pin) da página inicial <br> [Usuário](lexicos.md#usuario) seleciona a opção de [salvar](lexicos.md#salvar) [pin](lexicos.md#pin)  <br> [Usuário](lexicos.md#usuario) digita o nome que deseja dar à [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) escolhe a opção de criar [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) digita o nome que deseja dar à [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) escolhe se torna a [pasta](lexicos.md#pasta) [secreta](lexicos.md#pastaPrivada) ou não <br> [Usuário](lexicos.md#usuario) seleciona a opção criar <br> |

## Definir [interesses](lexicos.md#interesse)

|**Objetivo** |
|--|
| Escolher assuntos que são do [interesse](lexicos.md#interesse) do [usuário](lexicos.md#usuario) |
|**Contexto** |
| Local: Logo após o cadastro ou na aba de [interesses](lexicos.md#interesse) dentro da aba salvo <br>  Pré-Condição: estar [logado](lexicos.md#logado) <br>  Pós-Condição: [usuário](lexicos.md#usuario) recebe [pins](lexicos.md#pin) que são do seu [interesse](lexicos.md#interesse) no seu [feed](lexicos.md#feed)|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, [conta de usuário](lexicos.md#conta-de-usuario) |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Pinterest](lexicos.md#pinterest) não oferecer o interesse que o [usuário](lexicos.md#usuario) procura |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br>[Usuário](lexicos.md#usuario) visualiza página principal <br> [Usuário](lexicos.md#usuario) seleciona a aba "Salvos" <br> [Usuário](lexicos.md#usuario) aperta botão [interesses](lexicos.md#interesse) <br> [Usuário](lexicos.md#usuario) aperta botão "Adicionar [interesses](lexicos.md#interesse)" <br> [Usuário](lexicos.md#usuario) procura seus [interesses](lexicos.md#interesse) e os seleciona <br> [Usuário](lexicos.md#usuario) aperta "Concluído" |

## Editar um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Modificar um [pin](lexicos.md#pin) de acordo com a necessidade e desejo do dono da [conta](lexicos.md#perfil)|
|**Contexto** |
| Local: [Página](lexicos.md#página) de perfil do [usuário](lexicos.md#usuario) <br>  Pré-Condição: Conexão com a internet <br> Ter [pinado](lexicos.md#pinado), pelo menos, um [pin](lexicos.md#pin) <br> O [usuário](lexicos.md#usuario) deve estar [autenticado](lexicos.md#logado) em sua [conta](lexicos.md#conta) <br>  Pós-Condição: O [usuário](lexicos.md#usuario) contém um [pin](lexicos.md#pin) personalizado de acordo com seu interesse.|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, [pin](lexicos.md#pin)|
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash)
|**Episódios** |
| [Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica em sua página de [perfil](lexicos.md#perfil) no canto superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a aba [Pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) seleciona o [pin](lexicos.md#pin) que deseja editar <br> [Usuário](lexicos.md#usuario) clica no ícone de editar simbolizado por um lápis no canto superior esquerdo da tela. <br> **ou** <br> [Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica em sua página de [perfil](lexicos.md#perfil) no canto superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a aba [Pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) passa o mouse sobre o [pin](lexicos.md#pin) que deseja editar <br> [Usuário](lexicos.md#usuario) clica no ícone de editar simbolizado por um lápis na parte superior do [pin](lexicos.md#pin). <br> **ou** <br> [Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica em sua página de [perfil](lexicos.md#perfil) no canto superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a [aba](lexicos.md#aba) Pastas <br> [Usuário](lexicos.md#usuario) clica na pasta que está o [pin](lexicos.md#pin) que deseja editar <br> [Usuário](lexicos.md#usuario) passa o mouse sobre o [pin](lexicos.md#pin) que deseja editar <br> [Usuário](lexicos.md#usuario) clica no ícone de editar simbolizado por um lápis na parte superior do [pin](lexicos.md#pin). <br> **ou** <br> [Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica em sua página de [perfil](lexicos.md#perfil) no canto superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a [aba](lexicos.md#aba) "pastas" <br> [Usuário](lexicos.md#usuario) clica na [pasta](lexicos.md#pasta) que está o [pin](lexicos.md#pin) que deseja [editar](lexicos.md#editar) <br> [Usuário](lexicos.md#usuario) seleciona o [pin](lexicos.md#pin) que deseja [editar](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) clica no ícone de [editar](lexicos.md#editar) simbolizado por um lápis no canto superior esquerdo da tela.|

## Enviar um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Enviar um [Pin](lexicos.md#pin) para outro [usuário](lexicos.md#usuario) do [Pinterest](lexicos.md#pinterest) por meio de chat ou enviá-lo para outras pessoas que não utilizam o [Pinterest](lexicos.md#pinterest) por meio de outras redes sociais (WhatsApp, Facebook) ou até por SMS e e-mail |
|**Contexto** |
| Local: Página de detalhes de um [Pin](lexicos.md#pin) <br>  Pré-Condição: O [usuário](lexicos.md#usuario) deverá estar [logado](lexicos.md#logado) em sua conta do [Pinterest](lexicos.md#pinterest) <br>  Pós-Condição: O [Pin](lexicos.md#pin) é enviado a outro usuário. |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário, [pin](lexicos.md#pin) |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Pin](lexicos.md#pin) ser excluído ao ser enviado <br> [Usuário](lexicos.md#usuario) que for receber o [Pin](lexicos.md#pin) ter bloqueado o que for enviá-lo |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) entra na página inicial para visualizar e navegar pelo [feed](lexicos.md#feed) de [Pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) seleciona um [Pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) clica no botão Enviar <br> [Usuário](lexicos.md#usuario) escolhe a forma de envio <br> [Usuário](lexicos.md#usuario) enviar o [Pin](lexicos.md#pin) para outra pessoa |

## Fazer [login](lexicos.md#login)

|**Objetivo**|
|--|
|Utilizar todas as ferramentas exclusivas para usuários [logados](lexicos.md#login)|
|**Contexto**|
|Local: Pagina inicial do [Pinterest](lexicos.md#Pinterest) <br> Pré-Condição: Estar [cadastrado](), inserir o e-mail e a senha corretos <br>  Pós-Condição: O [usuário](lexicos.md#usuario) está [logado](lexicos.md#logado)|
|**Atores**|
|[Usuário](lexicos.md#usuario) cadastrado|
|**Recursos**|
|E-mail válido|
|**Restrição**|
| - |
|**Exceção**|
|Esquecer a senha <br> Esquecer o e-mail <br> Não ter cadastro|
|**Episódios**|
|Inicializar o [Pinterest](lexicos.md#pinterest) <br> Inserir e-mail <br> Clicar em "Continuar"|


## Ir para a fonte de um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Saber de qual site o [pin](lexicos.md#pin) está sendo enviado|
|**Contexto** |
| Local: Ao clicar em um [pin](lexicos.md#pin) ou passar o mouse sobre ele <br> Pré-Condição: Estar conectado à internet <br> Ser cadastrado no [Pinterest](lexicos.md#pinterest) <br>  Pós-Condição: O [usuário](lexicos.md#usuario) é direcionado para outra página na Internet que publicou o conteúdo do [pin](lexicos.md#pin) originalmente.|
|**Atores** |
| [Usuário](lexicos.md#usuario)|
|**Recursos** |
| Internet, aplicativo, [conta](lexicos.md#conta) de [usuário](lexicos.md#usuario) |
|**Restrição**|
| Ser um [link](lexicos.md#link) válido |
|**Exceção** |
| Falta de internet <br> Página fonte excluída antes do clique no [link](lexicos.md#link) da página|
|**Episódios** |feed
| [Usuário](lexicos.md#usuario) abre o aplicativo  <br> [Usuário](lexicos.md#usuario) faz o [login](lexicos.md#login)<br> [Usuário](lexicos.md#usuario) clica em um [pin](lexicos.md#pin)<br> [Usuário](lexicos.md#usuario) clica no botão com o link para o site fonte no canto inferior direito da página <br> **ou** <br>  [Usuário](lexicos.md#usuario) abre o aplicativo  <br> [Usuário](lexicos.md#usuario) faz o [login](lexicos.md#login)<br> [Usuário](lexicos.md#usuario) passa o mouse sobre um [pin](lexicos.md#pin)<br> [Usuário](lexicos.md#usuario) clica no botão com o link para o site fonte no canto inferior direito da [pin](lexicos.md#pin)<br>|

## Organizar [Pasta](lexicos.md#pasta)

|Objetivo |
|--|
| Realocar [pins](lexicos.md#pin) em [pastas](lexicos.md#pasta) ou [subpastas](lexicos.md#subpasta) e excluir [pins](lexicos.md#pin)|
|**Contexto** |
| Local: [Página](lexicos.md#aba) da [pasta](lexicos.md#pasta) a ser organizada <br> Tempo - A qualquer momento  <br> Pré-Condição: O [Usuário](lexicos.md#usuario) deve possuir [pins](lexicos.md#pin) na [pasta](lexicos.md#pasta) a ser organizada ou na [subpasta](lexicos.md#subpasta) a ser organizada  <br>  Pós-Condição: A [pasta](lexicos.md#pasta) e/ou a [subpasta](lexicos.md#pasta) estão organizadas de acordo com o interesse do [usuário](lexicos.md#usuario)|
|**Atores** |
| [Usuário](lexicos.md#usuario) proprietário da [pasta](lexicos.md#pasta) <br> [Usuários](lexicos.md#usuario) com quem a [pasta](lexicos.md#pasta) foi [compartilhada](lexicos.md#compartilhar)|
|**Recursos** |
| Internet <br> Conta no aplicativo <br>  [Pasta](lexicos.md#pasta) <br> [Subpastas](lexicos.md#subpasta) <br> [Pins](lexicos.md#pin) na [Pasta](lexicos.md#pasta) <br> |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até a [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) seleciona a opção de organizar [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) seleciona o [pin](lexicos.md#pin) que deseja modificar <br> [Usuário](lexicos.md#usuario) decide entre [excluir](lexicos.md#excluir), [mover](lexicos.md#mover) para [pasta](lexicos.md#pasta) ou para [subpasta](lexicos.md#subpasta)|

## [Pesquisar](lexicos.md#pesquisa) por tema

|**Objetivo** |
|--|
| Encontrar imagens referentes a um tema de preferência do usuário |
|**Contexto** |
| Local: [Página](lexicos.md#aba) inicial do aplicativo versão mobile <br> Tempo: a qualquer momento  <br> Pré-Condição: usuário ter em mente palavras-chaves relativas ao tema  <br>  Pós-Condição: O [usuário](lexicos.md#usuario) encontrará uma [página](lexicos.md#aba) repleta de [pins](lexicos.md#pin) de acordo com a temática desejada|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet <br> Conta no aplicativo <br>|
|**Restrição**|
| O conteúdo retornado pela pesquisa deve ter relação com o termo [pesquisado](lexicos.md#pesquisa). |
|**Exceção** |
| Palavras que coincidirem com outros temas <br> Internet cair <br> App dar [crash](lexicos.md#crash) <br> |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) escreve palavras relacionadas ao tema desejado na [barra de pesquisa](lexicos.md#barraDepesquisa) <br> [Usuário](lexicos.md#usuario) clica "enter" <br> Aplicativo mostra uma seleção de imagens referentes ao tema <br> Aplictivo mostra uma seleção de palavras relacionadas ao tema que direcione para pesquisas específicas|

## [Pesquisar](lexicos.md#pesquisa) por foto

|**Objetivo** |
|--|
| Utilizar o recurso de fotografar imagens para [pesquisar](lexicos.md#pesquisa) por imagens semelhantes |
|**Contexto** |
| Local: [Página](lexicos.md#aba) inicial do aplicativo versão mobile <br> Tempo - A Qualquer momento  <br> Pré-Condição: Celular possuir câmera <br>  Pós-Condição: O [usuário](lexicos.md#usuario) encontrará uma [página](lexicos.md#aba) repleta de [pins](lexicos.md#pin) que possuam semelhança com as características da foto detectadas pelo [Pinterest](lexicos.md#pinterest)|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet <br> Conta no aplicativo <br> Celular com câmera |
|**Restrição**|
| O conteúdo retornado pela [pesquisa](lexicos.md#pesquisa) deve estar relacionado à foto pesquisada. <br> A Foto possuir boa qualidade gráfica. <br> Existirem muitos [pins](#lexicos.md#pin) semelhantes à foto tirada.  |
|**Exceção** |
| Câmera não funcionar <br> Internet cair <br> App dar [crash](lexicos.md#crash) <br> |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> O [usuário](lexicos.md#usuario) visualiza [pagina](lexicos.md#aba) inical. <br> [Usuário](lexicos.md#usuario) seleciona o ícone de câmera na [barra de pesquisa](lexicos.md#barraDepesquisa) <br> [Usuário](lexicos.md#usuario) tira foto da imagem por qual busca semelhantes <br> Aplicativo mostra uma seleção de imagens semelhantes à enviada pelo [Usuário](lexicos.md#usuario)  |

## Seguir outro [usuário](lexicos.md#usuario)

|**Objetivo** |
|--|
| [Seguir](lexicos.md#seguir) um outro [Usuário](lexicos.md#usuario) para acompanhar sua atividade no [Pinterest](lexicos.md#pinterest) |
|**Contexto** |
| Local: Perfil de um [usuário](lexicos.md#usuario) <br>  Pré-Condição: o [usuário](lexicos.md#usuario) não pode [seguir](lexicos.md#seguir) a si mesmo  <br>  Pós-Condição: O [usuário](lexicos.md#usuario) [logado](lexicos.md#logado) poderá acompanhar os [pins](lexicos.md#pin) de outro [usuário](lexicos.md#usuario)|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Usuário](lexicos.md#usuario) ter sido bloqueado pelo outro [usuário](lexicos.md#usuario) que deseja [seguir](lexicos.md#seguir) |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até a página do perfil de outro [Usuário](lexicos.md#usuario) <br> [Usuário](lexicos.md#usuario) aperta botão [seguir](lexicos.md#seguir)|

## [Salvar](lexicos.md#pinar) um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| [Salvar](lexicos.md#pinar) um [Pin](lexicos.md#pin) em uma [pasta](lexicos.md#pasta) criada pelo [usuário](lexicos.md#usuario) do [Pinterest](lexicos.md#pinterest) |
|**Contexto** |
| Local: Página de detalhes de um [Pin](lexicos.md#pin) <br>  Pré-Condição: o [usuário](lexicos.md#usuario) deverá estar [logado](lexicos.md#logado) em sua conta do [Pinterest](lexicos.md#pinterest) <br>  Pós-Condição: O [Pin](lexicos.md#pin) é [salvo](lexicos.md#salvar) em uma [pasta](lexicos.md#pasta). |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, [conta de usuário](lexicos.md#conta-de-usuario), [pin](lexicos.md#pin) |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Pin](lexicos.md#pin) ser excluído ao ser [salvo](lexicos.md#salvar) <br> Não existir [pastas](lexicos.md#pasta) para [salvá-lo](lexicos.md#salvar) |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) entra na [página](lexicos.md#aba) inicial para visualizar e [navegar](lexicos.md#navegar) pelo [feed](lexicos.md#feed) de [Pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) seleciona um [Pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) clica no botão [Salvar](lexicos.md#salvar) <br> [Usuário](lexicos.md#usuario) escolhe a [pasta](lexicos.md#pasta) para [salvá-lo](lexicos.md#salvar) e se não houverem [pastas](lexicos.md#pasta) criadas, cria uma [pasta](lexicos.md#pasta) para poder [salvar](lexicos.md#salvar) o [Pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) [salvar](lexicos.md#salvar) o [Pin](lexicos.md#pin) na [pasta](lexicos.md#pasta) |

## Visualizar [Feed](lexicos.md#feed)

|**Objetivo** |
|--|
| Visualizar [pins](lexicos.md#pin) de [interesse](lexicos.md#interesse) do [usuário](lexicos.md#usuario) pelo [feed](lexicos.md#feed) |
|**Contexto** |
| Local: [Página](lexicos.md#aba) incial do [Pinterest](lexicos.md#pinterest) <br>  Pré-Condição: O [usuário](lexicos.md#usuario) deverá acessar o [Pinterest](lexicos.md#pinterest) caso queira visualizar algo de seu [interesse](lexicos.md#interesse) <br>  Pós-Condição: O [usuário](lexicos.md#usuario) visualizará o conteúdo da [página](lexicos.md#aba) inicial do [Pinterest](lexicos.md#pinterest)|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo |
|**Restrição**|
| Os [pins](lexicos.md#pin) devem obedecer os interesses do [usuário](lexicos.md#usuario) |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> O App não está atualizado frequentemente|
|**Episódios** |
| [Usuário](lexicos.md#usuario) acessa o [pinterest](lexicos.md#pinterest)  <br> [Usuário](lexicos.md#usuario) navega pelo [feed](lexicos.md#feed) de [pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) pesquisa [pins](lexicos.md#pin) de seu [interesse](lexicos.md#interesse) <br> [Usuário](lexicos.md#usuario) vizualiza o [pin](lexicos.md#pin) <br> |

## Visualizar aba [Seguindo](lexicos.md#feed)

|**Objetivo** |
|--|
| Visualizar [pins](lexicos.md#pin) de outros usuários que o [usuário](lexicos.md#usuario) [logado](lexicos.md#logado) segue
|**Contexto** |
| Local: [Aba](lexicos.md#aba) [seguindo](lexicos.md#seguindo) do [Pinterest](lexicos.md#pinterest) <br>  Pré-Condição: O [usuário](lexicos.md#usuario) deverá acessar o [Pinterest](lexicos.md#pinterest) caso queira publicado pelos demais usuários que segue <br>  Pós-Condição: O [usuário](lexicos.md#usuario) [logado](lexicos.md#logado) visualizará o conteúdo publicado pelos [usuários](lexicos.md#usuario) que está [seguindo](lexicos.md#seguir)|
|**Atores** |
| [Usuário](lexicos.md#usuario) [logado](lexicos.md#logado) <br> Usuários [seguidos](lexicos.md#seguir) pelo [usuário](lexicos.md#usuario) [logado](lexicos.md#logado)|
|**Recursos** |
| Internet, aplicativo |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br>|
|**Episódios** |
| [Usuário](lexicos.md#usuario) acessa o [pinterest](lexicos.md#pinterest)  <br> [Usuário](lexicos.md#usuario) navega pela [aba](lexicos.md#aba) [seguindo](lexicos.md#seguir)<br>  [Usuário](lexicos.md#usuario) vizualiza o conteúdo de cada [pin](lexicos.md#pin) <br> |

## Enviar mensagem para outros [usuários](lexicos.md#usuario)

|**Objetivo** |
|--|
| Poder se comunicar com outros [usuários](lexicos.md#usuario) por meio do [Pinterest](lexicos.md#pinterest) sendo por [mensagens](lexicos.md#mensagem) ou enviando [pins](lexicos.md#pin) |
|**Contexto** |
| Local: [Página](lexicos.md#aba) de [mensagens](lexicos.md#mensagem) <br>  Pré-Condição: O [usuário](lexicos.md#usuario) está [logado](lexicos.md#login) em sua conta do [Pinterest](lexicos.md#pinterest) <br>  Pós-Condição: O [usuário](lexicos.md#usuario) [logado](lexicos.md#logado) interagiu com outro [usuário](lexicos.md#usuario) que também está cadastrado no [Pinterest](lexicos.md#pinterest)|
|**Atores** |
| [Usuário](lexicos.md#usuario) e [usuários](lexicos.md#usuario) conhecidos|
|**Recursos** |
| Internet, aplicativo |
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [mensagem](lexicos.md#mensagem) não se entregue|
|**Episódios** |
| [Usuário](lexicos.md#usuario) [loga](lexicos.md#login) em seu [perfil](lexicos.md#perfil)  <br> [Usuário](lexicos.md#usuario) navega até o icone de [mensagem](lexicos.md#mensagem) <br> [Usuário](lexicos.md#usuario) procura por outro [usuários](lexicos.md#usuario) <br> [Usuário](lexicos.md#usuario) envia a [mensagem](lexicos.md#mensagem) <br> |

## Receber [notificações](lexicos.md#notificacao)

|**Objetivo** |
|--|
| Ser [notificado](lexicos.md#notificacao) sobre alguma interação de outros [usuários](lexicos.md#usuario) ou novos [pins](lexicos.md#pin) relacionados a um [pin](lexicos.md#pin) [pinado](lexicos.md#pinado) |
|**Contexto** |
| Local: [Página](lexicos.md#aba) de [notificações](lexicos.md#notificacao) <br> Pré-Condição: O [Usuário](lexicos.md#usuario) deve estar [logado](lexicos.md#login) na sua conta do [Pinterest](lexicos.md#pinterest) e ter algum [pin](lexicos.md#pin) [pinado](lexicos.md#pinado) ou [seguir](lexicos.md#seguir) algum outro [usuário](lexicos.md#usuario) <br>  Pós-Condição: O [usuário](lexicos.md#usuario) [logado](lexicos.md#logado) será [notificado](lexicos.md#notificacao) quando um outro [usuário](lexicos.md#usuario) interagir com ele|
|**Autores** |
| [Usuários](lexicos.md#usuario), [usuários](lexicos.md#usuario) seguido e o [Pinterest](lexicos.md#pinterest) |
|**Recursos** |
|Internet <br> Browser <br> Aplicativo <br>  [Seguir](lexicos.md#seguir) outro [usuário](lexicos.md#usuario) <br> [Pin](lexicos.md#pin) [pinado](lexicos.md#pinado) |
|**Restrição**|
| [Usuário](lexicos.md#usuario) não ter o app silenciado. |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br>  [Usuários](lexicos.md#usuario) [seguidos](lexicos.md#seguir) por um [usuário](lexicos.md#usuario) deixarem de segui-lo |
|**Episódios** |
|[Usuário](lexicos.md#usuario) acessa o [Pinterest](lexicos.md#pinterest) <br> [Usuário](lexicos.md#usuario) [pina](lexicos.md#pinar) um [pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) [segue](lexicos.md#seguir) outro [usuário](lexicos.md#usuario) <br> [Usuário](lexicos.md#usuario) clica em [notificações](lexicos.md#notificacao)  <br> [Usuário](lexicos.md#usuario) vê novas interações de outros [usuários](lexicos.md#usuario) e novos [pins](lexicos.md#pin) relacionados a um [pin](lexicos.md#pin) [pinado](lexicos.md#pinar)

## [Classificação](lexicos.md#classificar) de [pastas](#lexicos.md#pastas)
|**Objetivo** |
|--|
|Poder classificar as [pastas](lexicos.md#pasta) em cincos opções da preferência do [usuário](lexicos.md#usuario), sendo elas "Salvo pela última vez", "A a Z", "Igual à Web", "Mais antigas" e "Mais recentes" e assim as [pastas](lexicos.md#pasta) serão reorganizadas
| Local: Conjunto de [pastas](lexicos.md#pasta) <br> Pré-Condição: O [Usuário](lexicos.md#usuario) deve estar [logado](lexicos.md#login) na sua conta do [Pinterest](lexicos.md#pinterest) e ter mais de uma  [pasta](lexicos.md#pasta)  <br>  Pós-Condição: O [usuário](lexicos.md#usuario) consegue classificar suas [pastas](lexicos.md#pasta)|
|**Autores** |
| [Usuários](lexicos.md#usuario) |
|**Recursos** |
|Internet <br> Browser <br> Aplicativo <br> Ter mais de uma [pasta](lexicos.md#pasta) <br>  |
|**Restrição**|
| Ter mais de uma [pasta](lexicos.md#pasta) |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> |
|**Episódios** |
|[Usuário](lexicos.md#usuario) acessa o [Pinterest](lexicos.md#pinterest) <br> [Usuário](lexicos.md#usuario) clica no ícone de [perfil](lexicos.md#perfil) <br> [Usuário](lexicos.md#usuario) clica em um ícone <br> [Usuário](lexicos.md#usuario) clica no ícone de seta para baixo na parte superior direita da tela  <br> [Usuário](lexicos.md#usuario) escolhe entre as opções de classificação ("Salvo pela última vez", "A a Z", "Igual à Web", "Mais antigas" e "Mais recentes") |

## [Ocultar](lexicos.md#ocultar) um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| [Ocultar](lexicos.md#ocultar) um [pin](lexicos.md#pin) de uma [aba](lexicos.md#aba) do [Pinterest](lexicos.md#pinterest) para que o [usuário](lexicos.md#usuario) não visualize mais determinado conteúdo|
|**Contexto** |
| Local: Página de detalhes de um [Pin](lexicos.md#pin) <br>  Pré-Condição: o [usuário](lexicos.md#usuario) deverá estar [logado](lexicos.md#logado) em sua conta do [Pinterest](lexicos.md#pinterest) <br>  Pós-Condição: O [pin](lexicos.md#pin) não aparecerá mais para o [usuário](lexicos.md#usuario) em nenhuma das [abas](lexicos.md#aba) do [Pinterest](lexicos.md#pinterest) |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário, [pin](lexicos.md#pin) |
|**Restrição**|
| Que o [pin](lexicos.md#pin) não seja do interesse do [usuário](lexicos.md#usuario). |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Pin](lexicos.md#pin) ser excluído ao ser [ocultado](lexicos.md#ocultar) <br> |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) entra na página inicial para visualizar e navegar pelo [feed](lexicos.md#feed) de repleto de [pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) seleciona um [Pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) clica no botão [Ocultar](lexicos.md#ocultar) <br> [Pinterest](lexicos.md#pinterest) informa que [pins](lexicos.md#pin) com esse tipo de conteúdo não aparecerão mais para o [usuário](lexicos.md#usuario) <br> |

## [Denunciar](lexicos.md#denunciar) um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| [Denunciar](lexicos.md#denunciar) um [pin](lexicos.md#pin) presente em uma [aba](lexicos.md#aba) do [Pinterest](lexicos.md#pinterest)|
|**Contexto** |
| Local: Página de detalhes de um [Pin](lexicos.md#pin), na opção "Mais"<br>  Pré-Condição: o [usuário](lexicos.md#usuario) deverá estar [logado](lexicos.md#logado) em sua conta do [Pinterest](lexicos.md#pinterest) <br> O [usuário](lexicos.md#usuario) deverá encontrar um [pin](lexicos.md#pin) com conteúdo que julga como impróprio <br> Pós-Condição: O [pin](lexicos.md#pin) será encaminhado para a [comunidade](lexicos.md#comunidade) do [Pinterest](lexicos.md#pinterest) avaliar o conteúdo e não aparecerá mais para o [usuário](lexicos.md#usuario) em nenhuma das [abas](lexicos.md#aba) do [Pinterest](lexicos.md#pinterest) |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário, [pin](lexicos.md#pin) |
|**Restrição**|
| O [pin](lexicos.md#pin) ser inapropriado. |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) entra na página inicial para visualizar e navegar pelo [feed](lexicos.md#feed) repleto de de [pins](lexicos.md#pin) <br>  [Usuário](lexicos.md#usuario) encontra um [pin](lexicos.md#pin) com conteúdo impróprio <br> [Usuário](lexicos.md#usuario) seleciona um [Pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) clica no botão Mais <br>  [Usuário](lexicos.md#usuario) clica no botão [Denunciar](lexicos.md#denunciar) <br>  [Pinterest](lexicos.md#pinterest) informa que [pins](lexicos.md#pin) com esse tipo de conteúdo não aparecerão mais para o [usuário](lexicos.md#usuario) <br> [Comunidade](lexicos.md#comunidade) do [Pinterest](lexicos.md#pinterest) avalia o conteúdo do [pin](lexicos.md#pin) [denunciado](lexicos.md#denunciado) e remove o conteúdo do aplicativo |

## Classificar um [Pin](lexicos.md#pin) como [Experimentado](lexicos.md#experimentar)

|**Objetivo** |
|--|
| [Experimentar](lexicos.md#experimentar) o conteúdo de um [pin](lexicos.md#pin) e classificá-lo na [aba](lexicos.md#aba) do [Pinterest](lexicos.md#pinterest) de [Experimentados](lexicos.md#experimentar)|
|**Contexto** |
| Local: [Aba de Salvos](lexicos.md#abasalvos) do [Pinterest](lexicos.md#pinterest), na opção [Experimentados](lexicos.md#experimentar)<br>  Pré-Condição: o [usuário](lexicos.md#usuario) deverá estar [logado](lexicos.md#logado) em sua conta do [Pinterest](lexicos.md#pinterest) <br> O [usuário](lexicos.md#usuario) deverá [experimentar](lexicos.md#experimentar) na prática um [pin](lexicos.md#pin)<br> Pós-Condição: O [pin](lexicos.md#pin) ficará [salvo](lexicos.md#pinar) na [aba](lexicos.md#aba) [Experimentar](lexicos.md#experimentar) do [Pinterest](lexicos.md#pinterest) junto com uma foto do que foi [experimentado](lexicos.md#experimentar)|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário, [pin](lexicos.md#pin), câmera de celular e recursos do conteúdo a ser [experimentado](lexicos.md#experimentar) do [pin](lexicos.md#pin)|
|**Restrição**|
| O [usuário](lexicos.md#usuario) ter experimentado o conteúdo do pin na vida real. |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Usuário](lexicos.md#usuario) não ter os recursos exigidos pelo [pin](lexicos.md#pin) para [experimentá-lo](lexicos.md#experimentar)|
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) entra na [Aba Salvos](lexicos.md#abasalvos) <br>  [Usuário](lexicos.md#usuario) seleciona a opção [Experimentados](lexicos.md#experimentar) <br> [Pinterest](lexicos.md#pinterest) apresenta em lista os [pins](lexicos.md#pin) [salvos](lexicos.md#pinar) pelo [usuário](lexicos.md#usuario) <br>[Usuário](lexicos.md#usuario) seleciona a opção adicionar [pin](lexicos.md#pin)  <br> [Usuário](lexicos.md#usuario) tira foto do [pin](lexicos.md#pin) [experimentado](lexicos.md#experimentar) <br>  [Usuário](lexicos.md#usuario) inclui uma anotação a respeito de sua experiência <br> [Usuário](lexicos.md#usuario) seleciona a opção Concluído  |

## Sair do aplicativo [Pinterest](lexicos.md#pinterest)

|**Objetivo** |
|--|
| Sair de uma conta [logada](lexicos.md#logado)|
|**Contexto** |
| Local: [Aba de Salvos](lexicos.md#abasalvos) do [Pinterest](lexicos.md#pinterest), na opção da ignição <br>  Pré-Condição: o [usuário](lexicos.md#usuario) deverá estar [logado](lexicos.md#logado) em sua conta do [Pinterest](lexicos.md#pinterest) <br> Pós-Condição: O [usuário](lexicos.md#usuario) não estará mais [logado](lexicos.md#logado) no [Pinterest](lexicos.md#pinterest)|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário|
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br>|
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) entra na [Aba Salvos](lexicos.md#abasalvos) <br>  [Usuário](lexicos.md#usuario) seleciona a opção Ignição <br>[Usuário](lexicos.md#usuario) seleciona a opção Sair <br> [Usuário](lexicos.md#usuario) visualiza a [página](lexicos.md#aba) inicial de [login](lexicos.md#logado) do [Pinterest](lexicos.md#pinterest)<br>

## Editar [Perfil](lexicos.md#perfil)

|**Objetivo** |
|--|
| Alterar ou atualizar algum dado sobre o perfil do [usuário](lexicos.md#usuario)|
|**Contexto** |
| Local: [Página](lexicos.md#aba) de edição do [Pinterest](lexicos.md#pinterest) <br> Pré-Condição: Estar conectado à internet <br> Ser cadastrado no [Pinterest](lexicos.md#pinterest) <br>  Pós-Condição: O [usuário](lexicos.md#usuario) tem seus dados atualizados na sua [página](lexicos.md#aba) de perfil|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, [conta](lexicos.md#login) de usuário|
|**Restrição**|
| - |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br>|
|**Episódios** |
|[Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica na ignição superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a opção [perfil](lexicos.md#pefil) no canto superior esquerdo da [página](lexicos.md#pagina) de edição <br> O [Usuário](lexicos.md#usuario) muda seu nome e/ou sobrenome <br> **ou** <br> O [Usuário](lexicos.md#usuario) muda sua foto de [perfil](lexicos.md#perfil) <br> **ou**  <br> O [Usuário](lexicos.md#usuario) muda seu username <br> **ou** <br> O [Usuário](lexicos.md#usuario) adiciona ou muda a descrição sobre ele <br> **ou** <br> O [Usuário](lexicos.md#usuario) muda ou adiciona sua localização <br> **ou** <br> O [Usuário](lexicos.md#usuario) muda ou adiciona seu website, caso ele possua um

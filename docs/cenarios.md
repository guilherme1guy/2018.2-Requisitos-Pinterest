# Introdução

 A Técnica de modelagem por cenários consiste na elaboração de estruturas narrativas visando a construção de um contexto cujas informações permitam compreender ações desempenhadas no software, bem como os diversos fatores que influenciam essas ações, como o contexto, os recursos, elementos atuantes e etc. Essa técnica proporciona ainda uma forma de contextualização das funcionalidades desempenhadas em diferentes contextos de utilização do software analisado, trazendo elementos que auxiliam na compreensão da ideia abordada, permitindo uma forma direta de descrição.

# Cenários

## Cadastro de [usuário](lexicos.md#usuario)

|**Objetivo** |
|--|
| Cadastrar novo usuário no Pinterest |
|**Contexto** |
| Local: Página inicial do app [Pinterest](lexicos.md#pinterest) (quando não logado) <br>  Pré-Condição: não ter cadastro  |
|**Atores** |
| [Usuário](lexicos.md#usuario) não cadastrado|
|**Recursos** |
| Internet, aplicativo, conta de e-mail|
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> Senha inválida <br> E-mail inválido |
|**Episódios** |
| [Usuário](lexicos.md#usuario) não cadastrado abre o aplicativo <br> [Usuário](lexicos.md#usuario) seleciona fazer o cadastro <br> [Usuário](lexicos.md#usuario) preenche dados de cadastro <br> [Usuário](lexicos.md#usuario) confirma cadastro |

## Comentar em um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Criar comentário em um [Pin](lexicos.md#pin) |
|**Contexto** |
| Local: Página de detalhes de um [pin](lexicos.md#pin) <br>  Pré-Condição: o usuário deve estar autenticado em sua conta  |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de e-mail, [pin](lexicos.md#pin) |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Pin](lexicos.md#pin) ser apagado enquanto comentário é escrito |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) seleciona o [Pin](lexicos.md#pin) em que deseja comentar <br> [Usuário](lexicos.md#usuario) escreve seu comentário <br> [Usuário](lexicos.md#usuario) envia comentário |

## Compartilhar [Pasta](lexicos.md#pasta)

|Objetivo |
|--|
| Permitir que um ou mais [usuários](lexicos.md#usuario) tenham acesso a uma [pasta](lexicos.md#pasta), podendo editar os [Pins](lexicos.md#pin) existentes e adicionar novos. |
|**Contexto** |
| Local: [Página](lexicos.md#pagina) da [pasta](lexicos.md#pasta) a ser [compartilhada](lexicos.md#compartilhar) <br> Tempo: A qualquer momento  <br> Pré-Condição: O [Usuário](lexicos.md#usuario) com quem a [pasta](lexicos.md#pasta) será compartilhada deverá possuir ou criar uma nova conta no Pinterest.  |
|**Atores** |
| [Usuário](lexicos.md#usuario) proprietário da [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) com quem a [pasta](lexicos.md#pasta) será [compartilhada](lexicos.md#compartilhar)|
|**Recursos** |
| Internet <br> Conta no aplicativo <br>  [Pasta](lexicos.md#pasta) <br>  |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Usuário](lexicos.md#usuario) ter sido bloqueado pelo outro <br> [Usuário](lexicos.md#usuario) recusar o [convite](lexicos.md#convite) para [colaborar](lexicos.md#colaborar) |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até a [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) seleciona a opção de [compartilhar](lexicos.md#compartilhar) <br> [Usuário](lexicos.md#usuario) escolhe o outro [usuário](lexicos.md#usuario) com quem compartilhar <br> [Usuário](lexicos.md#usuario) envia o [convite](lexicos.md#convite) para [colaboração](lexicos.md#colaborar) |

## Criar [Pasta](lexicos.md#pasta)

|Objetivo |
|--|
| Criar um local para guardar [pins](lexicos.md#pin) de um mesmo tema de escolha do [usuário](lexicos.md#usuario)|
|**Contexto** |
| Local: [Página](lexicos.md#pagina) de [perfil](lexicos.md#perfil) <br> Tempo: A qualquer momento  <br> Pré-Condição:  [Usuário](lexicos.md#usuario) possuir [conta](lexicos.md#conta) no aplicativo. |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet <br> Conta no aplicativo |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Usuário](lexicos.md#usuario) ter sido bloqueado pelo outro  |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até seu [perfil](lexicos.md#perfil) <br> [Usuário](lexicos.md#usuario) seleciona a opção de criar nova [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) digita o nome que deseja dar à [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) escolhe se torna a [pasta](lexicos.md#pasta) [secreta](lexicos.md#pastaPrivada) ou não <br> [Usuário](lexicos.md#usuario) seleciona a opção criar <br> **Ou** <br> [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) seleciona um [pins](lexicos.md#pin) da página inicial <br> [Usuário](lexicos.md#usuario) seleciona a opção de [salvar](lexicos.md#salvar) [pin](lexicos.md#pin)  <br> [Usuário](lexicos.md#usuario) digita o nome que deseja dar à [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) escolhe a opção de criar [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) digita o nome que deseja dar à [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) escolhe se torna a [pasta](lexicos.md#pasta) [secreta](lexicos.md#pastaPrivada) ou não <br> [Usuário](lexicos.md#usuario) seleciona a opção criar <br> |

## Definir [interesses](lexicos.md#interesse)

|**Objetivo** |
|--|
| Escolher assuntos que são do [interesse](lexicos.md#interesse) do [usuário](lexicos.md#usuario) |
|**Contexto** |
| Local: Logo após o cadastro ou na aba de [interesses](lexicos.md#interesse) dentro da aba salvo <br>  Pré-Condição: estar logado |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de [usuário](lexicos.md#usuario) |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até a aba salvo [Usuário](lexicos.md#usuario) <br> [Usuário](lexicos.md#usuario) aperta botão [interesses](#interesse) <br> [Usuário](lexicos.md#usuario) escolhe [interesses](lexicos.md#interesse)|

## Editar um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Modificar um [pin](lexicos.md#pin) de acordo com a necessidade e desejo do dono da [conta](lexicos.md#perfil)|
|**Contexto** |
| Local: [Página](lexicos.md#página) de perfil do [usuário](lexicos.md#usuario) <br>  Pré-Condição: Conexão com a internet <br> Ter [pinado](lexicos.md#pinado), pelo menos, um [pin](lexicos.md#pin) <br> O [usuário](lexicos.md#usuario) deve estar [autenticado](lexicos.md#logado) em sua [conta](lexicos.md#conta) |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, [pin](lexicos.md#pin)|
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash)
|**Episódios** |
| [Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica em sua página de [perfil](lexicos.md#perfil) no canto superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a aba [Pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) seleciona o [pin](lexicos.md#pin) que deseja editar <br> [Usuário](lexicos.md#usuario) clica no ícone de editar simbolizado por um lápis no canto superior esquerdo da tela. <br> **ou** <br> [Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica em sua página de [perfil](lexicos.md#perfil) no canto superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a aba [Pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) passa o mouse sobre o [pin](lexicos.md#pin) que deseja editar <br> [Usuário](lexicos.md#usuario) clica no ícone de editar simbolizado por um lápis na parte superior do [pin](lexicos.md#pin). <br> **ou** <br> [Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica em sua página de [perfil](lexicos.md#perfil) no canto superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a [aba](lexicos.md#aba) Pastas <br> [Usuário](lexicos.md#usuario) clica na pasta que está o [pin](lexicos.md#pin) que deseja editar <br> [Usuário](lexicos.md#usuario) passa o mouse sobre o [pin](lexicos.md#pin) que deseja editar <br> [Usuário](lexicos.md#usuario) clica no ícone de editar simbolizado por um lápis na parte superior do [pin](lexicos.md#pin). <br> **ou** <br> [Fazer login](#fazer-login) <br> [Usuário](lexicos.md#usuario) clica em sua página de [perfil](lexicos.md#perfil) no canto superior direito da tela <br> [Usuário](lexicos.md#usuario) seleciona a [aba](lexicos.md#aba) "pastas" <br> [Usuário](lexicos.md#usuario) clica na [pasta](lexicos.md#pasta) que está o [pin](lexicos.md#pin) que deseja [editar](lexicos.md#editar) <br> [Usuário](lexicos.md#usuario) seleciona o [pin](lexicos.md#pin) que deseja [editar](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) clica no ícone de [editar](lexicos.md#editar) simbolizado por um lápis no canto superior esquerdo da tela.|

## Enviar um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Enviar um [Pin](lexicos.md#pin) para outro [usuário](lexicos.md#usuario) do [Pinterest](lexicos.md#pinterest) por meio de chat ou enviá-lo para outras pessoas que não utilizam o [Pinterest](lexicos.md#pinterest) por meio de outras redes sociais (WhatsApp, Facebook) ou até por SMS e e-mail |
|**Contexto** |
| Local: Página de detalhes de um [Pin](lexicos.md#pin) <br>  Pré-Condição: O [usuário](lexicos.md#usuario) deverá estar logado em sua conta do [Pinterest](lexicos.md#pinterest) |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário, [pin](lexicos.md#pin) |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Pin](lexicos.md#pin) ser excluído ao ser enviado <br> [Usuário](lexicos.md#usuario) que for receber o [Pin](lexicos.md#pin) ter bloqueado o que for enviá-lo |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) entra na página inicial para visualizar e navegar pelo feed de [Pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) seleciona um [Pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) clica no botão Enviar <br> [Usuário](lexicos.md#usuario) escolhe a forma de envio <br> [Usuário](lexicos.md#usuario) enviar o [Pin](lexicos.md#pin) para outra pessoa |

## Fazer [login](lexicos.md#login)

|**Objetivo**|
|--|
|Utilizar todas as ferramentas exclusivas para usuários [logados](lexicos.md#login)|
|**Contexto**|
|Local: Pagina inicial do [Pinterest](lexicos.md#Pinterest) <br> Pré-Condição: Estar [cadastrado](), inserir o e-mail e a senha corretos|
|**Atores**|
|[Usuário](lexicos.md#usuário) cadastrado|
|**Recursos**|
|E-mail válido|
|**Exceção**|
|Esquecer a senha <br> Esquecer o e-mail <br> Não ter cadastro|
|**Episódios**|
|Inicializar o [Pinterest](lexicos.md#pinterest) <br> Inserir e-mail <br> Clicar em "Continuar"|


## Ir para a fonte de um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Saber de qual site o [pin](lexicos.md#pin) está sendo enviado|
|**Contexto** |
| Local: Ao clicar em um [pin](lexicos.md#pin) ou passar o mouse sobre ele <br> Pré-Condição: Estar conectado à internet <br> Ser cadastrado no [Pinterest](lexicos.md#pinterest)|
|**Atores** |
| [Usuário](lexicos.md#usuario)|
|**Recursos** |
| Internet, aplicativo, [conta](lexicos.md#conta) de [usuário](lexicos.md#usuario) |
|**Exceção** |
| Falta de internet <br> Página fonte excluída antes do clique no [link](lexicos.md#link) da página|
|**Episódios** |feed
| [Usuário](lexicos.md#usuario) abre o aplicativo  <br> [Usuário](lexicos.md#usuario) faz o [login](lexicos.md#login)<br> [Usuário](lexicos.md#usuario) clica em um [pin](lexicos.md#pin)<br> [Usuário](lexicos.md#usuario) clica no botão com o link para o site fonte no canto inferior direito da página <br> **ou** <br>  [Usuário](lexicos.md#usuario) abre o aplicativo  <br> [Usuário](lexicos.md#usuario) faz o [login](lexicos.md#login)<br> [Usuário](lexicos.md#usuario) passa o mouse sobre um [pin](lexicos.md#pin)<br> [Usuário](lexicos.md#usuario) clica no botão com o link para o site fonte no canto inferior direito da [pin](lexicos.md#pin)<br>|

## Organizar [Pasta](lexicos.md#pasta)

|Objetivo |
|--|
| Realocar [pins](lexicos.md#pin) em [pastas](lexicos.md#pasta) ou [subpastas](lexicos.md#subpasta) e excluir [pins](lexicos.md#pin)|
|**Contexto** |
| Local: [Página](lexicos.md#pagina) da [pasta](lexicos.md#pasta) a ser organizada <br> Tempo - A qualquer momento  <br> Pré-Condição: O [Usuário](lexicos.md#usuario) deve possuir [pins](lexicos.md#pin) na [pasta](lexicos.md#pasta) a ser organizada ou na [subpasta](lexicos.md#subpasta) a ser organizada |
|**Atores** |
| [Usuário](lexicos.md#usuario) proprietário da [pasta](lexicos.md#pasta) <br> [Usuários](lexicos.md#usuario) com quem a [pasta](lexicos.md#pasta) foi [compartilhada](lexicos.md#compartilhar)|
|**Recursos** |
| Internet <br> Conta no aplicativo <br>  [Pasta](lexicos.md#pasta) <br> [Subpastas](lexicos.md#subpasta) <br> [Pins](lexicos.md#pin) na [Pasta](lexicos.md#pasta) <br> |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até a [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) seleciona a opção de organizar [pasta](lexicos.md#pasta) <br> [Usuário](lexicos.md#usuario) seleciona o [pin](lexicos.md#pin) que deseja modificar <br> [Usuário](lexicos.md#usuario) decide entre [excluir](lexicos.md#excluir), [mover](lexicos.md#mover) para [pasta](lexicos.md#pasta) ou para [subpasta](lexicos.md#subpasta)|

## Pesquisar por tema

|**Objetivo** |
|--|
| Encontrar imagens referentes a um tema de preferência do usuário |
|**Contexto** |
| Local: [Página](lexicos.md#pagina) inicial do aplicativo versão mobile <br> Tempo: a qualquer momento  <br> Pré-Condição: usuário ter em mente palavras-chaves relativas ao tema  |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet <br> Conta no aplicativo <br>|
|**Exceção** |
| Palavras que coincidirem com outros temas <br> Internet cair <br> App dar [crash](lexicos.md#crash) <br> |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) escreve palavras relacionadas ao tema desejado na [barra de pesquisa](lexicos.md#barraDepesquisa) <br> [Usuário](lexicos.md#usuario) clica "enter" <br> Aplicativo mostra uma seleção de imagens referentes ao tema <br> Aplictivo mostra uma seleção de palavras relacionadas ao tema que direcione para pesquisas específicas|

## Pesquisar por foto

|**Objetivo** |
|--|
| Utilizar o recurso de fotografar imagens para pesquisar por imagens semelhantes |
|**Contexto** |
| Local: [Página](lexicos.md#pagina) inicial do aplicativo versão mobile <br> Tempo - A Qualquer momento  <br> Pré-Condição: Celular possuir câmera  |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet <br> Conta no aplicativo <br> Celular com câmera |
|**Exceção** |
| Câmera não funcionar <br> Internet cair <br> App dar [crash](lexicos.md#crash) <br> |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) seleciona o ícone de câmera na [barra de pesquisa](lexicos.md#barraDepesquisa) <br> [Usuário](lexicos.md#usuario) tira foto da imagem por qual busca semelhantes <br> Aplicativo mostra uma seleção de imagens semelhantes à enviada pelo [Usuário](lexicos.md#usuario)  |

## Seguir outro [usuário](lexicos.md#usuario)

|**Objetivo** |
|--|
| [Seguir](lexicos.md#seguir) um outro [Usuário](lexicos.md#usuario) para acompanhar sua atividade no [Pinterest](lexicos.md#pinterest) |
|**Contexto** |
| Local: Perfil de um [usuário](lexicos.md#usuario) <br>  Pré-Condição: o [usuário](lexicos.md#usuario) não pode [seguir](lexicos.md#seguir) a si mesmo  |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Usuário](lexicos.md#usuario) ter sido bloqueado pelo outro [usuário](lexicos.md#usuario) que deseja [seguir](lexicos.md#seguir) |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) navega até a página do perfil de outro [Usuário](lexicos.md#usuario) <br> [Usuário](lexicos.md#usuario) aperta botão [seguir](lexicos.md#seguir)|

## Salvar um [Pin](lexicos.md#pin)

|**Objetivo** |
|--|
| Salvar um [Pin](lexicos.md#pin) em uma pasta criada pelo [usuário](lexicos.md#usuario) do [Pinterest](lexicos.md#pinterest) |
|**Contexto** |
| Local: Página de detalhes de um [Pin](lexicos.md#pin) <br>  Pré-Condição: o [usuário](lexicos.md#usuario) deverá estar logado em sua conta do [Pinterest](lexicos.md#pinterest) |
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo, conta de usuário, [pin](lexicos.md#pin) |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [Pin](lexicos.md#pin) ser excluído ao ser salvo <br> Não existir pastas para salvá-lo |
|**Episódios** |
| [Usuário](lexicos.md#usuario) abre o aplicativo <br> [Usuário](lexicos.md#usuario) entra na página inicial para visualizar e navegar pelo feed de [Pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) seleciona um [Pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) clica no botão Salvar <br> [Usuário](lexicos.md#usuario) escolhe a pasta para salvá-lo e se não haverem pastas criadas, cria uma pasta para poder salvar o [Pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) salvar o [Pin](lexicos.md#pin) na pasta |

## Vizualizar [Feed](lexicos.md#feed)

|**Objetivo** |
|--|
| Vizualizar [pins](lexicos.md#pin) de [interesse](lexicos.md#interesse) do [usuário](lexicos.md#usuario) pelo [feed](lexicos.md#feed) |
|**Contexto** |
| Local: [Página](lexicos.md#pagina) incial do [Pinterest](lexicos.md#pinterest) <br>  Pré-Condição: O [usuário](lexicos.md#usuario) deverá acessar o [Pinterest](lexicos.md#pinterest) caso queira vizualizar algo de seu [interesse](lexicos.md#interesse)|
|**Atores** |
| [Usuário](lexicos.md#usuario) |
|**Recursos** |
| Internet, aplicativo |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> O App não está atualizado frequentemente|
|**Episódios** |
| [Usuário](lexicos.md#usuario) acessa o [pinterest](lexicos.md#pinterest)  <br> [Usuário](lexicos.md#usuario) navega pelo [feed](lexicos.md#feed) de [pins](lexicos.md#pin) <br> [Usuário](lexicos.md#usuario) pesquisa [pins](lexicos.md#pin) de seu [interesse](lexicos.md#interesse) <br> [Usuário](lexicos.md#usuario) vizualiza o [pin](lexicos.md#pin) <br> |

## Vizualizar aba [Seguindo](lexicos.md#feed)

|**Objetivo** |
|--|
| Vizualizar [pins](lexicos.md#pin) de outros usuários que o [usuário](lexicos.md#usuario) [logado](lexicos.md#logado) segue
|**Contexto** |
| Local: [Aba](lexicos.md#aba) [seguindo](lexicos.md#seguindo) do [Pinterest](lexicos.md#pinterest) <br>  Pré-Condição: O [usuário](lexicos.md#usuario) deverá acessar o [Pinterest](lexicos.md#pinterest) caso queira publicado pelos demais usuários que segue|
|**Atores** |
| [Usuário](lexicos.md#usuario) [logado](lexicos.md#logado) <br> Usuários [seguidos](lexicos.md#seguidos) pelo [usuário](lexicos.md#usuario) [logado](lexicos.md#logado)|
|**Recursos** |
| Internet, aplicativo |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br>|
|**Episódios** |
| [Usuário](lexicos.md#usuario) acessa o [pinterest](lexicos.md#pinterest)  <br> [Usuário](lexicos.md#usuario) navega pela [aba](lexicos.md#aba) [seguindo](lexicos.md#seguindo)<br>  [Usuário](lexicos.md#usuario) vizualiza o conteúdo de cada [pin](lexicos.md#pin) <br> |

## Enviar mensagem para outros [usuários](lexicos.md#usuário)

|**Objetivo** |
|--|
| Poder se comunicar com outros [usuários](lexicos.md#usuario) por meio do [Pinterest](lexicos.md#pinterest) sendo por [mensagens](lexicos.md#mensagem) ou enviando [pins](lexicos.md#pin) |
|**Contexto** |
| Local: [Página](lexicos.md#pagina) de [mensagens](lexicos.md#mensagem) <br>  Pré-Condição: O [usuário](lexicos.md#usuario) está [logado](lexicos.md#login) em sua conta do [Pinterest](lexicos.md#pinterest)|
|**Atores** |
| [Usuário](lexicos.md#usuario) e [usuários](lexicos.md#usuario) conhecidos|
|**Recursos** |
| Internet, aplicativo |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br> [mensagem](lexicos.md#mensagem) não se entregue|
|**Episódios** |
| [Usuário](lexicos.md#usuario) [loga](lexicos.md#login) em seu [perfil](lexicos.md#perfil)  <br> [Usuário](lexicos.md#usuario) navega até o icone de [mensagem](lexicos.md#mensagem) <br> [Usuário](lexicos.md#usuario) procura por outro [usuários](lexicos.md#usuario) <br> [Usuário](lexicos.md#usuario) envia a [mensagem](lexicos.md#mensagem) <br> |

## Receber [notificações](lexicos.md#notificacão)

|**Objetivo** |
|--|
| Ser [notificado](lexicos.md#notificacao) sobre alguma interação de outros [usuários](lexicos.md#usuário) ou novos [pins](lexicos.md#pin) relacionados a um [pin](lexicos.md#pin) [pinado](lexicos.md#pinado) |
|**Contexto** |
| Local: [Página](lexicos.md#pagina) de [notificações](lexicos.md#notificacao) <br> Pré-Condição: O [Usuário](lexicos.md#usuário) deve estar [logado](lexicos.md#login) na sua conta do [Pinterest](lexicos.md#pinterest) e ter algum [pin](lexicos.md#pin) [pinado](lexicos.md#pinado) ou [seguir](lexicos.md#seguir) algum outro [usuário](lexicos.md#usuário) |
|**Autores** |
| [Usuários](lexicos.md#usuário), [usuários](lexicos.md#usuário) seguido e o [Pinterest](lexicos.md#pinterest) |
|**Recursos** |
|Internet <br> Browser <br> Aplicativo <br>  [Seguir](lexicos.md#seguir) outro [usuário](lexicos.md#usuário) <br> [Pin](lexicos.md#pin) [pinado](lexicos.md#pinado) |
|**Exceção** |
| Internet cair <br> App dar [crash](lexicos.md#crash) <br>  [Usuários](lexicos.md#usuário) [seguidos](lexicos.md#seguir) por um [usuário](lexicos.md#usuário) deixarem de segui-lo |
|**Episódios** |
|[Usuário](lexicos.md#usuário) acessa o [Pinterest](lexicos.md#pinterest) <br> [Usuário](lexicos.md#usuário) [pina](lexicos.md#pinar) um [pin](lexicos.md#pin) <br> [Usuário](lexicos.md#usuário) [segue](lexicos.md#seguir) outro [usuário](lexicos.md#usuário) <br> [Usuário](lexicos.md#usuário) clica em [notificações](lexicos.md#notificacao)  <br> [Usuário](lexicos.md#usuário) vê novas interações de outros [usuários](lexicos.md#usuário) e novos [pins](lexicos.md#pin) relacionados a um [pin](lexicos.md#pin) [pinado](lexicos.md#pinar)

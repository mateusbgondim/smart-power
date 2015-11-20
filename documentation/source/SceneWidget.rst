.. SmartPower documentation master file, created by
   sphinx-quickstart on Thu Jul 16 09:57:33 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

*class* SceneWidget(*[parent = QtGui.QGraphicsScene]*)
====================================================

Classe que cria a janela principal do programa.

Métodos
+++++++
* `create_dict_recloser(corrente, capacidade, num_rel, padrao)`_
* `mousePressEvent(mouse_event)`_
* `mouseMoveEvent(mouse_event)`_
* `mouseReleaseEvent(mouse_event)`_
* `mouseDoubleClickEvent(mouse_event)`_
* `keyPressEvent(event)`_
* `keyReleaseEvent(event)`_
* `break_edge(edge, mode, original_edge, insert)`_
* `recover_edge(item)`_
* `set_item_type`_
* `set_mode(mode)`_
* `change_state()`_
* `create_actions()`_
* `create_menus()`_
* `delete_item()`_
* `launch_dialog()`_
* `h_align()`_
* `v_align()`_
* `simulate()`_



__init__()
++++++++++++++++++++++++++++++++++++++++++++++++++
Metodo de definicao de flags, atributos auxiliares, definicao da geometria inicial da cena, cria as acoes e os menus executados na cena, e cria os dicionarios padroes do rele.
**Parametros:**
**window**-

create_dict_recloser()
++++++++++++++++++++++++++++++++
Este método cria um dicionário de um padrão de religador comercial,de acordo com os parâmetros passados.
**Parametros:**
**corrente**-string
**capacidade**-string
**num_rel**-string
**padrao**-PySide.QtCore.int

mousePressEvent()
+++++++++++++++++++++++++++++++
Este método define as ações realizadas quando um evento do tipo mousePress é detectado no diagrama grafico
**Parametros:**
**mouse_event**- PySide.QtGui.QGraphicsSceneMouseEvent

mouseReleaseEvent(mouse_event)
+++++++++++++++++++++++++++++++++++
Este método define as ações realizadas quando um evento do tipo
            mouseRelease e detectado no diagrama grafico. Neste caso conecta
            os dois elementos que estão ligados pela linha criada no evento
            mousePress.
**Parametros:**
**mouse_event**-  PySide.QtGui.QGraphicsSceneMouseEvent

MouseDoubleClickEvent(mouse_event)
++++++++++++++++++++++++++++++++++++++++++
Este método define as ações realizadas quando um evento do tipo
            mouseDoubleClick e detectado no diagrama grafico. Neste caso
            conecta os dois elementos que estão ligados pela linha criada no
            evento mousePress.
**Parametros:**
**mouse_event**-  PySide.QtGui.QGraphicsSceneMouseEvent

keyPressEvent(event)
+++++++++++++++++++++++++
Define a função de aperto de diversas teclas

**Parametros:**
**event**-PySide.QtCore.QEvent 


keyReleaseEvent(event)
++++++++++++++++++++++++++++++
**Parametros**
**event**-PySide.QtCore.QEvent

break_edge(edge, mode, original_edge, insert)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Função break_edge usada para quebrar a linha quando a inserção é a partir ou em cima de uma linha

**Parametros:**
**edge**-QtCore.QLineF
**mode**-PySide.QtCore.qint
**original_edge**-QtCore.QLineF
**insert**-

recover_edge(item)
+++++++++++++++++++++++++++++++++
Definição da função de recuperar uma linha quando está foi quebrada.

**Parametros:**
**item**- QtCore.QLineF

set_type_item(type)
+++++++++++++++++++++
Define em qual tipo de item sera inserido no diagrama grafico assim que um evento do tipo mousePress for detectado, podendo ser:
            Node.Subestacao
            Node.Religador
            Node.Barra
            Node.Agent
**Parametros:**
**type**- PySide.QtGui.QGraphicsItem

set_mode(mode)
++++++++++++++++++
 Define em qual modo
**Parametros**
**mode**-PySide.QtCore.Qt.ItemSelectionMode

change_state()
+++++++++++++++++++++++++
Define a função que muda o estado do religador. Esta função será chamada no momento que o usuário tiver selecionado um religador e pressionado a barra de espaço

create_actions()
+++++++++++++++++++++
Este metodo cria as ações que serão utilizadas nos menus dos itens gráficos.

delete_item()
++++++++++++++++++++
Este método implementa a ação de exclusão de um item gráfico do diagrama.

launch_dialog()
+++++++++++++++++++
Este método inicia os diálogos de configuração de cada um dos itens gráficos do diagrama.

increase_bus()
+++++++++++++++++++++
Este método implementa a ação de aumentar o tamanho do item gráfico barra.

decrease_bus()
++++++++++++++++++++
Este método implementa a ação de diminuir o tamanho do item gráfico barra.

simulate()
++++++++++++++++++
Inicia a simulação: cálculos de fluxo de carga e curto circuito










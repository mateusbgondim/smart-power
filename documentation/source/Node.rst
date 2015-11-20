.. SmartPower documentation master file, created by
   sphinx-quickstart on Thu Jul 16 09:57:33 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

*class* Node(*[parent = QtGui.QGraphicsRectItem]*)
====================================================
**Parâmetro: parent** - QtGui.QGraphicsLineItem

Classe que implementa o objeto DashedLine, utilizado para indicar que um elemento do diagrama foi selecionado. Sua representaçao e uma borda
tracejada laranja.

Métodos
+++++++
* `fix_item()`_
* `update_count()`_
* `remove_edges()`_
* `remove_edge(edge)`_
* `add_edge(edge)`_
* `edge_position(edge)`_
* `center()`_
* set_center(pos)`_
* `boundingRect()`_
* `paint(painter,option,widget)`_
* `itemChange(change,value)`_
* `MousePressEvet(mouse_event)`_
* `MouseMoveEvent(mouse_event)`_
* `MouseReleaseEvent(mouse_event)`_
* `MouseDoubleClickEvent(event)`_
* `adjust_in_grid(pos)`_
* `contextMenuEvent(event)`_
* `keyReleaseEvent(event)`_
* `recover_edge(item)`_
* `set_item_type(type)`_
* `increase_bus()`_
* `align_line_h()`_
* `align_line_v()`_
* `
__init__()
++++++++++
Configurações do texto

**Parametros:** 
**item_type** -QtCore.QRectF
**parent** - PySide.QtGui.QWidget
**scene** -object
**node_menu** -


fix_item(self)
+++++++++++++++++++++++++++++++++++++++++++++++++
Seta a flag de fixação do item.

update_count(self)
+++++++++++++++++
 Atualiza o contador que acompanha o número de Edges do item.

remove_edges(self)
+++++++++++++++++++++++++++++++++++

Método de remoção de todos objetos Edge associados ao objeto node.

remove_edge(self, edge)
++++++++++++++++++++++++++++++++
Esta função remove a edge passada na chamada do item presente.

**Parâmetros:**
**edge** -Edge.edge
 
add_edge(self,edge)
++++++++++++++++++++++++++++++++++
Método de adição de objetos edge associados ao objeto node

**Parâmetros:**
**edge** -QtCore.QPointF
 
edge_position(self, edge)
+++++++++++++++++++++++++++++++++++++++++++
 Este método é utilizado da distribuição das Edges ligadas numa
            barra, seguindo uma lógica de alinhamento.

**Parâmetros:**
**edge** -QtCore.QPointF

center(self)
++++++++++++++++++++++++++++++++++++
Método que retorna o centro do objeto passado

set_center(self, pos)
++++++++++++++++++++++++++++++++++++
Seta o centro
**Parâmetros:**
**edge** -QtCore.QPointF

boundingRect(self)
++++++++++++++++++++++++++++++++++
Reimplementação da função virtual que especifica a borda do objeto node

paint(self, painter, option, widget)
++++++++++++++++++++++++++++++++++++++++++++++

Método de desenho do objeto node implementado pela classe Node.Aqui se diferencia os objetos pela sua forma. Todos eram definidos por um retângulo QtCore.QRectF. Neste método, serão desenhadas suas formas baseadas em seus retângulos.

**Parâmetros:**
**painter**-PySide.QtGui.QPen
**option**-
**widget**-PySide.QtGui.QGraphicsWidget

itemChange(self,change,value)
++++++++++++++++++++++++++++++++
Método que detecta mudancas na posição do objeto Node
**Parâmetros:**
**change**-QtGui.QGraphicsItem.ItemPositionChange
**value**-QtGui.QGraphicsItem

mousePressEvent(self, mouse_event)
+++++++++++++++++++++++++++++++++++++++++++++++++++
Reimplementação da função virtual que define o evento referente
            ao aperto de botão do mouse
**Parâmetros:**
**mouse_event**-PySide.QtGui.QMouseEvent
mouseMoveEvent(self, mouse_event):
+++++++++++++++++++++++++++++++++++++++++++
Reimplementação da função virtual que define o evento referente
            ao movimento do mouse durante o aperto
**Parâmetros:**
**mouse_event**-PySide.QtGui.QMouseEvent

mouseReleaseEvent(self, mouse_event):
+++++++++++++++++++++++++++++++++++++++++++++++++++++++
Reimplementação da função virtual que define o evento referente
            ao soltar do botão mouse após aperto.
**Parâmetros:**
**mouse_event**-PySide.QtGui.QMouseEvent

mouseDoubleClickEvent(self, event)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Reimplementação da função de duplo clique do mouse.
**Parâmetros:**
**event**-PySide.QtGui.QMouseEvent

adjust_in_grid(self, pos)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Este método implementa uma grade invisível na cena, que limita o
            movimento dos Nodes para posições bem definidas.
**Parâmetros:**
**pos**-

contextMenuEvent(self, event)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Classe que implementa o container Gráfico onde os
        widgets residirão, denominado cena
**Parâmetros:**
**event**-





         



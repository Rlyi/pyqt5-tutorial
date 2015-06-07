StackedWidget
=============
The StackedWidget is a container which displays a single page at a time. A left-hand panel provides access to the pages which are then displayed to the right.

===========
Constructor
===========
Construction of the StackedWidget is done using::

  stackedwidget = QStackedWidget()

=======
Methods
=======
To add an item to the StackedWidget use::

  stackedwidget.addWidget(widget)
  stackedwidget.insertWidget(index, widget)

The *index* value should be set to the numerical position identifying where the widget should be inserted.

Removal of the widget from the StackedWidget is done using::

  stackedwidget.removeWidget(widget)

The index value or the widget currently visible widget within the StackedWidget is obtained via either::

  stackedwidget.currentIndex()
  stackedwidget.currentWidget()

Setting the currently visible widget is also done with::

  stackedwidget.setCurrentIndex(index)

To retrieve the number of widgets held by the StackedWidget call::

  stackedwidget.count()
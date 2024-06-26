layers.py
==============

The layers are auto-generated by filling the ``layers.csv`` file, ``FLYLINE_MARK`` / ``ERROR_MARK`` layer are defined by **Latitudeda** for error display.

::

    class LAYER(BASE_LAYER):
        NITRIDE = Layer(PROCESS.NITRIDE, PURPOSE.DRAW, 'Drawn objects on this layer will be protected from the silicon nitride etch.')
        NITRIDE_ETCH = Layer(PROCESS.NITRIDE_ETCH, PURPOSE.DRAW, 'Drawn objects on this layer will be exposed to the silicon nitride full etch to the BOX.')
        HEATER = Layer(PROCESS.HEATER, PURPOSE.DRAW, 'This layer defines the heater filaments.')
        PAD = Layer(PROCESS.PAD, PURPOSE.DRAW, 'This layer defines the heater contact pads.')
        FLOORPLAN = Layer(PROCESS.FLOORPLAN, PURPOSE.DRAW, 'This layer defines the design space boundaries')
        LABEL = Layer(PROCESS.LABEL_SETTINGS, PURPOSE.DRAW, 'This layer defines text labels')
        FLYLINE_MARK = Layer(PROCESS.FLYLINE, PURPOSE.MARK, 'Flyline for insufficient space in AutoLink')
        ERROR_MARK = Layer(PROCESS.ERROR, PURPOSE.MARK, 'Error mark')



For users using layout viewers (e.g. KLayout), they can import the layer properties file ``layers.lyp`` in the file folder.
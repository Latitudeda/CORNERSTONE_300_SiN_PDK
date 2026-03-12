factory.py
===============


Define the straight and bend waveguide factories for auto-routing function in **PhotoCAD**.

#. ``StraightFactory`` : Import the straight waveguide to use it for straight connection.

#. ``EulerBendFactory`` : Import ``BendEuler``, ``BendEuler90``, ``BendEuler90_STRIP_C_WIRE`` and ``BendEuler90_STRIP_O_WIRE`` from ``bend_euler`` and assigned each component to different situations.

    * Note that the default bend radius of every 90-degree bend used for auto-routing was set based on the different types of waveguides. However, users should define the bend radius themselves to meet the design requirements. A warning text is added in the component ``BendEuler``, ``BendEuler90``, ``BendEuler90_STRIP_C_WIRE`` and ``BendEuler90_STRIP_O_WIRE`` users can remove it after setting the right bend radius.

    .. image:: ../images/bend90warning.png

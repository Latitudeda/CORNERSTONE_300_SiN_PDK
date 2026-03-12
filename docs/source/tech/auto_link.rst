auto_link.py
=============

Define the auto link policies between different waveguide type.

For example:

``(type(WG.SIN_STRIP.C.WIRE) >> type(WG.SIN_STRIP.C.WIRE), StraightPrefer(WG.SIN_STRIP.C.WIRE), BendUsing(WG.SIN_STRIP.C.WIRE.BEND_EULER))``

It means that when the start and end waveguide are both ``WG.SIN_STRIP.C.WIRE``, the automated waveguide type for routing will be ``WG.SIN_STRIP.C.WIRE`` and an automated bend ``WG.SIN_STRIP.C.WIRE.BEND_EULER`` will be added at a 90 degree turn.


Users are allowed to define and set ``DEFAULT`` to their own specific linking policy.


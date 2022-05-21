# CameraMgr
Fork of https://gitlab.com/V3X3D/love-libs/-/tree/master/CameraMgr to fix my own issue with this lib.
Right now, you can pass w and h arguments to CameraMgr.update(dt, w, h) to allow this library work sirh scaling libraries, such as my https://github.com/Vovkiv/resolution_solution.
Problem is that, by default, library was using whole window size to center camera, meaning, that window size is dictating where to center camera and limits, while my scaling library, have width and height that it will render to, meaning you can see only that part of screen.
So to prevent that, library should accept different width and height for it's math.

Tup is a build system that keeps track of when files change and what the
dependencies actually are by monitoring file acces. This makes it ideal for
systems where dependencies cannot be introspected easily, such as binary files
for CAD etc.

These are some tup rules for working with solvespace, a small CAD program. It
will export all solvespace files to `.stl` files for 3d printing, and it
will also convert them into `.blend` files for rendering in blender.

Currenly it assumes all solvespace files are in teh same directoy, which is
fine for small projects. When I need recursive subdirectories I'll make
a new set of tupfiles/tupdefaults

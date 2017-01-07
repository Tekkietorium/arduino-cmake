=========================
Arduino CMake + QtCreator
=========================

This is a fork of https://github.com/queezythegreat/arduino-cmake.

Besides some bug fixes, this fork adds QtCreator support, namely a project wizard
to facilitate creation of Arduino projects in QtCreator.

QtCreator Usage
---------------
git-clone the repository:
code-block::
  cd /usr/local/share
  git clone https://github.com/rhaschke/arduino-cmake

Create a symlink to the wizards folder:
code-block::
  mkdir -p ~/.config/QtProject/qtcreator/templates/wizards
  ln -s /usr/local/share/arduino-cmake/qtcreator/wizards ~/.config/QtProject/qtcreator/templates/wizards/arduino

In QtCreator choose "New Project" -> "Import Project" -> "Arduino sketch".

License
-------
This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this file,
You can obtain one at http://mozilla.org/MPL/2.0/.

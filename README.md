tuned
=====

Currently two non-compatible versions of Tuned exists - Tuned (RHEL-7+) and
Tuned legacy (RHEL-6).

This role can install, configure (only non-legacy Tuned), and start Tuned
daemon. It can also activate arbitrary Tuned profile or activate Tuned profile
which is recommended for the machine / product (the latter is supported only on
non-legacy Tuned). It can also deploy custom Tuned / Tuned legacy profiles.

Role Variables
--------------

For list of supported role variables together with the description and preset
default values see:

./defaults/main.yml

Role Facts
----------

This role sets the following facts:

### tuned_legacy
True if there is Tuned legacy, false otherwise.

### tuned_recommended_profile
Name of the Tuned profile which is recommended as a default for the
machine / product. This is not supported on Tuned legacy, it's
set there to the empty string.

### tuned_available_profiles
List of Tuned profiles which are available on the machine.

License
-------

Copyright (C) 2017 Jaroslav Škarvada <jskarvad@redhat.com>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.

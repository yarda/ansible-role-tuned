tuned
=====

This role installs and starts Tuned daemon and sets predefined Tuned profile.
Currently two non-compatible versions of Tuned exists - Tuned (RHEL-7+) and
Tuned legacy (RHEL-6). This role can also deploy custom Tuned / Tuned legacy
profiles. In case of Tuned it can also deploy custom configuration and auto set
the Tuned profile which is recommended for the machine / product (this is not
supported on Tuned legacy).

Role Variables
--------------

For list of supported role variables together with description and preset
default values see:
./defaults/main.yml

Role Facts
----------

The role sets the following facts:

### tuned_legacy
True if there is Tuned legacy.

### tuned_recommended_profile
Name of Tuned profile which is recommended as a default for the
machine / product. This is not supported on Tuned legacy, it's
set to empty string there.

### tuned_available_profiles
List of Tuned profile names which are available on the machine.

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

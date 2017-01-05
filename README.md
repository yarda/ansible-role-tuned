tuned
=====

This role installs and starts Tuned daemon and sets predefined Tuned profile.

Role Variables
--------------

```
# Name of the Tuned profile, it can be throughput-performance,
# latency-performance, powersave, balanced. If empty string is used it uses
#default profile (with tuned-0.X, i.e. RHEL-6) or auto-detected profile which is
#the most suitable for the system/product (with tuned-2.X, i.e. RHEL-7+)
tuned_profile: throughput-performance
```

License
-------

Copyright (C) 2017 Jaroslav Škarvada <jskarvad@redhat.com>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the.
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.

tuned
=====

This role installs and starts Tuned daemon and sets predefined Tuned profile.

Role Variables
--------------

```
# Name of the Tuned profile, can be throughput-performance,
latency-performance, powersave, balanced. If empty string is used it uses
default profile (with tuned-0.X, i.e. RHEL-6) or auto-detected profile which is
the most suitable for the system/product (with tuned-2.X, i.e. RHEL-7+)

tuned_profile: throughput-performance
```

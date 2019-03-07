## Conventions for terminology on π-Base

We adhere to the following conventions:

- Where there is no contradiction, we use conventions established in the following texts:
  - [General Topology](https://mathscinet.ams.org/mathscinet-getitem?mr=2048350) by Stephen Willard
  - [Topology](https://mathscinet.ams.org/mathscinet-getitem?mr=3728284) by James Munkres
- For the separation axioms, `T_n \Rightarrow T_m` whenever `n\geq m`.
  - For example, on π-Base "regular" is defined to assert that points and closed sets can be separated, while 
    `T_3` is defined to be both regular and `T_0`. However, some authors swap these.
- If a property is "locally P", then that means that every point in the space has a neighborhood base
  satisfying P for every member of the base.
  - On the other hand, some authors define "locally" to mean there is a single neighborhood satisfying P
    for each point. This is fine for e.g. local metrizability, but is not equivalent in general, e.g.
    local compactness. See <https://github.com/pi-base/data/issues/42> for discussion. Use
    "locally P by single neighborhoods" instead in this case.

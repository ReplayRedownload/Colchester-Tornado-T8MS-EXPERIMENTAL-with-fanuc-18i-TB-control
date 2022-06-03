# Colchester-Tornado-T8MS-EXPERIMENTAL-with-fanuc-18i-TB-control

Colchester Tornado T8MS EXPERIMENTAL with fanuc 18i-TB control (Customized... Expect to have some bugs...)

# Changes:

Changes to the G-Code result:

G99 => G95 (Works... (for now...))

G98 => G94 (Works... (for now...))

G17 => G18 (Works... (for now...))

G83.5 => G83 (Works... (for now...))

Polar stuff... is forced and not working 100%... (You will have to manually add G13.1 when to stop...)

Changed H0. (Primary spindle incremental adress) => C0 (When primary spindle is active, but there won't be any H0.)

Changed H0. (Primary spindle incremental adress) => B0 (When secondary spindle is active, but there won't be any H0.)

# Stuff to do:

Remove M31 ( & M32, optional) when secondary spindle is active.

Get rid of C0 (Polar stuff... (Hard))

In G-Code end result export, make changes in description for better differentiating.

Insert before CO/B0 M109/M112 (Optional before tool).




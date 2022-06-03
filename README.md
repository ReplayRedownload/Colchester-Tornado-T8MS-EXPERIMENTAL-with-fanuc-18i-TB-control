# Colchester-Tornado-T8MS-EXPERIMENTAL-with-fanuc-18i-TB-control

Colchester Tornado T8MS EXPERIMENTAL with fanuc 18i-TB control (Customized... Expect to have some bugs...)

# SOURCE:

https://cam.autodesk.com/posts/post.php?name=samsung%20mill-turn%20fanuc

# Changes:

Changes to the G-Code result:

G99 => G95 (Works... (for now...))

G98 => G94 (Works... (for now...))

G17 => G18 (Works... (for now...))

G83.5 => G83 (Works... (for now...))

Polar stuff... is forced and not working 100%... (You will have to manually add G13.1 when to stop...)

Changed H0. (Primary spindle incremental adress) => C0 (When primary spindle is active, but there won't be any H0.)

Changed H0. (Primary spindle incremental adress) => B0 (When secondary spindle is active, but there won't be any H0.)

Changed G-Code export description for better differentiating (Only addeed a word...)

# Stuff to do:

Remove M31 ( & M32, optional) when secondary spindle is active.

Get rid of C0 (Polar stuff... (Hard))

Insert before CO/B0 M109/M112 (Optional before tool).




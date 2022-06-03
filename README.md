# Colchester-Tornado-T8MS-EXPERIMENTAL-with-fanuc-18i-TB-control

Colchester Tornado T8MS EXPERIMENTAL with fanuc 18i-TB control (Customized... Expect to have some bugs...)

# SOURCE:

https://cam.autodesk.com/posts/post.php?name=samsung%20mill-turn%20fanuc

# Changes:

G99 => G95 (Works... (for now...**(Used multiple times)**))

G98 => G94 (Works... (for now...**(Used multiple times)**))

G17 => G18 (Works... (for now...**(Used multiple times)**))

G83.5 => G83 (Works... (for now...**(Used once olny)**))

Polar stuff... is forced and not working 100%... (You will have to manually add G13.1 stuff like that)

Changed H0. (Primary spindle incremental adress) => C0. (When primary spindle is active, but there won't be any H0.) OR B0. (When secondary spindle is active, but there won't be any H0.)(Works... (For now.. **(Used multiple times)**))

Changed G-Code export description for better differentiating (Only addeed a word...)

Removed M31 & M32 when secondary spindle is active (Works... (For now...**(Used olny once)**))

# Stuff to do:

Get rid of the lone C0. (Polar stuff... (Hard))

Insert before C0/B0 M-Code M109/M112 (Optional, also before tool(Not really sure if I remember it correctly))




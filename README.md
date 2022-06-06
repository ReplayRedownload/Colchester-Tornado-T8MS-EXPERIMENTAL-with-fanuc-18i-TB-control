# Colchester-Tornado-T8MS-EXPERIMENTAL-with-fanuc-18i-TB-control

Colchester Tornado T8MS EXPERIMENTAL with fanuc 18i-TB control (Customized... Expect to have some bugs...)

# SOURCE:
<p>https://cam.autodesk.com/posts/post.php?name=samsung%20mill-turn%20fanuc</p>

# Changes:
<p>G99 => G95 (Works...)</p>
<p>G98 => G94 (Works...)</p>
<p>G17 => G18 (Works...)</p>
<p>G83.5 => G83 (Works...)</p>
<p>Polar stuff... is forced and not working 100%... (You will have to manually add G13.1 and stuff like that)</p>
<p>Changed H0. (Primary spindle incremental adress) => C0. (When primary spindle is active, but there won't be any H0.) OR B0. (When secondary spindle is active, but there won't be any H0.)(Works...)</p>
<p>Changed G-Code export description for better differentiating (Only addeed a word...)</p>
<p>Removed M31 & M32 when secondary spindle is active (Works...)<p>
<p>Make a certain character *cough* C0. *cough* to be the same when primary spindle active or become B0. when secondary spindle is active. (Works...)</p>
<p>Insert A0 after G55 and G00 when secondary spindle is active (Works...).<p>
<p>In subspindle grab removed(commented) unwated code (Torque skip on/off & G31 P98)<p>
<p>Moved M05, M105 below M116 (Cancel synchronization)<p>

# Stuff to do:
  
# I'm not sure if I need to do this...
<p>Insert before C0/B0 M-Code M109/M112 (Optional, also before tool(Not really sure if I remember it correctly))</p>

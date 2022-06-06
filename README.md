# Colchester-Tornado-T8MS-EXPERIMENTAL-with-fanuc-18i-TB-control

Colchester Tornado T8MS EXPERIMENTAL with fanuc 18i-TB control (Customized... Expect to have some bugs...)

# SOURCE:
<p>https://cam.autodesk.com/posts/post.php?name=samsung%20mill-turn%20fanuc</p>

# Changes:
<p>G99 => G95 (Works... (for now...(Used multiple times)))</p>
<p>G98 => G94 (Works... (for now...(Used multiple times)))</p>
<p>G17 => G18 (Works... (for now...(Used multiple times)))</p>
<p>G83.5 => G83 (Works... (for now...(Used once olny)))</p>
<p>Polar stuff... is forced and not working 100%... (You will have to manually add G13.1 stuff like that)</p>
<p>Changed H0. (Primary spindle incremental adress) => C0. (When primary spindle is active, but there won't be any H0.) OR B0. (When secondary spindle is active, but there won't be any H0.)(Works... (For now.. (Used multiple times)))</p>
<p>Changed G-Code export description for better differentiating (Only addeed a word...)</p>
</p>Removed M31 & M32 when secondary spindle is active (Works... (For now...(Used olny once)))</p>
</p>Make a certain character *cough* C0. *cough* to be the same when primary spindle active or become B0. when secondary spindle is active. (Works, but I doen't think it works 100% with the intent in mind (For now.. (Used multiple times)))</p>
</p>Insert A0 after G55 and G00 when secondary spindle is active.<p>

# Stuff to do:

# I'm not sure if I need to do this...
<p>Insert before C0/B0 M-Code M109/M112 (Optional, also before tool(Not really sure if I remember it correctly))</p>

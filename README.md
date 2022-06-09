# Colchester-Tornado-T8MS-EXPERIMENTAL-with-fanuc-18i-TB-control

<p>Colchester Tornado T8MS EXPERIMENTAL with fanuc 18i-TB control (Customized... Expect to have some bugs and to be a spaghetti mess...)<p>
<p>In the EXPERIMENTAL file has also comments<p>
<p>Example: //Changed something bla bla bla -AHF<p>
<p>You will easily find the differences in the code if you use Visual Studio Code or something else to compare with the one on the internet.<p>
    
# SOURCE:
<p>https://cam.autodesk.com/posts/post.php?name=samsung%20mill-turn%20fanuc</p>

# Changes:
<p>G99 => G95</p>
<p>G98 => G94</p>
<p>G17 => G18</p>
<p>G19 => G18<p>
<p>G83.5 => G83</p>
    <p>M00 => M03<p>
    <p>Added G94 in eject part<p>
<p>G54 => G55 in Eject Part<p>
<P>G17 => G18 in Eject Part<p>
<p>Changed H0. (Primary spindle incremental adress) => C0. (When primary spindle is active, but there won't be any H0.) OR B0. (When secondary spindle is active, but there won't be any H0.)</p>
<p>Changed G-Code export description for better differentiating (Only addeed a word...)</p>
<p>Removed M31 & M32 when secondary spindle is active<p>
<p>Make a certain character *cough* C0. *cough* to be the same when primary spindle active or become B0. when secondary spindle is active. (Works...)</p>
<p>Insert A0 after G55 and G00 when secondary spindle is active<p>
<p>In subspindle grab removed(commented) unwated code (Torque skip on/off & G31 P98)<p>
<p>Moved M05, M105 below M116 (Cancel synchronization)<p>
<p>Added Sub spindle retun AND Return to ABS PR in Part Eject end.<p>
<p>Added G00 A0 in a if statemeent in Eject Part<p>
<p>Add B0(SUB) or C0(MAIN) after (C=#)to help the machine find its axis<p>
<p>If secondary spindle is active in G71 line W change to W *-1<p>
<p>Corrected coordinates output (I hope it works in other scenarios too...)<p>
<p>Polar stuff... is forced and not working 100%... (You will have to manually add G13.1 and stuff like that)</p>
    
# Stuff to do:    
<p>Look into one operation which has error and possibly try to fix it<p>
    
# I'm not sure if I need to do this...
<p>Insert before C0/B0 M-Code M109/M112 (Optional, also before tool(Not really sure if I remember it correctly))</p>
<p>Check if thread is working as intented, something about G76<p>

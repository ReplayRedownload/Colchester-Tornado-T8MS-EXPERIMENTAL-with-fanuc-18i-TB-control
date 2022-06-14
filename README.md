# Colchester-Tornado-T8MS-EXPERIMENTAL-with-fanuc-18i-TB-control

<p>Colchester Tornado T8MS EXPERIMENTAL with fanuc 18i-TB control (Customized... Expect to have some bugs and to be a spaghetti mess...)<p>
<p>In the EXPERIMENTAL file has also comments<p>
<p>Example: //Changed something bla bla bla -AHF<p>
<p>You will easily find the differences in the code if you use Visual Studio Code or something else to compare with the one on the internet.<p>
    
# SOURCE:
<p>https://cam.autodesk.com/posts/post.php?name=samsung%20mill-turn%20fanuc</p>

# Changes:

<h3>Changing export values:</h3>
<ul>
  <li>G99 => G95;</li>
  <li>G98 => G94;</li>
  <li>G17 => G18;</li>
  <li>G83.5 => G83;</li>
  <li>G83.6 => G83;</li>
  <li>M00 => M03;</li>
  <li>G54 => G55 in Eject Part;</li>
  <li>Export description</li>
  <li>Moved M05 & M105 below M116 (Cancel synchronization)</li>
</ul>

<h3>Commented:</h3>
<ul>
    <li>In subspindle grab removed(commented) unwated code (Torque skip on/off & G31 P98)</li>
    <li>Commented most if not all lines which include "H"</li>
</ul>

<h3>Added:</h3>
<ul>
    <li>Added G94 in eject part</li>
    <li>Added G00 A0 in a if statemeent in Eject Part</li>
    </li>Added Sub spindle retun AND Return to ABS PR in Part Eject end.</li>
    </li>Add B0(SUB) or C0(MAIN) after(C=#)to help the machine find its axis</li>
</ul>

<h3>Change values when necessary conditions are met:</h3>
<ul>
    <li> H0. => B0./C0. when Secondary spindle or Main spindle selected</li>
    <li>Export description, ZMIN=-# when Main spindle is selected or else ZMAX=+#</li>
    <li>Removed in export M31 & M32 when secondary spindle is selected</li>
    <li>When left-tapping is selected it will output M28 and when right-tapping is selected it will output M27 and for the rest it is still M29</li>
    <li>When Flood is selected M03/M04 => M13/M14</li>
    <li>When secondary spindle is selected C0. => B0.</li>
    <li>Insert A0 after G55 and G00 when secondary spindle is active</li>
    <li>If secondary spindle is active in line the with G71, change W to W*-1</li>
</ul>

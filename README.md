I wrote this in 2010 before I knew Python, don't judge.

<h1>Starcraft 2 Auto-Queen</h1>

<h2>Purpose</h2>
<p>This script will, in Starcraft 2, automatically inject larva in all your hatcheries every 30s incredibly quickly (you may get an APM spike over 1000).</p>

<h2>Install</h2>
<p>The script uses <a href="pyhook.sourceforge.net">pyhook</a>, a library for low-level keyboard and mouse hooks in Windows. Pyhook has it's own <a href="http://sourceforge.net/apps/mediawiki/pyhook/index.php?title=Main_Page#System_Requirements">system requirements</a> - I think it also requires Python 2.7 or earlier.</p>

<h2>Usage</h2>
<p>Immediately after initiating the auto-injecting and every 30s thereafter, your computer will beep. One second later, the script will press:</p>
<ul>
<li>'ctrl+9' (to save your currently selected units)</li>
<li>'6' (to select the queens)</li> 
<li>for every hatchery you've indicated, it will press 'v' and click on that hatchery on the minimap</li>
<li>'9' (to reselect the units you had selected)</li>
</ul>
<p>Before entering a command, press the '\' key. There are four commands:</p>
<ul>
<li>'o' <strong>indicate hatchery</strong> - after pressing \o, click on your minimap where the hatchery is located. The location is now stored for future use in the script.</li>
<li>'q' <strong>initiate auto-injecting</strong> the script will begin auto-injecting every 30s. Before this command is issued, you must have indicated at least one hatchery location.</li> 
<li>'r' <strong>reset script</strong> this will delete all hatchery locations in memory and stop auto-injecting every 30s. You may re-assign the hatchery locations and start the auto-injections again.</li>
<li>'p' <strong>quit</strong></li>
</ul>
<p><strong>Notes:</strong>I recommend that you refrain from moving your mouse or pressing buttons during the 0.1s when the auto-injecting is happening. If you use the grid layout (not default), edit the script to change the 'v' to 'x' where it's marked. Assign your queens to hotkey 6. The script will use hotkey 9 to reselect the units you had selected when the script started. While the script is running, you may use four commands:</p>

<h1 align="center">TD VJ Controller Blueprint</h1>

###

<div align="center">
  <img height="" src="https://freight.cargo.site/w/1851/h/861/i/S1638342408656037859169199731133/VJ-Controller.png"  />
</div>

###

<h1 align="left">Overview</h1>

###

<p align="left">This optimized VJ Controller allows both non-MIDI and MIDI users to control and play their audiovisuals. It is accessible to users who cannot afford a MIDI controller and has the ability to "uncook" certain components, thereby reducing the resources TouchDesigner uses. Additionally, it offers the capability to use levels to combine different visuals for improved blending. It also includes a custom audiovisual analysis featuring two types of analysis: one from TouchDesigner itself and another employing a Bileam-style cutoff audio analysis. Lastly, the most commonly used feedback system is conveniently placed at the end and can be easily disabled through a slider or your MIDI key input. <br><br>Tested on:<br>Touchdesigner 2023.10130 (confirmed)<br>Touchdesigner 2022.33910 (unconfimed)<br>It should work on 2022 builds but the annotations will not show up. Not sure what they changed about the annotations that destroyed the backwards compatibility on it but the rest should work. <br><br>Equipment I'm using: <br>MIDI Controller: LaunchControlXL by novation<br><br>HINT:To better optimize this, please look into using the engine comp in parallel with the 'uncook' script.</p>

###

<h1 align="left">How to add more containers to create a larger set</h1>

###

<div align="center">
  <img height="" src="https://i.postimg.cc/Vv5KRK5z/Screenshot-2024-04-24-101643.png"  />
</div>

###

<p align="left">In order for the chopexec to work, which "uncooks" or "cooks" depending on value change (you can think it of as pulse), the chop null5 must have the correct corresponding name. If my first audiovisual component is named 'flower' for example, you must use the rename chop to rename it to 'flower'.  Also remember to do the same if you decided to switch to using the MIDI Controller and vice versa. To add more containers just add another button and it will automatically rename it to container6 up to 10. You can change this in your rename, the same applies to using the MIDI controller, use the 'select chop' to rename it corresponding to container</p>

###

<h1 align="left">Audio Analysis</h1>

###

<p align="left">This custom audio analysis container allows all settings to be adjusted through the container's settings, eliminating the need to manually change each setting inside. Since different types of music require varying amounts of gain, this feature can be adjusted right out of the box. While I recommend using addition sparingly, it can be incredibly useful for making drastic changes. The container also includes two texture operators that transform the audio spectrum into textures, which can be used in special cases to create interesting effects. The audio analysis employs both TouchDesigner in-house analysis and Bileam-style cutoff analysis. This project is still incomplete , as I am collaborating with sound engineers to fine-tune the control over high, mid, and low cutoffs. It's also important to note that this audio analysis does not perform well with unmastered songs, as unmastered songs typically blend the audio spectrum.</p>

###

<div align="center">
  <img height="" src="https://freight.cargo.site/w/1183/h/706/i/J1638355527648381688075537101245/Audio-analysis.png"  />
</div>

###

<h1 align="left">Container Settings</h1>

###

<div align="center">
  <img height="" src="https://freight.cargo.site/w/1240/h/750/i/I1638390725069091994027755319741/Audio-Anaylsis.png"  />
</div>

###

<p align="left">Custom Parameters that can be set out of the box. The purpose of this is to the set the gain, smoothing and addition before doing a show. As each different type of music has varying audio spectrum. You can also map this to your MIDI controller as long as you have enough buttons/knobs to do so.</p>

###

<p align="left">CREDITS: bileam tschepe (elekktronaut for the audio analysis for teaching me how to do cutoffs. Notoball for teaching me how to create the audio spectrum top. Torin Blankensmith for making this blueprint possible. All of them can be found on youtube and I highly  recommend watching their tutorials.</p>

###

<p align="left">Update as of 4/23/2024 - I will not be updating this for the foreseeable future as this is meant to be a blueprint as I already have a much more improved version of this but do feel free to contact me on discord on ways to improve this.<br><br>If there is more interest, I have a Serial Communication Parser for OSC communication to game engines such as Unity and Unreal. It also works for any program that accepts OSC messages.</p>

###

<div align="center">
  <a href="https://discord.com/users/po_tat" target="_blank">
    <img src="https://raw.githubusercontent.com/maurodesouza/profile-readme-generator/master/src/assets/icons/social/discord/default.svg" width="52" height="40" alt="discord logo"  />
  </a>
</div>

###

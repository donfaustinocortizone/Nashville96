# Nashville96
<p align="center">
	<img src="images/nashville96_logo.png" alt="Screenshot 1"/>
</p>

A collection of Windows-like GTK themes based on both Chicago95 (for GTK3) and Redmond97 (for GTK2) incoporating some infamous color schemes. 

**Note:** This was made with XFCE on mind, so you may find issues if you are using another DE.

### Installation
1. Download and unzip the latest release and copy the folder of your theme of choice to `~/.themes/` if you want a local installation, or just copy to `/usr/share/themes` if you want a global installation.
2. Select the theme with both Appearance and Window Manager. 

### Tips and tricks
Unlike Chicago95, the desktop icon colored labels come disabled by default. To revert that: 
1. Go to where your theme is located which is `~/.themes/` if installed locally, if installed globally then go to `/usr/share/themes`.
2. Open the folder of the theme you want to change, and then  navigate to `gtk-3.0/apps`.
3. Open `xfce.css` with your editor of choice.
4. Under `XfdesktopIconView.view`, replace the `background: transparent;` line with `background: @xfd_icon_backdrop;`. It should look like this:
	```
	/* Xfdesktop */
	XfdesktopIconView.view {
	  background: @xfd_icon_backdrop;
	  color: @selected_bg_color;
	  border-radius: 0px; }
	```		
5. Save the changes and restart the theme by just choosing another one and then selecting Nashville again.

If you are looking for  Windows-like icons i recommend to use either the [default Chicago95 icons](https://github.com/grassmunk/Chicago95/tree/master/Icons) or [SE98](https://github.com/nestoris/Win98SE).
		
### Screenshots
<p align="center">
	<img src="images/screenshot_1.png" alt="Screenshot 1"/>
	<img src="images/screenshot_2.png" alt="Screenshot 2"/>
	<figcaption>
		<b>Extra information: </b>
		<ul>
			<li><b>Icons:</b> <a href="https://github.com/nestoris/Win98SE">SE98</a>.</li>
			<li><b>Cursor:</b> <a href="https://github.com/grassmunk/Chicago95/tree/master/Cursors/Chicago95_Cursor_Black">Chicago95 Black</a>.</li>
			<li><b>Font:</b> <a href="https://en.wikipedia.org/wiki/Tahoma_(typeface)">Tahoma</a>.</li>
			<li><b>Terminal Font:</b> <a href="https://laemeur.sdf.org/fonts/">Less Perfect DOS VGA</a>, you can also get some good vintage fonts <a href="https://int10h.org/oldschool-pc-fonts/">from here</a>.</li>
			<li><b>Wallpaper:</b> Tile generated with <a href="https://bg.siteorigin.com/">Background Generator</a>.</li>
			<li><b>Compositor:</b> <a href="https://github.com/yshui/picom">picom</a>.</li>
		</ul>
	</figcaption>
</p>

### Thanks to 
- [@grassmunk](https://github.com/grassmunk) for [Chicago95](https://github.com/grassmunk/Chicago95).
- [@matthewmx86](https://github.com/matthewmx86) for [Redmond97](https://github.com/matthewmx86/Redmond97).
- [@morhetz](https://github.com/morhetz) for the [Gruvbox color scheme](https://github.com/morhetz/gruvbox).
- [@rebelot](https://github.com/rebelot) for the [Kanagawa color scheme](https://github.com/rebelot/kanagawa.nvim).
- [@tpenguinltg](https://github.com/tpenguinltg) for [Windows Classic theme designer](https://github.com/tpenguinltg/winclassic).

### License 
GNU General Public License v3.0

# Nashville Gruvbox

A Windows-like GTK theme based on both Chicago95 (for GTK3) and Redmond97 (for GTK2) incoporating the infamous Gruvbox color scheme. 

**Note:** This was made with XFCE on mind, so you may find issues if you are using another DE.

### Installation
1. Unzip the latest release and copy the `Nashville Gruvbox` directory to `~/.themes/` if you want a local installation, or just copy to `/usr/share/themes` if you want a global installation.
2. Select the theme with both Appearance and Window Manager. 

### Tips and tricks
Unlike Chicago95, the desktop icon colored labels come disabled by default. To revert that: 
1. Go to where your theme is located which is `~/.themes/` if installed locally, if installed globally then go to `/usr/share/themes`.
2. Open the `Nashville Gruvbox` folder, and then  navigate to `gtk-3.0/apps`.
3. Open `xfce.css` with your editor of choise.
4. Under `XfdesktopIconView.view`, replace the `background: transparent;` line with `background: @xfd_icon_backdrop;`. It should look like this:
	```
	/* Xfdesktop */
	XfdesktopIconView.view {
	  background: @xfd_icon_backdrop;
	  color: @selected_bg_color;
	  border-radius: 0px; }
	  
	```		
5. Save the changes and restart the theme by just choosing another one and then selecting Nashville again.
		
### Screenshots

<p align="center">
	<img src="images/screenshot_1.png" alt="Screenshot 1"/>
	<figcaption>
		<b>Extra information: </b>
		<ul>
			<li><b>Icons:</b> <a href="https://www.gnome-look.org/p/1012512/">Buuf</a>.</li>
			<li><b>Cursor:</b> <a href="https://github.com/mdomlop/retrosmart-x11-cursors">Retrosmart</a>.</li>
			<li><b>Font:</b> <a href="https://terminus-font.sourceforge.net/">Terminus</a>.</li>
			<li><b>Compositor:</b> <a href="https://github.com/yshui/picom">picom</a>.</li>
		</ul>
	</figcaption>
</p>

### Thanks to 

- [@grassmunk](https://github.com/grassmunk) for [Chicago95](https://github.com/grassmunk/Chicago95).
- [@matthewmx86](https://github.com/matthewmx86) for [Redmond97](https://github.com/matthewmx86/Redmond97).
- [@morhetz](https://github.com/morhetz) for the [Gruvbox color scheme](https://github.com/morhetz/gruvbox).
- [@tpenguinltg](https://github.com/tpenguinltg) for [Windows Classic theme designer](https://github.com/tpenguinltg/winclassic).

### License 
GNU General Public License v3.0

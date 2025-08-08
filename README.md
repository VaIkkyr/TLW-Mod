# Adrian's TLW Modification

## Changelog

### Gameplay & Mechanics

- **Bomb Kill Feed:** Now displays the killer's velocity, showing exactly how fast you were deleted.
- **Bomb Round Time Syncronized:** Now syncronizes the masterclient's round time with all clients and fades out the option for non masters.
- **Delayed Auto Spectate Slider:** Spectate can now be adjusted to not snap to a player immediately as the client dies, up to 2 seconds.
**Fixed HUD Freezing:** Hud no longer freezes or skips after a couple of seconds.
**Hud Reworked:** Changed the hud positioning and the kill info positioning, also added Show Time as a toggleable option in the Game Settings.
- **Hook Update Timing Fixed:** Removed a 1-frame delay where hooks updated before players. Input lag and inconsistencies are gone. (Thanks to Thyme for guiding me there.)
- **Bomb Kills Desync-Free:** Death and death effects now appear where the player actually died. Velocity and ping are properly handled.
- **Scroll Wheel Reeling Framerate-Independent:** Each scroll notch acts like a key press, making timing consistent. You can time them right before you hook and they will register just as they would using a key. In the Game Settings panel, use the "Once" option, not "Multiple"; it works best.
- **Extra Reel In and Reel Out:** Have returned to the Extra Keys panel.
- **Respawn Cooldown Added:** To prevent packet spam issues.
- **/roll Command:** Now balances teams randomly. Extra players are automatically sent to individual.
- **Network Interpolation Improved:** FOV, velocity, camera rotation, and position are now synchronized. (This is unrelated to camera interpolation.)
- **Dead Players No Longer Send Data:** They are now proper spectators.
- **Redundant Input Code Removed:** Input handling is faster and more accurate.
- **Turbo and Normal Assets Swappable:** Can now be swapped during a round. No restart required.
- **Turbo Assets Implicitly Turned Off:** Faded out from the menu when racing or playing custom maps to prevent texture bugs.
- **Bomb Round Time Slider Added:** You can now adjust how much it takes until the round restarts after everyone perishes.
- **Hook Colors and Levi Special Networked:** You can see Levi’s animation including the rope spinning if another player does it. The hooks can be toggled on/off from the Hooks section under Colors; click on Hooks, and the “Spectator Colors” toggle will show.

### Camera & UI

- **Camera Tilt Smoother:** With improved camera handling. A toggle for ground tilt has been added for those who want it.
- **Fullscreen and Camera Updates:** Now properly respect your refresh rate.
- **HUD Positioning:** Now adjusts based on refresh rate, reducing visual artifacts when switching between fullscreen and windowed.
- **Camera System Reworked:** Fake frame masking has been removed. Input is now clean and responsive.
- **Spectator HUD Added:** Shows who you're watching and lets you toggle between tracking and free cam using a rebindable key.
- **Player Name Tags Hidden (Spectating):** The HUD now handles identity display.
- **Spectator Cursor UI Added:** You can now see player bomb cooldowns, velocity, and aim direction.
- **Player Names in Teams Visible While Spectating:** They are only hidden when you play and only if you explicitly turn the setting ON, and it would only affect your team. Guild Name and Name Length “#” are no longer visible either; there was a bug where they showed even when names were hidden.
- **Camera Options Expanded:**
  - Toggle for ground tilt.
  - Camera height slider added; it can be tweaked independently of camera distance. It has a toggle so if you prefer to use only camera distance, it can be completely turned off. It is set up so it wouldn’t interfere with your standing still/walking animations or stock; it will only work when you actually fly. This is also networked so you can see it on the spectator view.
  - Added Original Camera Speed when people switch to original camera instead of Mouse Sensitivity.
  - Original Camera Speed sensitivity works independently from TPS and newTPS and saves separately.

### Performance & Stability

- **Spectator Mode Fully Removed:** Do not try to use it.
- **Spectator System Rebuilt:** It now auto-tracks when you die or join a room. No more manual switching. You can still cycle players with 1 and 2.
- **Option Added:** To disable thunderspear animations and gas burst effects.
- **Fullscreen Mode:** Is now true exclusive fullscreen, not simulated borderless.
- **Minimal Launcher Added:** Allows custom resolution and display mode selection.
- **FPS Counter:** Now reflects your actual frame rate. No more inflated numbers.
- **Hook and Cursor Jitter Fixed:** Hook and cursor is now visibly smooth and stable.
- **Many Other Optimizations:** Were made but are not listed here to keep the changelog readable.

---

## Credits

Thanks to **Syal** for providing the source code, suggestions, and some fixes.  
Also, thank you to everyone who helped test.

**Original Mod Creator:** Syal  
**Testing Credits:** Ph3x, Fen, Kaze, Tornado, Yui, Myao, Rai, Terami
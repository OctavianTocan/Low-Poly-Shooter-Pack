# Low Poly Shooter Pack v6.0

![Cover](/assets/images/cover.jpg)

A comprehensive Unreal Engine FPS template featuring custom blueprints, detailed documentation, and meticulously fine-tuned configurations for optimal gameplay experience.

## About This Project

This project is a polished Unreal Engine FPS template that enables developers to create stylized first-person shooter games without starting from scratch. The pack provides a complete foundation with smooth shooter mechanics, modular low poly weapons, AI enemies, and full multiplayer support.

This project represents a deep dive into Unreal Engine development, where every aspect has been carefully crafted and optimized. Rather than using default settings, this project showcases the level of polish achievable through systematic refinement and attention to detail.

## My Contributions

### 🏗️ **Custom Blueprints**

* I created every Blueprint in the entire project myself. That includes:

  * First and third-person player controllers
  * The weapon inventory system
  * Two complex Animation Blueprints, which honestly took a long time to get right because of all the depth I added—like the custom spring system for weapon sway, plus those small transition animations and additive turning blends
  * Full multiplayer replication, which I added *after* building the asset (wasn’t originally structured for networking, so it was a real challenge to retrofit everything for multiplayer, but I managed to do it anyway)
  * The AI systems (these were pretty basic, but they work and add enemy encounters)
  * All the UI systems—everything from the weapon pickup UI, the player HUD, ammo pickups, to the weapon loadout/spawn menu. I actually designed and laid out the entire UI myself.

**What I’m most proud of:**

* **Custom spring system for weapon sway:**
  This took the longest to nail down. It’s not just the spring system itself; it’s how it works together with the animation system—like how we blend in additive turning animations on the first-person weapons while you’re looking around, and how the system changes the weapon’s position and rotation based on where you’re aiming, for posture simulation (and same for crouching). The animation system adapts to and reacts to what you’re doing, and I got a lot of that into third-person as well.
* **Making everything replicated for multiplayer after the fact:**
  The asset wasn’t built with networking in mind, so I had to go through every feature and figure out how to network it. It wasn’t perfect, but I managed to get it all working pretty well for online play. If I started over, I’d do a bunch of things differently, but I’m still proud of how it turned out.
* **Weapon attachment systems:**
  I went through several different approaches—ChildActorComponents, Spawning Actors, Mesh Components, and more—before settling on a system that worked for the pack. The solution I landed on was Child Actor-based and robust. (For my later assets, like the Realistic Assault Rifle Template, I’ve done this even better.)

### 📚 **Comprehensive Documentation**

* Wrote a full documentation suite that explains **every variable, function, and Blueprint** in the entire asset.
* Created detailed setup guides and how-tos for users, including:

  * **General Info & FAQ**: Covered everything from “what do you use for animating” to “how do I modify the weapon sway/lag” and more.
  * **Step-by-step Guides** for:

    * Manually upgrading from v5.0 to v6.0
    * Adding new weapons (full process)
    * Adjusting weapon ironsight aiming offsets
    * Adding new weapon presets or skins
    * Adding weapon pickups
    * Migrating the asset to another project
    * Making the third-person character always face forward while moving
  * **Category-based Documentation**:

    * Broke down the systems into categories (Animation, Health, Inventory, Saves, Characters, Damageables, Interactions, Notifies, etc.) and documented how every part works, how it all connects, and how to extend or modify anything.

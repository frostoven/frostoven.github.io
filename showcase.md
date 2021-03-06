## Showcase and screenshots

### Disclaimer
When I first recorded the below, a lot of them were only intended for friends
and family. I've since realised these make for a pretty good showcase, although
some were unfortunately recorded by pointing a phone at a computer screen.

Due to the project still being in early stages of development, much of these
visuals require writing special code to make visible. Writing code just to
reproduce a showcase takes time, yet these features will eventually reveal
themselves naturally as the code evolves. For that reason I feel the poor
quality showcase is acceptable for now. This will be revised in future to have
a more professional feel.

All below images generated using the
[Cosmosis game engine](https://github.com/frostoven/Cosmosis/) (unless
otherwise stated).

## Early stages

### Demo
Very first gif recorded to show literally anything. In this image, the Sun,
Moon, and Earth are to scale and have real-world distance. Their rotations are
wrong, though.

![demo.gif](showcase/demo.gif)

### Getting stars right

Getting stars right was tough. I had to crash course an astronomy course to get
some basic stuff going.

I started by rendering 10,000 random dots. This number was chosen because we
can, at most, see 9,110 stars at night with the naked eye assuming ideal
conditions (incidentally, my machine could handle 1 million dots before things
would start crawling).

Random dots to simulate a basic starfield:

![first_starfield.jpg](showcase/first_starfield.jpg)

Accompanying video:

* [starfield.mp4](showcase/first_starfield.mp4)

### True star positions

I could not find a catalogue that contained all Earth-visible stars
(with 3D positions), so I
[made one myself](https://github.com/frostoven/BSC5P-JSON-XYZ). It took waaayyy
too long to make (50 days). Luckily it does the job.

Here is an early experiment rendering it:

![starfield_sphere.gif](showcase/starfield_sphere.gif)

### Generating true star colour

Star colour needs to mimic Planck's law if you want stars to look good (I
learned this the hard way after first trying generic fade-ey dots). This is the
final result I ended up with, generated via shader:

![star_colour.png](showcase/star_colour.png)

Combining the shader with actual star positions we created earlier,
things start looking interesting:

![orion_and_beyond.gif](showcase/orion_and_beyond.gif)

Indeed, do a Google search for Orion's Belt and decide for yourself if this
looks like a real photo:
<!--
  Hint: it doesn't :p. There was a bug that caused colours in that
  screenshot to come out wrong (this was caused by an array offset issue;
  it has since been fixed as seen in the gif above).
  TODO: Take a new screenshot where the bug has been fixed.
-->

![orion.png](showcase/orion.png)

## Graphics

### Random screenshots taken during development

Godrays:

![god_rays.png](showcase/god_rays.png)

Lighting test:

![ds69f.png](showcase/ds69f.png)

In the following screenshot, the ship's shadow is all messed due to
accidentally calculating backfaces, making it look like a type of carbon
fibre:

![broken_shadow.jpg](showcase/broken_shadow.jpg)

## Modelling

All screenshots and videos in this section taken from Blender. Blender is
currently used exclusively for all modelling.

### Ships currently being worked on

First spaceship ever made for the game, the DS69F:
<!--
  This is in the reference to the Deep Space 69 cartoon, where they find an
  abandoned two-seater spaceship. This ship was inspired by that ship.
-->

![first_spaceship.png](showcase/first_spaceship.png)

Its cockpit frame is currently being revised:

![frame.jpg](showcase/frame.jpg)

Second ship ever made for the game. It's still under construction:

![second_spaceship.png](showcase/second_spaceship.png)

Accompanying video:

* [CELL57.mp4](showcase/CELL57.mp4)

Another ship currently being worked on is the Scorpion-D:

![scorpion_d.png](showcase/scorpion_d.png)

Video showcasing internals:

* [maintenance access.mp4](showcase/scropion_d_maintenance.mp4)

### Random screenshots taken during development

![prototype.png](showcase/prototype.png)

![proto_inside.png](showcase/proto_inside.png)

![experiment.jpg](showcase/experiment.jpg)

### Texture experiments

These will probably never make it into the game, but they served as good
entertainment, so I decided to add them here.

Jungle Gym style:

![junglegym.jpg](showcase/junglegym.jpg)

Space Tractor:

![space_tractor.jpg](showcase/space_tractor.jpg)

Cloth Ship:

![cloth_ship.jpg](showcase/cloth_ship.jpg)

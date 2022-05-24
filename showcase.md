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
[Cosmosis game engine](https://github.com/frostoven/Cosmosis/).

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

![starfield.mp4](showcase/first_starfield.mp4)

### True star positions

I could not find a catalogue of that contains all Earth-visible stars, so I
[made one myself](https://github.com/frostoven/BSC5P-JSON-XYZ). It took waaayyy
too long to make (50 days) but it does the job.

Here is an early experiment rendering it:

![starfield_sphere.gif](showcase/starfield_sphere.gif)

### Generating true star colour

Star colour needs to mimic Planck's law if you want stars to look good (I
learned this the hard way after trying generic fade-ey dots). This is the
final result I ended up with, generated via shader:

![star_colour.gif](showcase/star_colour.png)


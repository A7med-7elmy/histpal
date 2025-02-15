# Historical Palettes (histpal)

Histpal is a Python library that empowers you to explore and utilize color palettes from various historical civilizations. 

The history of human civilization is intricately woven with color. From the vibrant hues adorning cave paintings to the majestic pigments used in monumental architecture, color has served as a powerful tool for storytelling, symbol-making, and artistic expression. As we embark on a captivating exploration of historical palettes, our initial destination is the cradle of civilization itself:
 Ancient Egypt.


 ## Ancient Egypt: Coloring the Temple of Dendur

Imagine the Temple of Dendur, a majestic sandstone structure from ancient Egypt, not bathed in the stark white of a museum setting, but aglow with the vibrant colors it once possessed. This is precisely the captivating experience offered by The Metropolitan Museum of Art's groundbreaking project: "Coloring the Temple of Dendur."
 
 ![image](Images/Dendur.png)

The Met's innovative project employed cutting-edge technology and meticulous research to digitally reconstruct the temple's lost color scheme.
 By meticulously studying surviving fragments of pigment and analyzing depictions of temples in ancient Egyptian art, experts were able to piece together a comprehensive picture of the temple's original vibrancy.
 
This project unlocks the secrets of ancient Egyptian colors using modern technology which you could directly import it using histpal library.

If you interested in more detailes about this project, here is a [Met Museum Article](https://www.metmuseum.org/articles/color-the-temple), [Met Museum Journal 53](https://cdn.sanity.io/files/cctd4ker/production/077e163a879f0c80c9183e2a5635318c0f3eccef.pdf) and [The Source Code of The Project](https://github.com/metmuseum-medialab/colorthetemple/tree/master). 


You also can find an academic presentation about colors used in egyptian arts and it's meaning by Prof. Howie Baum from University of Cincinnati [here](https://www.uc.edu/content/dam/refresh/cont-ed-62/olli/21-fall/egypt%208.pdf).

 
## Egyptian Blue

[Egyptian Blue](https://en.wikipedia.org/wiki/Egyptian_blue) (#1034a6 ), dating back to 3250 BCE, is the oldest known synthetic pigment. For centuries, the exact recipe for Egyptian blue remained a captivating mystery. It wasn't until the 20th century,
 with the aid of advanced scientific techniques, that researchers were able to unravel the secrets of its production. This breakthrough not only shed light on the Egyptians' remarkable scientific understanding but also offered a deeper appreciation for the complex chemistry behind this enduring pigment.
 
 The popularity of Egyptian blue wasn't confined to the Nile Valley. Evidence suggests it was traded throughout the Roman Empire; Its influence can be seen in Roman art and architecture, a testament to the lasting impact of this ancient innovation. Egyptian blue is far more than just a color; it's a portal to the ingenuity, artistry, and scientific prowess of a civilization that continues to captivate us.


## Inspiring Palettes

Websites like [Coolors.co](https://coolors.co/) offer a powerful tool for generating color palettes. By using Coolors.co, we can create unique color palettes inspired by the most remarkable Egyptian monuments. These palettes can then be seamlessly imported using the histpal library, adding a touch of grandeur and historical context to your data visualizations.

![image](Images/egypal-medium.png)


You can find these generated palettes on [coolors.co website](https://coolors.co/u/ahmed_helmy2).


## Documentation

egypal function has two parameters name & number.

```
egypal(name, n)
```

name has only 5 possible values.

"dendur" .........for palette of coloring the temple of dendura. (Default)

"tut"..................for Tut Ankh Amun regenerated palette.

"anibus"..........for the god of death anibus palette.

"beetle"...........for the palette of sacrab beetle statuette.

"ankh".............for the regenerated palette of a wooden case for a mirror, formed in the shape of an ankh.


n .....is number of colors returned from the selected palette (Default = 6).

### Examples

After installing histpal, here is an example of its default egyptian palette.

```
import seaborn as sns
from histpal.egypal import *

palette = egypal()

sns.palplot(palette)
```

Another example showing how to import the first 4 colors from the palette of scarab beetle. 

```
import seaborn as sns
from histpal.egypal import *

palette = egypal(name = "beetle", n = 4)

sns.palplot(palette)
```




Get started with histpal and bring the rich history of color to your projects!

### Credits

-You can find the sources of the images used to generate the palettes here : [Tut Ankh Amoun](https://www.flickr.com/photos/mharrsch/33822793526/in/photostream/), [Anibus](https://www.metmuseum.org/art/collection/search/590939), [Beetle, Ankh](https://www.nbcnews.com/slideshow/amp/king-tut-36719464).

-The fascinating project of coloring the temple has been achieved by the efforts of Matt Felsen, Erin Peters, and Maria Paula Saba.

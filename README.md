![Simple paper-spinner](../gh-pages/simple-paper-spinner.gif)

# Simple `<paper-spinner>`

Intrigued by Keanu Lee's amazing [article](//blog.keanulee.com/2014/10/20/the-tale-of-three-spinners.html) describing how he built the official [`<paper-spinner>` Polymer element](//polymer.github.io/paper-spinner/components/paper-spinner/demo.html) seen in the [Google Material Design spec](//www.google.com/design/spec/components/progress-activity.html), I had to see if it was possible to simplify the spinner further by condensing it down to a single HTML element. My goal was to rebuild the paper-spinner in a way that was:

*   Accessible ✓
*   Cross browser compatible (IE10+) ✓*
*   A single HTML element ✓
*   HTML and CSS only ✓
*   Uses relative units for easy scalability ✓
*   Animated with strictly composite properties (`transform` and `opacity`) ✓**

Well…I got really close. Check it out. (Pull requests are more than welcome.)

* * *

*I use `clip-path: circle()`, which is not available in IE or Firefox, as a progressive enhancement only to remove small artifacts left over from the animations.

**All spinners animate with composite properties except the multicolor spinner. The multicolor spinner unfortunately invokes repaints on color changes. :/ On the plus side, I haven't seen the frame rate dip below 60fps.



## License

The MIT License (MIT)

Copyright (c) 2015-2020 [Chris Nager](https://twitter.com/chrisnager)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

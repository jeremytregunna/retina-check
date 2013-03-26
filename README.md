# Retina Check
Copyright © 2013 Jeremy Tregunna, All Rights Reserved.

Retina Check is a simple borne shell script compatible with all borne compatible shells (sh/ash/ksh/bash/zsh/...). It checks that your images are good for use on iOS/Mac projects that will run on retina devices.

For instance, let's assume you have an app which displays an image `foo.png`. This image has a width of 100 and a height of 200. This script will check for a `foo@2x.png` which has a width of exactly 200, and a height of exactly 400. If those conditions don't hold, a message will be printed such like this:

    foo@2x.png: Height is 399, expected 400 (diff: -1)
    foo@2x.png: Width is 202, expected 200 (diff: 2)

Nothing will be displayed if the images are the expected size. Upon successful run, retina-check will return a zero exit status. If an error is encountered, retina-check will return a non-zero exit status.

## Installation

Just throw it somewhere in your `$PATH` and make sure it's executable.

## License

Copyright © 2013, Jeremy Tregunna, All Rights Reserved.

Permission is hereby granted, free of charge, to any person obtaining a copy of this
software and associated documentation files (the "Software"), to deal in the
Software without restriction, including without limitation the rights to use, copy,
modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
and to permit persons to whom the Software is furnished to do so, subject to the
following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


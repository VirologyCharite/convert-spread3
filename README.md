## Convert SpreaD3 files

The `index.html` file produced by
[SpreaD3](https://rega.kuleuven.be/cev/ecv/software/SpreaD3) fails to load
properly due to a
[CORS](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing) issue.

There's a Github issue that I (Terry) commented on
[here](https://github.com/phylogeography/SpreaD3/issues/32#issuecomment-540656648).

This repo holds the horrible shell script I wrote to convert the SpreaD3
output to something that works.

## Usage

Here's (more or less) the message I wrote about it on the GitHub ticket:


The script will produce two new files, `index-new.html` and
`main-new.js`. Open the former with your browser.

NOTE: this is extremely brittle. If the spread3 developers change what they
write into `main.js` (which they certainly will do!), this code will cease to
produce output that works. I've just written it so a colleague can work
with spread3 and post it here in case it helps you. It also illustrates how
the overall problem could be fixed, along the lines that I posted above.

If you don't see a map loaded in your browser, open the console and have a
look for JavaScript errors. Then post them here & maybe I'll be able to
help.

The person I wrote this for tells me he is using version `0.9.7.1` of
SpreaD3. The above script is, I expect, highly unlikely to work on any
other version.

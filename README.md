Dirfuzz
=============

This is a tool for directory discovery of web applications, by default it uses a dictionary
based approach which is in data/fdirs.txt it can also use the crawler module to find links
up to 1 level of depth.

Usage
-------

Basic usage:

./dirfuzz host [options]


To see the available options use:

./dirfuzz -h


If you are getting alot of redirects try with the -i option which will ignore these.

./dirfuzz host -i

To enable extraction of links using the crawler module use -l 0 or -l 1, the difference being the depth
of the crawling, just frontpage links or frontpage links and use these to dig a bit depeer.


While the included wordlist is not optimized for finding files you can still use it for this task with the -e option.

./dirfuzz host -e .sql


Requirements
-----------

Ruby 1.9.2+

Gems:
term-ansicolor
nokogiri
work_queue
json

If you run on windows you will need to turn the colors off or use ansicon (http://adoxa.3eeweb.com/ansicon/index.html)

License
-------

Dirfuzz is distributed under the GNU General Public License, see COPYING for details.





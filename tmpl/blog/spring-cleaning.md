We've been plugging away on Mirage for the last few months, and things are starting to take shape nicely. As the older blog entries were out-of-date, we have shifted the descriptive material to a new [wiki](/wiki) section instead. What else has been happening?

* The Xen microkernel backend is fully event-driven (no interrupts) and very stable under stress testing now. The TCP stack is also complete enough to self-host this website, and you can try it out by navigating to [xen.openmirage.org](http://xen.openmirage.org). The stack doesnt actually do retransmissions yet, so your user experience may "vary".
* [Richard Mortier](http://www.cs.nott.ac.uk/~rmm/) has put together a performance testing framework that lets us analyse the performance of Mirage applications on different backends (e.g. UNIX vs Xen), and against other conventional applications (e.g. BIND for DNS serving). Read more in the wiki [here](/wiki/performance).
* Thomas Gazagnaire has also integrated experimental Node.JS support to fill in our buzzword quota for the year (and more seriously, to explore alternative VM backends for Mirage applications). 
* Thomas has also rewritten the website to use the COW syntax extensions. He's also started a new job with [OCamlPro] doing consultancy on OCaml, so congratulations are in order!
* The build system (often a bugbear of such OS projects) now fully uses [ocamlbuild]() for all OCaml and C dependencies.

There are some exciting developments coming up later this year too!

* Raphael Proust will be joining the Mirage team in Cambridge over the summer in an internship.
* Anil Madhavapeddy will be giving several [tech talks](/wiki/talks) on Mirage: at the [OCaml User's Group] in Paris at the end of the week, at Citrix Cambridge in May, and at Acunu in London in June. If you are interested, please do drop by and say hi.
* Verisign has supported the project with an Internet Infrastructure Grant to celebrate 25 Years of Dot Com.
* [David Scott](http://dave.recoil.org) (chief architect of the Xen Cloud Platform) and [Anil Madhavapeddy](http://anil.recoil.org) will give a joint tutorial on constructing functional operating systems at the [Commercial Users of Functional Programming](http://cufp.org) workshop in Tokyo, Japan in September.
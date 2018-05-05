# About Me

I'm gholt. I forget stuff. A lot. This page is to help me remember what I have
on GitHub. :-)

I mostly write code in Go these days, but I have some older Python code here
still. Anything older than that (Java, C++, C, etc.) was before I had a GitHub
account.

[ring](https://github.com/gholt/ring) - I've put a lot of work into this
solution for consistent hashing distribution. It has been in flux for quite a
while, but hopefully it is settling down now.

[swiftly](https://github.com/gholt/swiftly) - A Python client for Swift /
Hummingbird. I would love to replace this with a Go equivalent, but just
haven't had the time yet. Turns out this tool is used quite a bit "out there"
and occasionally requires some maintenance.

[brimtext](https://github.com/gholt/brimtext) - Text tools for Go. This has
Align, for pretty-printing tables of text, and Wrap, and other text tidbits.

[blackfridaytext](https://github.com/gholt/blackfridaytext) - This is a text
renderer edition of Russ Ross's [Blackfriday Markdown Processor](https://github.com/russross/blackfriday).
This is pretty useful to quickly see if some Markdown you have is "okay" on the
command line, and is useful in generating detailed help text for cli tools.

[store](https://github.com/gholt/store) - Super fast key value store, or more
specifically, a keyhash value store. Too much to detail here, but it's the
product of another R&D project that hasn't yet found a home. This is the code I
wrote to abuse 40-core machines with dual PCI-e SSDs and 256Gs of RAM.

[locmap](https://github.com/gholt/locmap) - This goes hand-in-hand with the
store above. It's an in-memory location map that tracks keyhashes to locations
where the values are, whether still in memory or now on disk. This was a lot of
fun to write as I quickly found single-core choke points I had to work around.

[kvt](https://github.com/gholt/kvt) - Very simple key|value|timestamp store.
This is mainly for small sets of metadata that will be changed on multiple
machines and synced up later.

[gastly](https://github.com/gholt/gastly) - Simplistic Go source file rewriter.
I use this now instead of my previous project `got` whenever I need "generics"
with Go.

[got](https://github.com/gholt/got) - Go Templating for `go generate`. Quick
and simple tool I've used when I need "generics".

[findfind](https://github.com/gholt/findfind) - A parallel find utility. This
is useful when working with highly distributed file systems, like CFS.

[cpcp](https://github.com/gholt/cpcp) - A parallel cp utility, much like
findfind, for use with distributed file systems.

[dudu](https://github.com/gholt/dudu) - Yes, horrible name, but I already had
findfind and cpcp, so... It's a parallel du utility.

[holdme](https://github.com/gholt/holdme) - Go package of generic structures
for holding values. Ordered slices, a weird ValueOrderedKeys construct, and
hopefully more over time.

[brimtime](https://github.com/gholt/brimtime) - This library does its best to
translate human-typed dates and times into machine time.Times, and back. It has
fun things in it like NearDateString that tries to reduce the verbosity of a
date and time the closer it is to now (or another reference time), and
TranslateRelativeDate that lets you use phrases like "3 weeks from now".

[brimio](https://github.com/gholt/brimio) - Has a checksummed reader,writer and
a random data reader.

[brimpath](https://github.com/gholt/brimpath) - This one's a bit weird in that
it's so small, just one function that I needed and couldn't figure out where
else to put it.

[bdow](https://github.com/gholt/bdow) - Quick tool to run on my Windows gaming
machine when I leave Black Desert Online running overnight. The game has a bad
habit of cranking the GPU full throttle when it loses connection to the server.
This tool just monitors the process for a network connection and kills it if it
doesn't have one anymore.

[tcod](https://github.com/gholt/tcod) - Just my personal junk drawer. My
`.vimrc` is here amongst other things.

[brimcrypt](https://github.com/gholt/brimcrypt) - This library is getting a bit
of moss growing on it. I had been experimenting with AES io.Reader,Writers with
temporary cached keys. I may play around with this again someday; it was fun.

[chantimeout](https://github.com/gholt/chantimeout) - Experiment to find out
why Go's time.After was horribly slow and what alternatives there were.

[context](https://github.com/gholt/context) - Goes along with the above
chantimeout and is a quick implementation of Go's Context, but avoiding
time.After.

[python-brim](https://github.com/gholt/python-brim) - Now this one just brings
back memories. I had fanciful notions of a framework for creating Python
services that would be easy to deploy and maintain. R&D. Also, L&G (Learn and
Grow).


## Projects I work (or have worked) on, but don't solely maintain:

[swift](https://github.com/openstack/swift) - A distributed, highly scalable
object storage system much like S3. It was one of the two original products
that started OpenStack.

[hummingbird](https://github.com/troubling/hummingbird) - A rewrite of
OpenStack Swift in Go, with some cruft left out, and probably some added we
didn't mean to. We're aiming for more speed and simpler deployments. Go is much
better with concurrency and a rewrite lets you apply a lot of lessons you've
learned the first time around.

[cfs](https://github.com/getcfs/megacfs) - An R&D project where we were making
a distributed file system, think Swift or Hummingbird but mountable like a
local hard drive, or think NAS. Unfortunately, company direction changed and we
got canceled, but we had it to a working prototype stage, learned a lot, and
had a lot of fun.

[swauth](https://github.com/gholt/swauth) - I wrote this auth system back when
OpenStack didn't have one yet. It now has Keystone, but there are quite a few
users of Swauth out there still. So much so that active development of it was
taken over by some OpenStack devs again at
<https://github.com/openstack/swauth> of which I'm very thankful.

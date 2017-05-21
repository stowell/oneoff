# `oneoff`

Most everything I've ever completed has started out gross. Once I'm
desperate and worn down enough to not care about propriety and just get
something tiny working in the worst way possible then I actually do stuff. The rest
of the time I spend worrying about how things will look  and what
other people will think. I have nothing but regret for the time I've wasted
worrying in this life.

If `oneoff` takes away that worrying for me and maybe another human, I'll be happy.
You type into a `textarea` for goodness sake.

I was about to launch into wha the language is like but maybe I should just start
typing it:

```
idtosmallid is
  files
  first
  shouldbe
    id is string32
    smallid is uint4

previds is
  idtosmallid
  just id

latestids is
  files
  second
  shouldbe
    id is string32

start is
  idtosmallid
  just smallid
  max

newidtosmallid is
  latestids
  minus previds
  enumerate
  map
    smallid is offset plus start

idtosmallid
union newidtosmallid
```

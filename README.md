# JS Graph

Me playing around with graphs and Cayley

## Required

`brew install cayley`

## Running

### REPL

```
cayley repl --config=cayley.cfg
```

### HTTP Interface

```
cayley http --config=cayley.cfg --assets /usr/local/Cellar/cayley/0.5.0/share/cayley/assets
```

## Sample Queries

"Things that are Design Patterns"

```
g.V("Design Pattern").Tag("target").In("is a").Tag("source").All();
```

"Things that OOP is"
```
g.V("OOP").Tag("source").Out("is a").Tag("target").All();
```

"Things that are related to things"

```
g.V("Module Pattern").Tag("source").Both("is related to").Tag("target").All();
g.V("Object Literal").Tag("source").Both("is related to").Tag("target").All();
g.V("Encapsulation").Tag("source").Both("is related to").Tag("target").All();
g.V("Revealing Module Pattern").Tag("source").Both("is related to").Tag("target").All();
g.V("OOP").Tag("source").Both("is related to").Tag("target").All();
```

[ ihavenoideawhati'mdoing.jpg ]

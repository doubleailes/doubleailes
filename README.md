# Hi there 👋

I'm Philippe Llerena, tech guy in CG. I'm working in VFX and Animation industry since 2005ish. I have a female jackhuahua named [Fury](https://www.instagram.com/furythedestroyer) because, she is furious.

## Languages

I'm fluent in English, French, python. I know a little bit of Japanase and Español. I started developpement in basic with my dad's casio and latter my T.I 89. I learn java at college but i forgot everything. During covid i started Rust because of a joke with [Paul](https://github.com/pypoulp) and hit the [GIL](https://en.wikipedia.org/wiki/Global_interpreter_lock). I'm now learning Rust and i'm very happy with it. Here some of my rust project: [quiet-stroll](https://github.com/forticheprod/quiet-stroll), [fls](https://github.com/forticheprod/fls), [girolle](https://github.com/doubleailes/girolle)

## Projects

### Girolle

My latest personnal project is [girolle](https://github.com/doubleailes/girolle), i used [nameko](https://github.com/nameko/nameko) to create microservices in python. I wanted to learn rust ( of course ) so i wrote Girolle inspired by Nameko. One of the big challenges not already solved is macro-procedural part. The AST got still mysterious and low documentation. I'm working on it. I feel more and more closer to rewrite the whole thing for a more ideomatic rust and division of responsibility.

### framels

[fls](https://github.com/forticheprod/fls) project is intent to deliver a `ls` command inspired by `bls` from [Buf Compagnie](https://buf.com/) or more recently `rvls` from **RV**.

![cliexample](https://github.com/forticheprod/fls/blob/main/images/fls_demo.gif)

Here is an exemple of the usage of my fls library:

```bash
cargo add framels
```

In your main.rs

```rust
use framels::{
    basic_listing, parse_dir,
    paths::{Paths, PathsPacked},
};
let source = "./samples/big".to_string();
let paths: Paths = parse_dir(&source);
let results: PathsPacked = basic_listing(paths);
println!(results);
```

### python template cookiecutter

Since i learn to use cookiecutter at Superprod, thanks to Jordie Bastide and Marc Dubrois. I can't stop using it. I wrote a couple of ones for **python 3** at Fortiche.

My latest one is [rusty-cookie](https://github.com/doubleailes/cookiecutter-rust) which a offer a strong base to create a rust package with a wonderful documentation based on [zola](https://www.getzola.org/) and [adidoks](https://github.com/aaranxu/adidoks).

### Moana Island

In 2018, with the help of Tcherno, Vincent Debellis, Djl and [Benjamin Legros](https://github.com/BenMercenaries). We were the first one to re-assembly the Moana Island scene from Disney as far as i know.

![Moana Island](https://pbs.twimg.com/media/DlmFMdfX0AAwUyb?format=jpg&name=large)

## Work

I start as a compositing artist in London, a little bit of mattepainting, then i switch to pipeline TD. I worked at [Mercenaries Engenering](https://github.com/MercenariesEngineering) with [Benjamin Legros](https://github.com/BenMercenaries) and [Cyril Corvazier](https://github.com/hulud75). I had the chance to work on wonderfull project like [Nomand Land](https://www.imdb.com/title/tt9770150/). I'm now CTO at Fortiche Prod. I met a lot of peple in this industry and i'm very glad to work with them.

### Talks

I gave a couple of talks in the past. I love to share my knowledge and experience with the community. I think it's important to give back to the community that helped me grow. Thanks to all my co-speakers and the organizers of these events for their support and collaboration.
Here is a list of my talks or panels:


#### 2019

- [CGWIRE #1(FR)](https://diplomeo.com/actualite-meetup_1_films_d_animation_quelle_organisation)

#### 2020

- [PIDS 2020(FR)](https://youtu.be/MQuoRxaoSN4?si=fY94qDCJVpC8G6UY) - GPU vs CPU, quel rendu pour quel image ?
- [CGWIRE #3(FR)](https://youtu.be/B2Pc-Fx2TUM?si=g_iFlRsRRiwT9jEl) - Le coût financier et humain de la render farm

#### 2021

- [CGWIRE #8(FR)](https://www.youtube.com/live/CXyxaXGsjfQ?si=9RoKXMhN5Be5L_QV) - Meetup special Fortiche

#### 2022

- [PIDS 2022(FR)](https://youtu.be/aE4yVaMqOH4?si=zZP8ZIaC9KxYCSt8) - Études de cas animation: Arcane par Fortiche
- [FMX 2022(ENG)](https://fmx.de/en/history/fmx-2022/detail/event/23305) - ARCANE: A Potpourri of Fortiche
- [RAF 2022(FR)](https://youtu.be/Q_CMxj_6oKI?si=ptBODRQAa7VLhj7V) - Recruter et former les ITs pour les studios d'animation

#### 2023

- [SIGGRAPH 2023(ENG)](https://dl.acm.org/doi/10.1145/3577023.3585274) - Fortiche : Crafting the BridgeNE: A Potpourri of Fortiche

#### 2024

- [SIGGRAPH ASIA 2024(ENG)](https://asia.siggraph.org/2024/program/key-speakers/) - The (Hex)tech of Arcane Season 02

#### 2025

- [PIDS 2025(FR)](https://www.pids-enghien.fr/prog2025-24janv/) - The (Hex)Tech of Arcane Season 2
- [ANIMA 2025(ENG)](https://www.flagey.be/en/activity/12214-arcane-season-2-behind-the-scenes-futuranima-12) - The (Hex)tech of Arcane Season 02
- [FMX 2025(ENG)](https://fmx.de/en/program/program-2025/detail/event/32906) - The (Hex)tech of Arcane Season 02
- [DEVOXX 2025(FR)](https://youtu.be/ekM8V_u_uD4?si=-1yUH2C--KO4mS9k) - Arcane: Quand la technologie n’est pas le produit: une série d’animation

## Hobbies

I'm a big fan of [central texas style BBQ](https://www.instagram.com/fireandfurybbq/), spirits, [Urbex](https://www.360cities.net/profile/doubleailes)(my profile picture was shot in a municipal pool). I used to was into [photography](https://www.flickr.com/photos/doubleailes/) but i don't have time anymore.

### Central texas style BBQ

I was always interested in smoky flavor. I smoke cigars but not so much and peated whisky. In 2014 in Paris opend the first texan bbq joint. This place was the only reconize texan bbq outside of texas, **The Beast**. [Crazy stories about this restaurant](https://www.texasmonthly.com/bbq/the-beast/), [New York Times](http://www.nytimes.com/interactive/2015/08/23/travel/paris-restaurants-barbecue.html), [Whasinghton Post](https://www.washingtonpost.com/lifestyle/food/move-over-foie-gras-the-latest-rage-in-paris-is--classic-american-barbecue/2016/01/15/1b3ff700-ba52-11e5-829c-26ffb874a18d_story.html) I started to be friend with the [owner, Thomas](https://www.texasmonthly.com/bbq/interview-thomas-abramowicz-of-the-beast/). But sadly **The Beast** closed during COVID and i was part of his friends who helped him to remove the last furniture.
So in 2020 my girlfriend offer me a big green egg to start bbq myself. After a couple of years i bought in 2023 my first offset smoker from Texas, a mill scale 94 Gallon built in Lockhart, TX.

Central texas style is defined by 3 things:

- Salt and pepper rub
- Post oak wood
- Low and slow

There is no post oak in France so i use [ashwood](https://en.wikipedia.org/wiki/Fraxinus) from my family wood and i'll start to plant my own trees.

[What is the Best Wood for Smoking Meat?](https://www.chadsbbq.com/what-is-the-best-wood-for-smoking-meat-part-2/)

I read a lots of book about it. The major one is: [Aaron Franklin, smoke.](https://www.amazon.fr/Franklin-Smoke-Wood-Fire-Cookbook/dp/1984860488)

I'm now cooking for friends and family and i'm very glad to share my passion with them.

Anytime i'm traveling, i try to visit bbq joint. I visited:

- [Hometown BBQ](https://www.hometownbbq.com/) in Brooklyn, NY
- [Moo's Craft BBQ](https://www.mooscraftbarbecue.com/) in Los Angeles, CA
- [Horse Thief BBQ](https://www.horsethiefbbq.com/) in Los Angeles, CA
- [Smokestack](https://www.smokestak.co.uk/) in London, UK
- [Heritage BBQ](https://www.heritagecraftbbq.com) in Los Angeles, CA.

## Contact

You can reach me on [Twitter](https://twitter.com/doubleailes) or [LinkedIn](https://www.linkedin.com/in/philippe-llerena-89a24013/).

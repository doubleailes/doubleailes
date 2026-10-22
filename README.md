# Hi there 👋

I'm Philippe, CTO at [Fortiche Prod](https://www.forticheprod.com/). Yep, the **Arcane** folks. I've been messing around with pixels in VFX and animation since 2005ish. My side quest these days is rewriting the VFX stack in Rust, one library at a time, because apparently I don't sleep.

## What I'm hacking on

It all started during COVID with a joke with [Paul](https://github.com/pypoulp) and one too many fights with the [GIL](https://en.wikipedia.org/wiki/Global_interpreter_lock). Now I can't stop porting things to Rust. Everything here is a work in progress, so expect sharp edges:

- **[crust-render](https://github.com/doubleailes/crust-render)**: a path tracer in safe Rust that reads USD natively. The goal is to render Moana Island and ALab without crying. MaterialX, OpenPBR and MIS are all in there.
- **[ocio-rs](https://github.com/doubleailes/ocio-rs)**: OpenColorIO, but make it Rust.
- **[OpenSubdiv-rs](https://github.com/doubleailes/OpenSubdiv-rs)**: subdivision surfaces, still oxidizing.
- **[ptex-rs](https://github.com/doubleailes/ptex-rs)**: Ptex, but crab-shaped.
- **[openqmc-rs](https://github.com/doubleailes/openqmc-rs)**: a faithful port of ASWF's [openqmc](https://github.com/AcademySoftwareFoundation/openqmc). Sobol, lattice and PMJ samplers, plus blue noise, because random is overrated.

## Off the grid: Reticulum

When I'm not rendering things, I'm sending messages without the internet. [Reticulum](https://reticulum.network/) is a networking stack for resilient, encrypted mesh networks that run over LoRa, packet radio, Wi-Fi or whatever wire you have lying around. LXMF is its messaging layer. Naturally, I'm bringing Rust to the party:

- **[LXMF-rs](https://github.com/doubleailes/LXMF-rs)**: an LXMF implementation in Rust.
- **[foxhole](https://github.com/doubleailes/foxhole)**: a terminal LXMF client in Rust, built on the wonderful work of Ratspeak. Chatting over radio, from your terminal, like it's 1994 but encrypted.

## Places I've talked too much

I love sharing what we break and fix along the way. The highlights:

- [SIGGRAPH Asia 2024](https://asia.siggraph.org/2024/program/key-speakers/): key speaker, *The (Hex)tech of Arcane Season 2*
- [FMX 2025](https://fmx.de/en/program/program-2025/detail/event/32906): *The (Hex)tech of Arcane Season 2*
- [Devoxx France 2025](https://youtu.be/ekM8V_u_uD4?si=-1yUH2C--KO4mS9k): *Arcane : quand la technologie n'est pas le produit*
- [SIGGRAPH 2023](https://dl.acm.org/doi/10.1145/3577023.3585274): *Fortiche: Crafting the Bridge* <!-- TODO: check the exact title; the old README merged it with the FMX 2022 one -->
- [FMX 2022](https://fmx.de/en/history/fmx-2022/detail/event/23305): *Arcane: A Potpourri of Fortiche*

<details>
<summary>The full list, for the brave</summary>

#### 2025

- [PIDS 2025 (FR)](https://www.pids-enghien.fr/prog2025-24janv/): The (Hex)tech of Arcane Season 2
- [ANIMA 2025 (EN)](https://www.flagey.be/en/activity/12214-arcane-season-2-behind-the-scenes-futuranima-12): The (Hex)tech of Arcane Season 2
- [FMX 2025 (EN)](https://fmx.de/en/program/program-2025/detail/event/32906): The (Hex)tech of Arcane Season 2
- [Devoxx 2025 (FR)](https://youtu.be/ekM8V_u_uD4?si=-1yUH2C--KO4mS9k): Arcane : quand la technologie n'est pas le produit, une série d'animation

#### 2024

- [SIGGRAPH Asia 2024 (EN)](https://asia.siggraph.org/2024/program/key-speakers/): The (Hex)tech of Arcane Season 2

#### 2023

- [SIGGRAPH 2023 (EN)](https://dl.acm.org/doi/10.1145/3577023.3585274): Fortiche: Crafting the Bridge

#### 2022

- [PIDS 2022 (FR)](https://youtu.be/aE4yVaMqOH4?si=zZP8ZIaC9KxYCSt8): Études de cas animation, Arcane par Fortiche
- [FMX 2022 (EN)](https://fmx.de/en/history/fmx-2022/detail/event/23305): Arcane: A Potpourri of Fortiche
- [RAF 2022 (FR)](https://youtu.be/Q_CMxj_6oKI?si=ptBODRQAa7VLhj7V): Recruter et former les ITs pour les studios d'animation

#### 2021

- [CGWIRE #8 (FR)](https://www.youtube.com/live/CXyxaXGsjfQ?si=9RoKXMhN5Be5L_QV): Meetup spécial Fortiche

#### 2020

- [PIDS 2020 (FR)](https://youtu.be/MQuoRxaoSN4?si=fY94qDCJVpC8G6UY): GPU vs CPU, quel rendu pour quelle image ?
- [CGWIRE #3 (FR)](https://youtu.be/B2Pc-Fx2TUM?si=g_iFlRsRRiwT9jEl): Le coût financier et humain de la render farm

#### 2019

- [CGWIRE #1 (FR)](https://diplomeo.com/actualite-meetup_1_films_d_animation_quelle_organisation)

</details>

Big thanks to every co-speaker and organizer who put up with me.

## Older toys

- **[framels (fls)](https://github.com/forticheprod/fls)**: `ls`, but it actually understands image sequences. It's inspired by `bls` from [BUF Compagnie](https://buf.com/) and `rvls` from RV. Try `cargo add framels` and say goodbye to scrolling through 4,000 EXRs.

  ![fls demo](https://github.com/forticheprod/fls/blob/main/images/fls_demo.gif)

  ```rust
  use framels::{basic_listing, parse_dir, paths::{Paths, PathsPacked}};

  let paths: Paths = parse_dir("./samples/big");
  let results: PathsPacked = basic_listing(paths);
  println!("{:?}", results);
  ```

- **[girolle](https://github.com/doubleailes/girolle)**: talk to [nameko](https://github.com/nameko/nameko) microservices from Rust. Proc macros and I are still in couples therapy.
- **[rer](https://github.com/doubleailes/rer)**: a [rez](https://github.com/AcademySoftwareFoundation/rez) solver in Rust, because resolving environments should be fast.
- **[quiet-stroll](https://github.com/forticheprod/quiet-stroll)**: a Rust tool from Fortiche. <!-- TODO: add a real one-liner -->
- **[cookiecutter-rust](https://github.com/doubleailes/cookiecutter-rust)**: a Rust project template with [Zola](https://www.getzola.org/) and [AdiDoks](https://github.com/aaranxu/adidoks) docs. Jordie Bastide and Marc Dubrois got me hooked on cookiecutter at Superprod, and I never recovered.
- **Moana Island (2018)**: Tcherno, Vincent Debellis, Djl, [Benjamin Legros](https://github.com/BenMercenaries) and I reassembled Disney's Moana Island scene. As far as I know, we were the first to pull it off.

  ![Moana Island](https://pbs.twimg.com/media/DlmFMdfX0AAwUyb?format=jpg&name=large)

## How I got here

Compositing in London → a bit of matte painting → pipeline TD → [Mercenaries Engineering](https://github.com/MercenariesEngineering), hanging out with [Benjamin Legros](https://github.com/BenMercenaries) and [Cyril Corvazier](https://github.com/hulud75) and working on fun stuff like [Nomadland](https://www.imdb.com/title/tt9770150/) → CTO at Fortiche. I met a ton of great people along the way.

## When I'm not at a keyboard

- **Central Texas BBQ.** Salt, pepper, smoke, patience. France has no post oak, so I burn [ash](https://en.wikipedia.org/wiki/Fraxinus) from my family's woods and I'm planting my own trees (see you in 30 years). It all started at **The Beast**, Paris's legendary Texan joint ([crazy story here](https://www.texasmonthly.com/bbq/the-beast/)). I became friends with [Thomas, the owner](https://www.texasmonthly.com/bbq/interview-thomas-abramowicz-of-the-beast/), and I helped carry out the last furniture when it closed during COVID. I started on a Big Green Egg in 2020, and these days I cook on a 94-gallon Mill Scale offset shipped all the way from Lockhart, TX. My bible: [Franklin Smoke](https://www.amazon.fr/Franklin-Smoke-Wood-Fire-Cookbook/dp/1984860488). Pit stops so far: [Hometown](https://www.hometownbbq.com/) (Brooklyn), [Moo's Craft](https://www.mooscraftbarbecue.com/), [Horse Thief](https://www.horsethiefbbq.com/) and [Heritage](https://www.heritagecraftbbq.com) (LA), and [Smokestak](https://www.smokestak.co.uk/) (London). Smoke signals at [@fireandfurybbq](https://www.instagram.com/fireandfurybbq/).
- **[Fury](https://www.instagram.com/furythedestroyer)**, my jackhuahua. She's called Fury because she is furious. No further questions.
- **Urbex** ([360cities](https://www.360cities.net/profile/doubleailes)). Yes, my profile pic was shot in a municipal pool. I used to do [photography](https://www.flickr.com/photos/doubleailes/) too, before life got busy.
- **Languages**: French, English and Python, all fluently. I speak a little Japanese and Spanish, I forgot all my Java, and I started out writing BASIC on my dad's Casio and a TI-89.

## Say hi

[X / Twitter](https://twitter.com/doubleailes) · [LinkedIn](https://www.linkedin.com/in/philippe-llerena-89a24013/) · or come for brisket

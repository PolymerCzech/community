# Polymeristi - tvoříme lepší web zítřka <sup><sub>CZ & SK <a href="https://github.com/Polymeristi/readme/compare/v1.3.0...v1.4.0#files_bucket">v1.4.0</a> - 2018-04-18</sub></sup>

[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://help.github.com/articles/about-pull-requests/)

- [Proč Polymer?](#proč-polymer)
- [Co je to Polymer Project?](#co-je-to-polymer-project)
  - [Webová komponenta](#webová-komponenta)
  - [Jak na SEO?](#jak-na-seo)
- [Motto #UseWebPlatform](#motto-usewebplatform)
- [Místa kde diskutujeme](#místa-kde-diskutujeme)
  - [Pravidla diskuse](#pravidla-diskuse)
- [Novinky, události, srazy](#novinky-události-srazy)
- [Nabídky práce](#nabídky-práce)
- [Jak začít?](#jak-začít)
- [FAQ](#faq)

## Proč Polymer?

Projekt Polymer a kombinace technologií HTTP/2, W3C Service Workers, W3C HTML Templates, W3C Custom Elements, W3C CSS Custom Properties, W3C Shadow DOM, JavaScript ES6 Modules a vzoru [PRPL-50](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs/blob/master/README.md#prpl-50) nám umožňují tvořit **rychlé, modulární, dlouhodobě udržitelné a čitelné pro většinu vývojářů** SPA nebo PWA aplikace i pro pomalé a nestabilní sítě.

[Progresivní webové aplikace (PWA)](https://developers.google.com/web/progressive-web-apps/) jsou spolehlivé, rychlé a vytváří dojem plnohodnotné aplikace. Nevyžadují instalaci a centrální app store pro aktualizace a dohledatelnost.

:sparkles: Jen čisté HTML, CSS, JS. :sparkles: Lehká Polymer knihovna je postavena na Ecma a W3C standardech, takže nás nenutí se učit nové API či jazyky. :+1: :tada:

Na projektu Polymer je postaven např. [nový YouTube](https://www.youtube.com/new), který je díky němu modulární a [rychlejší o 15%](https://www.youtube.com/watch?v=tNulrEbTQf8&index=8&list=PLNYkxOF6rcIDP0PqVaJxqNWwIgvoEPzJi&t=22m2s). :+1:

<p align="center">
  <a href="https://www.youtube.com/watch?v=eG0ILA2k5qo&list=PLNYkxOF6rcICUD5nBfRdAR6Fveosnqa5m&index=13" target="_blank"><img src="https://raw.githubusercontent.com/Polymeristi/readme/master/images/pwa-vs-native-apps.png" alt="PWA vs nativní aplikace" title="PWA vs nativní aplikace"></a>
</p>

PWA aplikace v produkci ukazují, že mají význam, viz statistiky [PWA Stats](https://www.pwastats.com). :+1:

Více informací o PWA je na stránce [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs#8-progresivní-webové-aplikace-pwa). :eyes:

## Co je to Polymer Project?

<p align="center">
  <img src="https://raw.githubusercontent.com/Polymeristi/readme/master/images/history-of-javascript-frameworks.png" alt="Historie Javascript frameworků" title="Historie Javascript frameworků">
</p>

[Polymer Project](https://github.com/StartPolymer/awesome-polymer#general-resources) je open-source projekt veden týmem front-endových vývojářů v rámci projektu Chrome ve společnosti Google.

Cílem projektu je vytvořit knihovny, nástroje a architektonické vzory, které umožní vývojářům vytvářet moderní [progresivní webové aplikace (PWA)](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs#8-progresivní-webové-aplikace-pwa) s plným využitím špičkových API webové platformy jako jsou W3C [Web Components](https://www.webcomponents.org/introduction), W3C [Service Workers](https://developers.google.com/web/fundamentals/primers/service-workers/) a protokolu [HTTP/2](https://developers.google.com/web/fundamentals/performance/http2/).

Lehká Polymer knihovna jen usnadňuje zápis W3C standardů ([syntactic sugar](https://en.wikipedia.org/wiki/Syntactic_sugar)) a nevytváří vlastní vrstvu jako ostatní frameworky, tím ji lze použít s libovolným frameworkem nebo knihovnou (např. Angular, Redux) díky projektu [Custom Elements Everywhere](https://custom-elements-everywhere.com).

Projekt Polymer nás nepoutá k žádnému full-stack řešení. Je v synergii s moderní architekturou [JAMstack](https://jamstack.org). Tento stack dobře vysvětluje přednáška [JAMstack, moderní architektura pro stavbu webů](https://www.youtube.com/watch?v=AmdSoR-x7bE).

Vývojáři z projektu Polymer mají vizi ve webovém designeru, kde si budem moci webovou aplikaci poskládat pomocí již hotových elementů. Prvním prototypem byl [Polymer Designer](https://polymer-designer.appspot.com) ([video](https://www.youtube.com/watch?v=djQh8XKRzRg), [git](https://github.com/polymer/designer)) a druhým [wizzywid](https://polymerlabs.github.io/wizzywid/) ([video](https://www.youtube.com/watch?v=otcmcNY-3pk&list=PLNYkxOF6rcIDP0PqVaJxqNWwIgvoEPzJi&index=14), [git](https://github.com/PolymerLabs/wizzywid)).

S Polymerem je již vytvořeno několik webových stránek a aplikací, např. [nový YouTube](https://www.youtube.com/new), [Google Earth](https://www.google.com/earth/), Google Play Music, Google Sites, Chrome PDF viewer, Chrome Settings, Electronic Arts, IBM Bluemix console, atd.

- [Seznam webových stránek a aplikací vytvořených s Polymerem.](https://github.com/abdonrd/PolymerProjects)
- [Polymer @ YouTube - Stránka YouTube se skládá z více než 400 webových komponent.](https://www.youtube.com/watch?v=tNulrEbTQf8)

### Webová komponenta

Webová komponenta je modul, který se skládá z několika významných vrstev. Tyto moduly komunikují mezi sebou pomocí vzoru [Mediator Pattern](https://github.com/StartPolymer/awesome-polymer#managing-state).

<p align="center">
  <img src="https://raw.githubusercontent.com/Polymeristi/readme/master/images/web-component.png" alt="Webová komponenta" title="Webová komponenta">
</p>

### Jak na SEO?

Polymer projekt vyvíjí [PRPL server](https://github.com/Polymer/prpl-server-node), který umí search bótům podstrčit statickou stránku (bez JavaScriptu) vygenerovanou pomocí [Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome).

Více informací v sekci [Polymer is SEO-friendly na stránce Awesome Polymer](https://github.com/StartPolymer/awesome-polymer#polymer-is-seo-friendly).

## Motto #UseWebPlatform

Naše motto [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs) obsahuje pravidla pro lepší web a vysvětluje misi projektu Polymer.

## Místa kde diskutujeme

- [**facebook**.com/groups/polymeristi](https://www.facebook.com/groups/polymeristi)
- [#polymeristi @ polymer.**slack**.com](https://polymer.slack.com) - [registrace zde](https://polymer-slack.herokuapp.com)
  - Je nás už přes 9000...
  - ![Polymer na Slacku](https://raw.githubusercontent.com/Polymeristi/readme/master/images/slack-polymer.png)
- [**plus.google**.com/u/0/communities](https://plus.google.com/u/0/communities/100749807415316706653)

### Pravidla diskuse

1. DRŽÍME TÉMA  
Diskutujeme hlavně o projektu Polymer a na téma [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs). Téma držíme i v otevřených diskuzích.

2. NESPAMUJEME  
Nabídky práce patří na [pracovní forum Polymeristů](https://www.facebook.com/groups/polymeristi.prace/). Reklama na produkty a služby sem nepatří.

3. NELADÍME CHYBY  
Bugy softwaru patří do jeho Github issues, technické zádrhele zase na StackOverflow.

4. PTÁME SE PŘESNĚ  
Pokud vám něco nefunguje: uveďte, v čem je problém a co je očekávaný výsledek. Přiložte ukázku kódu v aplikaci CodeSandbox, JSFiddle nebo CodePen.

5. NEDUPLIKUJEME DOTAZY  
Než se zeptáte, vyhledáváním si zjistěte, zda už se to v diskusi neřešilo.
    - [Slack Search](https://polymer.slack.com/messages/C790AMQKH/search/redux/)
    - [G+ Community Search](https://plus.google.com/u/0/communities/100749807415316706653/s/redux)
    - [Facebook Group Search](https://facebook.com/groups/polymeristi/search/?query=redux)

6. DISKUTUJEME VĚCNĚ, SLUŠNĚ A S RESPEKTEM K DRUHÝM  
Všechny názory podepíráme argumenty. Žádné osobní útoky. Nováčkům se nesmějeme, naopak je vřele vítáme.

7. TYKÁME SI  
Tykání nenutíme, ale připravte se na to, že vám v diskusi tykat budou.

## Novinky, události, srazy

- [facebook.com/Polymeristi](https://www.facebook.com/Polymeristi)
- [twitter.com/Polymeristi](https://twitter.com/Polymeristi)

## Nabídky práce

Nabídky práce podáváme a hlídáme na [pracovním foru Polymeristů](https://www.facebook.com/groups/polymeristi.prace/).

## Jak začít?

1. Zkoukněte videa z playlistu [Polycasts](https://www.youtube.com/playlist?list=PLNYkxOF6rcIDdS7HWIC_BYRunV6MHs5xo).
2. Objevte sílu lehké knihovny Polymer v online editoru pomocí [StartPolymer Playgrounds](https://github.com/StartPolymer/playgrounds).
3. Použijte základní šablonu pro PWA aplikace [Polymer Starter Kit](https://github.com/PolymerElements/polymer-starter-kit).
4. Zkoukněte kód [demo PWA shopu](https://github.com/Polymer/shop), [demo PWA news](https://github.com/Polymer/news) a PWA aplikace [Polymer Summit 2017](https://github.com/Polymer/summit-2017).
5. V kolekci zdrojů [Awesome Polymer](https://github.com/StartPolymer/awesome-polymer) naleznete užitečné odkazy.

## FAQ

- Proč projekt Polymer opustil HTML importy ve verzi 3.0?
  - Během několika let se nepodařilo prosadit HTML importy u ostatních prohlížečů (Safari, Firefox, Edge). JS ES6 moduly jsou na druhou stranu pěknou alternativou. Viz například [demo shopu přepsané do Polymer 3.0](https://github.com/Polymer/shop/blob/3.0/src/shop-app.js). Dále díky tomuto přechodu vznikl skvělý [lit-html](https://github.com/Polymer/lit-html).

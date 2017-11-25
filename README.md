# Polymeristi - tvoříme lepší web zítřka <sup><sub>CZ & SK <a href="https://github.com/Polymeristi/readme/compare/v1.1.0...v1.2.0#files_bucket">v1.2.0</a></sub></sup>

[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://help.github.com/articles/about-pull-requests/)

- [Proč Polymer?](#proč-polymer)
- [Motto #UseWebPlatform](#motto-usewebplatform)
- [Co je to Polymer Project?](#co-je-to-polymer-project)
  - [Webová komponenta](#webová-komponenta)
  - [Jak na SEO?](#jak-na-seo)
- [Místa kde diskutujeme](#místa-kde-diskutujeme)
  - [Pravidla diskuse](#pravidla-diskuse)
- [Novinky, události, srazy](#novinky-události-srazy)
- [Nabídky práce](#nabídky-práce)
- [Jak začít?](#jak-začít)
- [FAQ](#faq)

## Proč Polymer?

Projekt Polymer nám umožňuje tvořit **rychlé modulární** [progresivní webové aplikace (PWA)](https://developers.google.com/web/progressive-web-apps/), které se chovají "stejně" jako nativní aplikace na platformě Android, iOS či Windows (na iOS a Windows není zatím plná podpora). Na platformách [Chrome OS](https://www.google.cz/search?q=Chrome+OS) ([Chromebook](https://www.google.cz/search?q=Chromebook), [Chromebox](https://www.google.cz/search?q=Chromebox), [Chromebase](https://www.google.cz/search?q=Chromebase)) a [Chromium OS](https://www.chromium.org/chromium-os) ([CloudReady](https://www.neverware.com)) beží PWA nativně. Jejich progresivní přístup jim umožňuje běžet vlastně kdekoliv. :tada:

Více informací je na stránce [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs#8-progresivní-webové-aplikace-pwa).

## Motto #UseWebPlatform

Naše motto [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs) obsahuje pravidla pro lepší web a vysvětluje misi projektu Polymer.

## Co je to Polymer Project?

<p align="center">
  <img src="https://raw.githubusercontent.com/Polymeristi/readme/master/images/history-of-javascript-frameworks.png" alt="Historie Javascript frameworků" title="Historie Javascript frameworků">
</p>

[Polymer Project](https://github.com/StartPolymer/awesome-polymer#general-resources) je open-source projekt veden týmem front-endových vývojářů v rámci organizace Chrome ve společnosti Google.

Cílem projektu je vytvořit knihovny, nástroje a architektonické vzory, které pomůžou vývojářům vytvářet moderní [progresivní webové aplikace (PWA)](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs#8-progresivní-webové-aplikace-pwa) s plným využitím špičkových funkcí webové platformy jako jsou W3C [Web Components](https://www.webcomponents.org/introduction), W3C [Service Workers](https://developers.google.com/web/fundamentals/primers/service-workers/) a protokolu IETF [HTTP/2](https://developers.google.com/web/fundamentals/performance/http2/) od vývojářů z projektu Polymer.

Polymer knihovna nevytváří vlastní vrstvu jako ostatní frameworky, tím ji lze použít s libovolným frameworkem nebo knihovnou, např. Angular, Redux.

Projekt Polymer nás nepoutá k žádnému full-stack řešení, viz pravidlo [Negenerujte HTML na straně serveru](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs#4-negenerujte-html-na-straně-serveru).

Vývojáři z projektu Polymer mají vizi ve webovém designeru, kde si budem moci webovou aplikaci poskládat pomocí již hotových elementů. Prvním prototypem byl [Polymer Designer](https://polymer-designer.appspot.com) ([video](https://www.youtube.com/watch?v=djQh8XKRzRg), [git](https://github.com/polymer/designer)) a druhým [wizzywid](https://polymerlabs.github.io/wizzywid/) ([video](https://www.youtube.com/watch?v=otcmcNY-3pk&list=PLNYkxOF6rcIDP0PqVaJxqNWwIgvoEPzJi&index=14), [git](https://github.com/PolymerLabs/wizzywid)).

S Polymerem je již vytvořeno několik webových stránek a aplikací, např. [nový Youtube](https://www.youtube.com/new), [Google Earth](https://www.google.com/earth/), Google Play Music, Google Sites, Chrome PDF viewer, Chrome Settings, Electronic Arts, IBM Bluemix console, atd.

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

## Místa kde diskutujeme

- [#polymeristi @ polymer.slack.com](https://polymer.slack.com) - [registrace zde](https://polymer-slack.herokuapp.com)
  - Je nás už přes 9000...
  - ![Polymer na Slacku](https://raw.githubusercontent.com/Polymeristi/readme/master/images/slack-polymer.png)
- [facebook.com/groups/polymeristi](https://www.facebook.com/groups/polymeristi)
- [plus.google.com/u/0/communities](https://plus.google.com/u/0/communities/100749807415316706653)

### Pravidla diskuse

1. Diskutujeme hlavně o projektu Polymer a na téma [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform-cs).
2. Než se zeptáte, vyhledáváním si zjistěte, zda už se to neřešilo.
   - [Slack Search](https://polymer.slack.com/messages/C790AMQKH/search/redux/)
   - [G+ Community Search](https://plus.google.com/u/0/communities/100749807415316706653/s/redux)
   - [Facebook Group Search](https://facebook.com/groups/polymeristi/search/?query=redux)
3. Neladíme zde chyby. Bugy patří do Github issues, technické zádrhele zase na StackOverflow.
4. Diskutujeme věcně. Všechny názory podepíráme argumenty.
5. Diskutujeme slušně. Žádné osobní útoky. Nováčkům se nesmějeme, naopak je vřele vítáme.
6. **Nabídky práce** patří na stránku [Polymeristi/prace](https://github.com/Polymeristi/prace).
7. Příspěvky s vypnutým komentováním budou smazány.
8. V diskusi si tykáme.

## Novinky, události, srazy

- [twitter.com/Polymeristi](https://twitter.com/Polymeristi)
- [facebook.com/Polymeristi](https://www.facebook.com/Polymeristi)

## Nabídky práce

Nabídky práce podáváme a hlídáme (přes Watch button) na stránce [Polymeristi/prace](https://github.com/Polymeristi/prace).

## Jak začít?

1. Hrajeme si s Polymerem v online editoru přes stránku [StartPolymer/playgrounds](https://github.com/StartPolymer/playgrounds). :eyes:
2. Základní šablona pro PWA aplikace se jmenuje [Polymer Starter Kit](https://github.com/PolymerElements/polymer-starter-kit).
3. Máme kolekci zdrojů [Awesome Polymer](https://github.com/StartPolymer/awesome-polymer).

## FAQ

- Hot Reloading?
  - [StartPolymer Toolbox](https://github.com/StartPolymer/toolbox) - obsahuje tool pro Hot Reloading

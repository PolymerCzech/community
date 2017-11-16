# Polymeristi - tvoříme lepší web zítřka (CZ & SK)

[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://help.github.com/articles/about-pull-requests/)

- [Naše desatero](#naše-desatero)
- [Co je to Polymer Project?](#co-je-to-polymer-project)
  - [Architektonické vzory](#architektonické-vzory)
  - [Hot Reloading](#hot-reloading)
  - [Jak na SEO?](#jak-na-seo)
- [Místa kde diskutujeme](#místa-kde-diskutujeme)
  - [Pravidla diskuse](#pravidla-diskuse)
- [Novinky, události, srazy](#novinky-události-srazy)
- [Nabídky práce](#nabídky-práce)
- [Zdroje](#zdroje)
- [FAQ](#faq)

## Naše desatero

1. Tvoříme lepší web postavený na nových W3C standardech [Custom Elements v1](https://developers.google.com/web/fundamentals/web-components/customelements) a [Shadow DOM v1](https://developers.google.com/web/fundamentals/getting-started/primers/shadowdom). W3C [DOM](https://en.wikipedia.org/wiki/Document_Object_Model) je náš framework. Naše motto je [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform).

2. Nepotřebujeme těžké frameworky (Angular, Bootstrap, jQuery, React, Vue, atd.), které zpomalují načtení  
(žerou data, výkon i baterii) a omezují vývoj front-endu. Srovnání frameworků pomocí PWA je na [HNPWA](https://hnpwa.com).

3. Komplexní webové aplikace tvoříme modulárně z mnoha zapouzdřených custom elementů s vlastním stromem pomocí [Shadow DOM](https://meowni.ca/posts/shadow-dom/). Jednotlivé elementy pak stahujeme (jen jednou) na základě dané URL, kde jsou třeba pro render na straně klienta. Hlídáme velikost stažených dat do **50 KB** per URL, což nám zajišťuje rychlé načtení stránky na mobilních 3G sítích, viz [PRPL-50](https://github.com/UseWebPlatform/motto-UseWebPlatform#prpl-50).

4. Nepotřebujeme SSR (Server Side Rendering), např. Django, PHP, React, Tomcat, Vue. Kombinace CSR (Client Side Rendering) + [PRPL vzor](https://github.com/UseWebPlatform/motto-UseWebPlatform/blob/master/README.md#8-prpl-pattern) + [CDN](https://cs.wikipedia.org/wiki/Content_delivery_network) řeší rychlé načtení front-endu. Komunikace s back-endem probíhá přes [JSON API](http://jsonapi.org), [GraphQL](http://graphql.org) nebo [REST API](https://cs.wikipedia.org/wiki/Representational_State_Transfer). Příkladem je [JAMstack](https://jamstack.org).

5. Programujeme v čistém jazyce [JavaScript ES6](http://es6-features.org). Jazyk TypeScript a jiné JS preprocessory nepotřebujeme, máme statické typy na úrovni custom elementů. Nepotřebujeme CSS preprocessory (SASS, LESS, Stylus), neboť máme [CSS Properties](https://www.polymer-project.org/2.0/docs/devguide/custom-css-properties) a [CSS Mixins](https://www.polymer-project.org/2.0/docs/devguide/custom-css-properties#use-custom-css-mixins).

6. Dodržujeme metodu [progressive enhancement](https://www.zdrojak.cz/clanky/graceful-degradation-vs-progressive-enhancement/) za pomoci [polyfillů](https://www.polymer-project.org/2.0/docs/polyfills) a [pravidla přístupného webu](http://www.pravidla-pristupnosti.cz), s kterýma nám pomáhají již vytvořené Polymer komponenty.

7. Dodržujeme checklist pro custom elementy [The Gold Standard Checklist for Web Components](https://github.com/webcomponents/gold-standard/wiki).

8. Tvoříme modulární [PWA aplikace](https://github.com/UseWebPlatform/motto-UseWebPlatform#5-progressive-web-apps) s architekturou [App Shell](https://developers.google.com/web/fundamentals/architecture/app-shell) dle checklistu [Progressive Web App Checklist](https://developers.google.com/web/progressive-web-apps/checklist). 

9. Píšeme [dokumentaci](https://www.polymer-project.org/2.0/docs/tools/documentation) a [testy pomocí Web Component Tester](https://www.polymer-project.org/2.0/docs/tools/tests) pro každý znovu použitelný custom element, který žije ve vlastním git repozitáři s landing a demo stránkou.

10. Jsme na platformě GitHub, kde publikujeme své veřejné znovu použitelné custom elementy pro ostatní. Tyto elementy pak ukládáme do katalogu [webcomponents.org](https://www.webcomponents.org). Notifikace z platformy GitHub hlídáme pomocí aplikace [Octobox](https://octobox.io).

## Co je to Polymer Project?

[Polymer Project](https://github.com/UseWebPlatform/motto-UseWebPlatform#10-polymer-project) je open-source projekt veden týmem front-endových vývojářů v rámci organizace Chrome ve společnosti Google.

Cílem projektu je vytvořit knihovny, nástroje a architektonické vzory, které pomůžou vývojářům vytvářet moderní [PWA (Progressive Web Apps)](https://github.com/UseWebPlatform/motto-UseWebPlatform#5-progressive-web-apps) aplikace s plným využitím špičkových funkcí platformy jako jsou [Web Components](https://github.com/UseWebPlatform/motto-UseWebPlatform#2-web-components), [Service Workers](https://github.com/UseWebPlatform/motto-UseWebPlatform#4-service-workers-web-workers) a [HTTP/2](https://github.com/UseWebPlatform/motto-UseWebPlatform#3-http2--server-push--html-imports--es6-modules).

Polymer knihovna nevytváří vlastní vrstvu jako ostatní frameworky, tím ji lze použít s libovolným frameworkem nebo knihovnou, např. Angular, Redux.

S Polymerem je již vytvořeno několik webových stránek a aplikací, např. [nový Youtube](https://www.youtube.com/new), [Google Earth](https://www.google.com/earth/), Google Play Music, Google Sites, Chrome PDF viewer, Chrome Settings, Electronic Arts, IBM Bluemix console, atd..

- [Seznam webových stránek a aplikací vytvořených s Polymerem.](https://github.com/abdonrd/PolymerProjects)
- [Polymer @ YouTube - Stránka YouTube se skládá z více než 400 webových komponent.](https://www.youtube.com/watch?v=tNulrEbTQf8)

### Architektonické vzory

- [PRPL Pattern](https://www.polymer-project.org/2.0/toolbox/prpl)
  - [End to End Apps with Polymer (Polymer Summit 2017)](https://www.youtube.com/watch?v=0A-2BhEZiM4)
- [UniFlow - uni-directional data flow + maintains state of entire application](https://github.com/google/uniflow-polymer)
  - [Difference between UniFlow and Redux](https://github.com/google/uniflow-polymer/issues/9)

Více informací v sekci [Patterns na stránce Awesome Polymer](https://github.com/StartPolymer/awesome-polymer/blob/master/README.md#patterns).

### Hot Reloading

- [StartPolymer Toolbox](https://github.com/StartPolymer/toolbox) - obsahuje tool pro Hot Reloading

### Jak na SEO?

Polymer projekt vyvíjí [PRPL server](https://github.com/Polymer/prpl-server-node), který umí search bótům podstrčit statickou stránku (bez JavaScriptu) vygenerovanou pomocí [Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome).

Více informací v sekci [Polymer is SEO-friendly na stránce Awesome Polymer](https://github.com/StartPolymer/awesome-polymer#polymer-is-seo-friendly).

## Místa kde diskutujeme

- [#polymeristi @ polymer.slack.com](https://polymer.slack.com) - [registrace zde](https://polymer-slack.herokuapp.com)
- [facebook.com/groups/polymeristi](https://www.facebook.com/groups/polymeristi)
- [plus.google.com/u/0/communities](https://plus.google.com/u/0/communities/100749807415316706653)

### Pravidla diskuse

1. Diskutujeme hlavně o projektu Polymer a na téma [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform).
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

## Zdroje

Máme kolekci zdrojů [Awesome Polymer](https://github.com/StartPolymer/awesome-polymer).

Hrajeme si s Polymerem v online editoru na stránce [StartPolymer/playgrounds](https://github.com/StartPolymer/playgrounds). :eyes:

## FAQ

- TBD

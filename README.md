# Polymeristi - tvoříme lepší web zítřka

[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://help.github.com/articles/about-pull-requests/)

Tvoříme lepší web bez těžkých frameworků (Angular, Bootstrap, jQuery, React, Vue, atd.), které zpomalují načtení  
(žerou data, výkon i baterii) a omezují vývoj front-endu. Srovnání frameworků pomocí PWA je na [HNPWA](https://hnpwa.com).

Komplexní webové aplikace tvoříme modulárně z mnoha zapouzdřených custom elementů s vlastním stromem pomocí [Shadow DOM](https://meowni.ca/posts/shadow-dom/).

Nepotřebujeme SSR (Server Side Rendering), např. Django, PHP, React, Tomcat, Vue. Kombinace CSR (Client Side Rendering) + [PRPL vzor](https://github.com/UseWebPlatform/motto-UseWebPlatform/blob/master/README.md#8-prpl-pattern) + [CDN](https://cs.wikipedia.org/wiki/Content_delivery_network) řeší rychlé načtení front-endu. Komunikace s back-endem probíhá přes [JSON API](http://jsonapi.org), [GraphQL](http://graphql.org) nebo [REST API](https://cs.wikipedia.org/wiki/Representational_State_Transfer). Příkladem je [JAMstack](https://jamstack.org).

Naše motto je [#UseWebPlatform](https://github.com/UseWebPlatform/motto-UseWebPlatform).

## Co je to Polymer Project?

[Polymer Project](https://github.com/UseWebPlatform/motto-UseWebPlatform#10-polymer-project) je open-source projekt veden týmem front-endových vývojářů v rámci organizace Chrome ve společnosti Google.

Cílem projektu je vytvořit knihovny, nástroje a vývojářské vzory, které pomůžou vývojářům vytvářet moderní [PWA (Progressive Web Apps)](https://github.com/UseWebPlatform/motto-UseWebPlatform#5-progressive-web-apps) aplikace s plným využitím špičkových funkcí platformy jako jsou [Web Components](https://github.com/UseWebPlatform/motto-UseWebPlatform#2-web-components), [Service Workers](https://github.com/UseWebPlatform/motto-UseWebPlatform#4-service-workers-web-workers) a [HTTP/2](https://github.com/UseWebPlatform/motto-UseWebPlatform#3-http2--server-push--html-imports--es6-modules).

Polymer knihovna nevytváří vlastní vrstvu jako ostatní frameworky, tím ji lze použít s libovolným frameworkem nebo knihovnou, např. Angular, Redux.

S Polymerem je již vytvořeno několik webových stránek a aplikací, např. [nový Youtube](https://www.youtube.com/new), [Google Earth](https://www.google.com/earth/), Google Play Music, Google Sites, Chrome PDF viewer, Chrome Settings, Electronic Arts, IBM Bluemix console, atd..

- [Seznam webových stránek a aplikací vytvořených s Polymerem.](https://github.com/abdonrd/PolymerProjects)
- [Polymer @ YouTube - Stránka YouTube se skládá z více než 400 webových komponent.](https://www.youtube.com/watch?v=tNulrEbTQf8)

### Jak na SEO?

Polymer projekt vyvíjí [PRPL server](https://github.com/Polymer/prpl-server-node), který umí search bótům podstrčit statickou stránku (bez JavaScriptu) vygenerovanou pomocí [Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome).

- [Solving SEO with Headless Chrome (Polymer Summit 2017)](https://www.youtube.com/watch?v=ydThUDlBDfc&index=21&list=PLNYkxOF6rcIDP0PqVaJxqNWwIgvoEPzJi)
- [Playground pro Puppeteer](https://try-puppeteer.appspot.com)
- [Rendertron - headless rendering service](https://render-tron.appspot.com)

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

## Novinky, události, srazy

- [twitter.com/Polymeristi](https://twitter.com/Polymeristi)
- [facebook.com/Polymeristi](https://www.facebook.com/Polymeristi)

## Zdroje

Máme kolekci zdrojů [Awesome Polymer](https://github.com/StartPolymer/awesome-polymer).

Vyzkoušejte si Polymer na hřišti v online editoru - [StartPolymer Playgrounds](https://github.com/StartPolymer/playgrounds). :eyes:

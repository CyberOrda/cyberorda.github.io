---
hide:
  - feedback
tags:
  - API
  - OWAPS
  - XSS
---

# **Frontend Security**

Рассмотрим некоторые уязвимости, которые могут встречатся в Frontend, а также инструменты, которыми их можно обнаружить.

## **Cross Site Scripting(xss)**

### **Reflected XSS**

* [Codegrazer: 7 отраженных межсайтовых скриптов (XSS)](http://codegrazer.com/blog/7-reflected-xss.html)
* [Построение XSS-вектора, не используя букв - inventropy](https://inventropy.us/blog/constructing-an-xss-vector-using-no-letters)
* [PwnDizzle: XSS, расширения и Content-Types](https://pwndizzle.blogspot.com/2015/07/xss-extensions-and-content-types.html)
* [Обход XSS-защиты Ebay для запуска XSS by...](https://whitehatnepal.tumblr.com/post/153333332112/xssonebay)
* [История о специфическом XSS для параметров!](https://www.noob.ninja/2017/09/story-of-parameter-specific-xss.html)
* [Cloudflare WAF XSS - Abdullah Hussam](https://ahussam.me/Cloudflare-xss/)
* [XSS to RCE in ...](https://matatall.com/xss/rce/bugbounty/2015/09/08/xss-to-rce.html)
* [One Payload to XSS Them All! ](https://ahussam.me/One-payload-to-xss-them/)
* [Uber Bug Bounty: превращаем Self-XSS в Good-XSS - Джек](https://whitton.io/articles/uber-turning-self-xss-into-good-xss/)
* [Мой "public Evernote": Turning Self-XSS into Good XSS v2: Challenge Completed but Not Rewarded](https://httpsonly.blogspot.com/2016/08/turning-self-xss-into-good-xss-v2.html)
* [How I XSS'ed Uber and Bypassed CSP - Efkan - Medium](https://medium.com/@efkan162/how-i-xssed-uber-and-bypassed-csp-9ae52404f4c5)
* [Запись обхода XSS "403 запрещено" - Nur A Alam Dipu - Medium](https://medium.com/@nuraalamdipu/xss-403-forbidden-bypass-write-up-e070de52bc06)
* [Подмена содержимого Medium приводит к XSS](https://ahussam.me/Medium-content-spoofing-xss/)
* [Reflected Client XSS at Amazon.com - Jonathan Bouman - Medium](https://medium.com/@jonathanbouman/reflected-client-xss-amazon-com-7b0d3cec787)
* [Airbnb - когда обход JSON-кодировки, XSS-фильтра, WAF, CSP и auditor превращается в восемь уязвимостей](https://buer.haus/2017/03/08/airbnb-when-bypassing-json-encoding-xss-filter-waf-csp-and-auditor-turns-into-eight-vulnerabilities/)
* [CSP: обход действия формы с помощью отраженного XSS](https://labs.detectify.com/2016/04/04/csp-bypassing-form-action-with-reflected-xss/)
* [Взлом XSS-mitigations с помощью Script Gadgets](https://www.blackhat.com/docs/us-17/thursday/us-17-Lekies-Dont-Trust-The-DOM-Bypassing-XSS-Mitigations-Via-Script-Gadgets.pdf)
* [sirdarckcat: 🤷 Unpatched (0day) jQuery Mobile XSS](https://sirdarckcat.blogspot.com/2017/02/unpatched-0day-jquery-mobile-xss.html)
* ['>">123\: [dev.twitter.com] XSS](https://blog.blackfan.ru/2017/09/devtwittercom-xss.html)
* [[BBP系列二] Uber XSS via Cookie | zhchbin](https://zhchbin.github.io/2017/08/30/Uber-XSS-via-Cookie/)



### **Stored XSS**

* [MB blog: Another XSS in Google Colaboratory](https://blog.bentkowski.info/2018/09/another-xss-in-google-colaboratory.html?view=sidebar)
* [Persistent XSS to Steal Passwords - Paypal ](https://wesecureapp.com/blog/persistent-xss-to-steal-passwords-paypal/)
* [Как мы захватили аккаунты shopify одним кликом | WeSecureApp | Research & Blog](https://wesecureapp.com/blog/how-we-tookover-shopify-accounts-with-one-single-click/)
* [Превращение Self-XSS в Non-Self Stored-XSS через проблему авторизации в "PayPal Tech-Support and Brand...](https://medium.com/@YoKoKho/turning-self-xss-into-non-self-stored-xss-via-authorization-issue-at-paypal-tech-support-and-brand-3046f52ac16b)
* [Persistent XSS is Not Self-XSS ](https://buer.haus/2016/06/21/persistent-xss-is-not-self-xss/)
* [Account Recovery XSS - Bughunter University](https://sites.google.com/site/bughunteruniversity/best-reports/account-recovery-xss)
* [#152067 Stored XSS на developer.uber.com через компрометацию учетной записи администратора](https://hackerone.com/reports/152067)
* [Klikki Oy - Yahoo Mail stored XSS](https://klikki.fi/adv/yahoo.html)
* [Klikki Oy - Yahoo Mail stored XSS #2](https://klikki.fi/adv/yahoo2.html)
* [AirBnb Bug Bounty: Turning Self-XSS into Good-XSS #2 | Geekboy | Security Researcher](http://www.geekboy.ninja/blog/airbnb-bug-bounty-turning-self-xss-into-good-xss-2/)
* [Как я нашел XSS Google Maps за $5000 (возившись с Protobuf) - Medium](https://medium.com/@marin_m/how-i-found-a-5-000-google-maps-xss-by-fiddling-with-protobuf-963ee0d9caff)

### **DOM Based XSS**

* [Обзор DOM XSS](https://ancat.github.io/web/xss/2012/05/26/an-overview-of-dom-xss.html)
* [DOM Based XSS - OWASP](https://www.owasp.org/index.php/DOM_Based_XSS)
* [Тестирование на DOM-based Cross site scripting (OTG-CLIENT-001) - OWASP](https://www.owasp.org/index.php/Testing_for_DOM-based_Cross_site_scripting_(OTG-CLIENT-001))
* [Комбинация методов приводит к DOM Based XSS в Google](https://sasi2103.blogspot.com/2016/09/combination-of-techniques-lead-to-dom.html)
* [DOM XSS Wiki](https://github.com/wisec/domxsswiki/wiki)
* [DOM XSS - auth.uber.com ](https://stamone-bug-bounty.blogspot.com/2017/10/dom-xss-auth14.html)
* [Minded Security Blog: DOM XSS в библиотеке Google VRView](https://blog.mindedsecurity.com/2018/04/dom-based-cross-site-scripting-in.html)
* [#231053 XSS на любом магазине Shopify через злоупотребление структурированным алгоритмом клонирования HTML5 в слушателе postMessage на "/:id/digital_wallets/dialog"](https://hackerone.com/reports/231053)
* [#262230 Tinymce 2.4.0](https://hackerone.com/reports/262230)

### **Blind XSS**

* [Poisoning the Well - Compromising GoDaddy Customer Support With Blind XSS | The Hacker Blog](https://thehackerblog.com/poisoning-the-well-compromising-godaddy-customer-support-with-blind-xss/index.html)

### **Cheatsheet/Payloads**

* [Browser's XSS Filter Bypass Cheat Sheet - masatokinugawa/filterbypass Wiki](https://github.com/masatokinugawa/filterbypass/wiki/Browser's-XSS-Filter-Bypass-Cheat-Sheet)
* [cure53/H5SC: HTML5 Security Cheatsheet - коллекция векторов XSS-атак, связанных с HTML5](https://github.com/cure53/H5SC)
* [Коллекция полезных нагрузок XSS в getto ](https://d3adend.org/xss/ghettoBypass)
* [cujanovic/Markdown-XSS-Payloads: XSS полезные нагрузки для эксплуатации синтаксиса Markdown](https://github.com/cujanovic/Markdown-XSS-Payloads)
* [PayloadsAllTheThings/XSS-инъекция в master - swisskyrepo/PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/XSS%20injection)

### **Tools**

* [evilcos/xssor2: XSS'OR - взлом с помощью JavaScript](https://github.com/evilcos/xssor2)
* [DanMcInerney/xsscrapy: XSS spider - обнаружено 66/66 wavsep XSS](https://github.com/DanMcInerney/xsscrapy)
* [nVisium/xssValidator: Это расширитель Burp, предназначенный для автоматизации и проверки XSS-уязвимостей](https://github.com/nVisium/xssValidator)
* [mandatoryprogrammer/xssless: Автоматизированный генератор XSS-payloads, написанный на python.](https://github.com/mandatoryprogrammer/xssless)
* [stamparm/DSXS: Damn Small XSS Scanner](https://github.com/stamparm/DSXS)
* [JSFuck](http://www.jsfuck.com/)
* [XSS Hunter - лучший способ борьбы с межсайтовым скриптингом](https://xsshunter.com/)
* [Unicode Converter](https://www.branah.com/unicode-converter)

## **Content Security Policy(CSP)**

* [Content Security Policy (CSP) - HTTP | MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP)
* [Content Security Policy Cheat Sheet - OWASP](https://www.owasp.org/index.php/Content_Security_Policy_Cheat_Sheet)
* [Блог h3xStream: Аудит заголовков CSP с помощью Burp и ZAP](https://blog.h3xstream.com/2016/06/auditing-csp-headers-with-burp-and-zap.html)
* [[CSP] Об отчетности и фильтрации | Dropbox Tech Blog](https://blogs.dropbox.com/tech/2015/09/on-csp-reporting-and-filtering/)
* [Как использовать Google CSP Evaluator для обхода CSP - блог Томаса Орлиты](https://blog.thomasorlita.cz/vulns/google-csp-evaluator/)
* [Обход CSP с помощью JPEG-polyglots | Блог](https://portswigger.net/blog/bypassing-csp-using-polyglot-jpegs)
* [Chrome XSS Auditor - SVG Bypass - Brute XSS](https://brutelogic.com.br/blog/chrome-xss-auditor-svg-bypass/)
* [Аккуратный обход CSP](https://lab.wallarm.com/how-to-trick-csp-in-letting-you-run-whatever-you-want-73cb5ff428aa)
* [A Novel CSP Bypass Using data: URI](https://www.nccgroup.trust/us/about-us/newsroom-and-events/blog/2019/april/a-novel-csp-bypass-using-data-uri/)

### **Burp Extensions**

* [PortSwigger/csp-auditor: плагин Burp и ZAP для анализа заголовков CSP](https://github.com/portswigger/csp-auditor)
* [PortSwigger/csp-bypass: Плагин Burp для обнаружения слабых мест в CSP](https://github.com/portswigger/csp-bypass)

## **Regular Expression**

* [attackercan/regexp-security-cheatsheet](https://github.com/attackercan/regexp-security-cheatsheet)
* [RegexOne - Сайт, для изучения регулярных выражений ](https://regexone.com/)
* [ReDoS Checker](https://devina.io/redos-checker)
* [Recheck](https://makenowjust-labs.github.io/recheck/playground/)

## **Cross Site Request Forgery**

* [Cross-Site Request Forgery (CSRF) - OWASP](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF))
* [Тестирование на CSRF (OTG-SESS-005) - OWASP](https://www.owasp.org/index.php/Testing_for_CSRF_(OTG-SESS-005))
* [Как я в очередной раз обошел CSRF в Facebook! | Dynamic World](https://blog.darabi.me/2016/05/how-i-bypassed-facebook-csrf-in-2016.html)
* [Получение токенов входа для учетной записи Outlook, Office или Azure - Jack](https://whitton.io/articles/obtaining-tokens-outlook-office-azure-account/)
* [Messenger.com Site-Wide CSRF - Jack](https://whitton.io/articles/messenger-site-wide-csrf/)
* [Кража токенов доступа Facebook с помощью CSRF в потоке входа на устройство - Josip Franjković](https://www.josipfranjkovic.com/blog/hacking-facebook-csrf-device-login-flow)
* [[PayPal BBP] Я мог удалить все SMC-сообщения. Используя bruteforce.](https://blog.ayoubaitelmokhtar.com/2018/06/paypal-bbp-i-couldve-deleted-all-smc.html)
* [Facebook GraphQL CSRF - Это не те access_tokens, которые вы ищете](https://philippeharewood.com/facebook-graphql-csrf/)
* [#44146 Выполнение вызовова API от имени другого пользователя (обход защиты CSRF)](https://hackerone.com/reports/44146)
* [Paypal bug bounty: Обновление картинки профиля Paypal.me без согласия пользователя (CSRF-атака)](https://hethical.io/paypal-bug-bounty-updating-the-paypal-me-profile-picture-without-consent-csrf-attack/)
* [Как я обнаружил ошибку Remote Code Execution, затрагивающую серверы Facebook](https://www.ubercomp.com/posts/2014-01-16_facebook_remote_code_execution)

### **JSON CSRF**

* [#245346 JSON CSRF на POST Heartbeats API](https://hackerone.com/reports/245346)
* [Эксплуатация JSON Cross Site Request Forgery (CSRF) с помощью Flash ](http://www.geekboy.ninja/blog/exploiting-json-cross-site-request-forgery-csrf-using-flash/)
* [Ubiquiti Bug Bounty: UniFi v3.2.10 Generic CSRF Protection Bypass - RCE Security](https://www.rcesecurity.com/2016/02/ubiquiti-bug-bounty-unifi-v3-2-10-generic-csrf-protection-bypass/)

### **Tools**

* [SWF-based JSON CSRF exploitation Tool](https://github.com/sp1d3r/swf_json_csrf)
* [appsecco/json-flash-csrf-poc: Этот репозиторий содержит файлы, необходимые для проведения CSRF-атаки с использованием Flash и перенаправления HTTP 307](https://github.com/appsecco/json-flash-csrf-poc)

## **Angular JS**
* [Philippe De Ryck on Twitter: "Как OWASP top 10 влияет на приложения #Angular? Эта #шпаргалка по безопасности охватывает набор лучших практик для 5 наиболее актуальных проблем для @Angular-приложений"](https://twitter.com/PhilippeDeRyck/status/1042360699572379648)
* [Angular - Top 10 Security Best Practices vis-a-vis Security Risks - Reskilling IT](https://vitalflux.com/angular-top-10-security-best-practices-vis-vis-security-risks/)
* [XSS без HTML: Client-Side Template Injection with AngularJS | Blog](https://portswigger.net/blog/xss-without-html-client-side-template-injection-with-angularjs)
* [DOM-based AngularJS sandbox escapes | Blog](https://portswigger.net/blog/dom-based-angularjs-sandbox-escapes)
* [Angular JS Security Videos](https://www.youtube.com/playlist?list=PLhixgUqwRTjwJTIkNopKuGLk3Pm9Ri1sF)
* [XSS без HTML: инъекция в шаблоны со стороны клиента с помощью AngularJS | Блог](https://portswigger.net/blog/xss-without-html-client-side-template-injection-with-angularjs)

## **React JS**

* [XSS через spoofed элемент React](http://danlec.com/blog/xss-via-a-spoofed-react-element)

## **postMessage vulnerabilities**

### Базовый материал для изучения

* [Exfiltration using postMessage](https://ancat.github.io/web/xss/2012/06/13/exfiltration-using-postmessage.html)
* [HTML5 Security: Cross Domain Messaging](https://resources.infosecinstitute.com/html5-security-cross-domain-messaging/#gref)
* [Security Risks Arise From Insecure Implementations of HTML5 postMessage() API | McAfee Blogs](https://securingtomorrow.mcafee.com/technical-how-to/security-risks-arise-insecure-implementations-html5-postmessageapi/)
* [Security Risks Arise From Insecure Implementations of HTML5 postMessage() API | McAfee Blogs](https://securingtomorrow.mcafee.com/technical-how-to/security-risks-arise-insecure-implementations-html5-postmessageapi/)
* [postmessage-asiaccs16.pdf](http://csis.gmu.edu/ksun/publications/postmessage-asiaccs16.pdf)
* [Контрольный список проверки безопасности postMessage()](https://gist.github.com/jedp/3005816)
* [HTML5 Security Part 2/3 - postMessage Vulnerabilities - YouTube](https://www.youtube.com/watch?v=XTKqQ9mhcgM)
* [Охота на уязвимости postMessage](https://www.sec-1.com/blog/wp-content/uploads/2016/08/Hunting-postMessage-Vulnerabilities.pdf)

### **Прохождения лабораторных**

* [Cross-Origin Message Vulnerability on xbox.com | James Slater](http://james.slaterspage.com/cross-origin-message-vulnerability-on-xbox-com/)
* [Автозаполнение LinkedIn раскрывает имя посетителя, его электронную почту сторонним сайтам | Lightning Security](https://lightningsecurity.io/blog/linkedin/)
* [Тайна postMessage - Рон Чан](https://ngailong.wordpress.com/2018/02/13/the-mystery-of-postmessage/)
* [The pitfalls of postMessage](https://labs.detectify.com/2016/12/08/the-pitfalls-of-postmessage/)
* [PostMessage XSS на миллионе сайтов](https://labs.detectify.com/2016/12/15/postmessage-xss-on-a-million-sites/)
* [#207042 Кража данных контактной формы на www.hackerone.com с помощью Marketo Forms XSS с использованием postMessage frame-jumping и jQuery-JSONP](https://hackerone.com/reports/207042)
* [#217745 XSS в $shop$.myshopify.com/admin/ через "Button objects" во вредоносном приложении](https://hackerone.com/reports/217745)
* [Read&Write Chrome Extension Same Origin Policy (SOP) Bypass Vulnerability | The Hacker Blog](https://thehackerblog.com/reading-your-emails-with-a-readwrite-chrome-extension-same-origin-policy-bypass-8-million-users-affected/index.html)
* [#231053 XSS в любом магазине Shopify через злоупотребление структурированным алгоритмом клонирования HTML5 в postMessage listener на "/:id/digital_wallets/dialog"](https://hackerone.com/reports/231053)
* [Взлом Slack с помощью postMessage и WebSocket-reconnect для кражи вашего драгоценного токена](https://labs.detectify.com/2017/02/28/hacking-slack-using-postmessage-and-websocket-reconnect-to-steal-your-precious-token/)

## **Flash Security**

### **Базовый материал для обучения**

* [Adobe ActionScript® 3 (AS3) API Reference](https://help.adobe.com/en_US/FlashPlatform/reference/actionscript/3/)
* [senocular.com - Security Domains, Application Domains, and More in ActionScript 3.0](http://www.senocular.com/flash/tutorials/contentdomains/)
* [Тестирование на xss (OTG-CLIENT-008) - OWASP](https://www.owasp.org/index.php/Testing_for_Cross_site_flashing_(OTG-CLIENT-008))

### **Writeups**

* [WordPress Flash XSS в flashmediaelement.swf](https://gist.github.com/cure53/df34ea68c26441f3ae98f821ba1feb9c)
* [XSS и CSRF через SWF-апплеты (SWFUpload, Plupload) " Neal Poole](https://nealpoole.com/blog/2012/05/xss-and-csrf-via-swf-applets-swfupload-plupload/)
* [Advanced Flash Vulnerabilities in Youtube - Part 1 | OpnSec](https://opnsec.com/2017/08/advanced-flash-vulnerabilities-in-youtube/)
* [Advanced Flash Vulnerabilities in Youtube - Part 2 | OpnSec](https://opnsec.com/2017/08/advanced-flash-vulnerabilities-in-youtube-part-2/)
* [Расширенные Flash-уязвимости в Youtube - часть 3 | OpnSec](https://opnsec.com/2017/08/advanced-flash-vulnerabilities-in-youtube-part-3/)
* [Расширенные Flash-уязвимости в Youtube - часть 4 | OpnSec](https://opnsec.com/2017/09/advanced-flash-vulnerabilities-in-youtube-part-4/)
* [#176308 Wordpress.com REST API oauth bypass via Cross Site Flashing](https://hackerone.com/reports/176308)
* [#164916 Обход политики одинакового происхождения на e.mail.ru с помощью межсайтовой прошивки](https://hackerone.com/reports/164916)
* [#182160 XSS в IE11 на portswigger.net через Flash](https://hackerone.com/reports/182160)

### **Tools**

* [cure53/Flashbang: Проект "Flashbang" - помощник по Flash-безопасности с открытым исходным кодом](https://github.com/cure53/Flashbang)

## **Dangling Markup**

* [Обход CSP с помощью DOM-based dangling markup | Blog](https://portswigger.net/blog/evading-csp-with-dom-based-dangling-markup)
* [CSP 2015](https://blog.innerht.ml/csp-2015/)
* [#87040 XSS на конечной точке авторизации/аутентификации OAuth](https://hackerone.com/reports/87040)
* [#199779 Google Analytics может быть использован как обход CSP для утечки данных на hackerone.com](https://hackerone.com/reports/199779)
* [GitHub's post-CSP journey | GitHub Engineering](https://githubengineering.com/githubs-post-csp-journey/)
* [AppSec EU 2017 So We Broke All CSPs You Won't Guess What Happened Next by Michele Spagnuolo - YouTube](https://www.youtube.com/watch?v=YBBqtrJmMRc)



## **JSON Hijacking**

* [JSON Hijacking](http://www.ninoishere.com/json-hijacking/)
* [Web Security Geeks - The Security Blog: JSON Hijacking](http://www.websecgeeks.com/2016/04/json-hijacking.html)
* [JSON hijacking for the modern web | Blog](https://portswigger.net/blog/json-hijacking-for-the-modern-web)
* [JSON hijacking](https://www.owasp.org/images/6/6a/OWASPLondon20161124_JSON_Hijacking_Gareth_Heyes.pdf)
* [AJAX Security Cheat Sheet - OWASP](https://www.owasp.org/index.php/AJAX_Security_Cheat_Sheet)


## **Web Sockets**

* [Cross-Site WebSocket Hijacking (CSWSH)](https://www.christian-schneider.net/CrossSiteWebSocketHijacking.html)
* [Тестирование WebSockets (OTG-CLIENT-010) - OWASP](https://www.owasp.org/index.php/Testing_WebSockets_(OTG-CLIENT-010))

### **Tools**

* [nccgroup/wssip: Приложение для захвата, модификации и отправки пользовательских данных WebSocket с клиента на сервер и наоборот](https://github.com/nccgroup/wssip)

## **Relative Path Overwrite**

* [Обнаружение и эксплуатация уязвимостей в импорте таблиц стилей с относительным путем (PRSSI) | Блог](https://portswigger.net/blog/detecting-and-exploiting-path-relative-stylesheet-import-prssi-vulnerabilities)
* [RPO](http://www.thespanner.co.uk/2014/03/21/rpo/)
* [Несколько методов эксплуатации RPO](https://www.mbsd.jp/Whitepaper/rpo.pdf)
* [RPO в Google Fusion Table](https://blog.innerht.ml/internet-explorer-has-a-url-problem/#rpoingooglefusiontable)

## **CSS Injection**

* [Testing for CSS Injection (OTG-CLIENT-005) - OWASP](https://www.owasp.org/index.php/Testing_for_CSS_Injection_(OTG-CLIENT-005))
* [Yahoo Login Protection Seal - Stored CSS Injection | Brett Buerhaus](https://buer.haus/2016/04/18/yahoo-login-protection-seal-stored-css-injection/)
* [Exfiltration via CSS Injection - d0nut - Medium](https://medium.com/@d0nut/exfiltration-via-css-injection-4e999f63097d)
* [dxa4481/cssInjection: Кража CSRF-токенов с помощью CSS-инъекции (без iFrames)](https://github.com/dxa4481/cssInjection)

## **ClickJacking**

* [Clickjackings in several Google Products](https://medium.com/@raushanraj_65039/google-clickjacking-6a04132b918a)
* [Кликджекинг на Google MyAccount стоимостью 7 500$ - Apapedulimu](https://apapedulimu.click/clickjacking-on-google-myaccount-worth-7500/)

## **CORS Vulnerabilities**

* [Test Cross Origin Resource Sharing (OTG-CLIENT-007) - OWASP](https://www.owasp.org/index.php/Test_Cross_Origin_Resource_Sharing_(OTG-CLIENT-007) )
* [Руководство по CORS (Cross-Origin Resource Sharing) для REST API | Moesif's Musings on Software](https://www.moesif.com/blog/technical/cors/Authoritative-Guide-to-CORS-Cross-Origin-Resource-Sharing-for-REST-APIs/)
* [Критическая проблема открыла приватные чаты пользователей Facebook Messenger для злоумышленников - Cynet](https://www.cynet.com/blog-facebook-originull/)
* [The Complete Guide to CORS (In)Security](https://www.bedefended.com/papers/cors-security-guide)

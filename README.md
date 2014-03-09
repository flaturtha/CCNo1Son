README.md

# Tales of Murder 
## [Prelaunch] - CharlieChan, v.00.1 (pre-alpha) ... repo name changed to facilitate new CharlieChan repo [3/9/14]

The CharlieChan repo on the TalesofMurder.com site is a static rendition to sort out grid, layout and structure. Once complete and operational (javascript, form, etc.), it will be cut up into Jekyll and renamed MilesArcher (replacing the current MilesArcher repo).

* mobile-first
* device-agnostic

### Site Structure Outline
```
1.  body: full width
1.1.  divs for scroll/fade background image

2.  header: full width = 100% of browser window
2.1.  header-wrap: max-width=60rem (desktop); max-width=100% (mobile)
2.1.1.  masthead: full-width (of parent) on mobile; 66% & float:left on desktop
2.1.2.  openingstar: display:none on mobile; 33% & float:right on desktop

3.  lede: @extend header
3.1.  lede-wrap: @extend header-wrap
3.1.1.  3x <p> teaser

4.  query: @extend header + full browser width red bar
4.1.  query-wrap: @extend header-wrap
4.1.1.  Qquery
4.1.2.  ul>li*3 questions

5.  content: @extend header
5.1.  main: @extend header-wrap [100% of ‘’-wrap for no sidebar; GR-large with sidebar…float:left on desktop]
5.1.1.  setup: max-width=[max appropriate measure for screen size]
5.1.2.  info: @extend header-wrap (full site width)
5.1.2.1.  info-box1: 33% of info
5.1.2.2.  info-box2: 33% of info
5.1.2.3.  info-box3: 33% of info
5.1.3.  takedown: @extend setup
5.2.  aside: @extend main [GR-small…float:right on desktop; below main on mobile]
5.2.1.  email-form: Sinatra app

6.  footer: @extend header
6.1.  footer-wrap: @extend header-wrap
```

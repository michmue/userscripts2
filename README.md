# project for modifying webpages to my liking:

## usage
install the userscript addon firemonkey (not tested: violentmonkey, greasemonkey, tempermonkey)
```
npm install
npm run serve
```
Compiled scripts now available at dist/ and available for browser through the started webserver (dev.user.js script need webserver to fetch changes).

1. Copy paste the whole script e.g. ArbeitsagenturFilter.user.js to a new script in the browser addon.
2. Copy the 'userscript header' from ArbeitsagenturFilter.user.mts to the addon script at the top.
3. go to the job searching [Arbeitsagentur.de/jobsuce/suche](https://www.arbeitsagentur.de/jobsuche/suche?berufsfeld=IT-Netzwerktechnik,%20-Administration,%20-Organisation;IT-Systemanalyse,%20-Anwendungsberatung%20und%20-Vertrieb;Informatik;Softwareentwicklung%20und%20Programmierung&angebotsart=1&wo=w%C3%BCrzburg&umkreis=25&sort=entfernung&zeitarbeit=true&id=10000-1196870944-S9)




## some interessting project insight
- First scripts were developed inside the userscript addon's editor in plain javascript [commit to browse](https://github.com/michmue/userscripts2/tree/53ef8196953afe6a867bba32fc46d1244b2b5e5c)
- Second 'evolution' was to develop them in javascript inside an ide
- Third big modification was to switch to typescript for reusable modules which are common inside most scripts to reduce copy/paste for each individual userscript
- Fourth project modification was to create a dev.user.js script so we dont have to copy/pase the compiled script back to the addon while developing. So now while developing we only rely on the dev script inside the addon and if the compiled source script changed it will autoreload the webpage while switching 'focus' from ide to browser.
- Fifth was to add source mappings *.js.map to access typescript sources in the browser debugger

next goal: 
- automation to add header to compiled sources to reduce copy/paste

![grafik](https://github.com/michmue/userscripts2/assets/37136025/fca8f2e9-849e-415c-bd58-811b586ed720)

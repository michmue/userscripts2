# project for modifying webpages to my liking:

- first scripts were developed inside the userscript addon's editor in plain javascript [commit to browse](https://github.com/michmue/userscripts2/tree/53ef8196953afe6a867bba32fc46d1244b2b5e5c)
- second 'evolution' was to develop them in javascript inside an ide
- third big modification was to switch to typescript for reusable modules which are common inside most scripts to reduce copy/paste for each individual userscript
- fourth project modification was to create a dev.user.js script so we dont have to copy/pase the compiled script back to the addon while developing. So now while developing we only rely on the dev script inside the addon and if the compiled source script changed it will autoreload the webpage while switching 'focus' from ide to browser.
- fifth was to add source mappings *.js.map to access typescript sources in the browser debugger

![grafik](https://github.com/michmue/userscripts2/assets/37136025/fca8f2e9-849e-415c-bd58-811b586ed720)

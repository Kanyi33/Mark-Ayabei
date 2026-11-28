Mark Ayabei - static site (no build step)

Open index.html in a browser, or drag this whole folder onto Netlify / Vercel / any web host.

Files
  index.html      page shell
  css/styles.css  all styling
  js/data.js      ALL CONTENT: films, other work, special projects, video links
  js/app.js       navigation, pages, player
  media/          hero.jpg (Home banner, text removed - the name/titles are live text),
                  portrait.jpg (Biography), plus posters / mp4 files

Contact form (js/data.js)
  formAction:'' opens the visitor's email app. Paste a Formspree/Netlify form URL to send messages directly.

Videos (js/data.js)
  Vimeo:   vimeo:'123456789'  (unlisted: '123456789/abcdef1234')
           In Vimeo > video settings > Privacy, allow embedding on the site's domain.
           Vimeo embeds need the site to be on http(s) (a hosted URL or localhost), not a double-clicked file.
  Self-hosted mp4: src:'media/clench/trailer.mp4'
  Poster image:    poster:'media/clench/poster.jpg'
  Showreel: reelVimeo:'...' (plays muted on loop, no controls) or reel:'media/reel.mp4'

Menu: Home, Categories (Films, TV series, Documentaries), Special Projects, Biography, Contact. Routes use #home, #categories, #special-projects, #biography, #contact, #clench, #wakariru, #road-home.


Placeholders are hidden automatically: boxes without a video or poster simply do not render. Film synopses are not displayed. Add vimeo/src/poster in js/data.js and they appear.
Film tiles are 16:9: set tile:"media/name.jpg" per film in js/data.js (use a film still when available; otherwise a crop of the poster).
Other work items without video show as text rows; add a vimeoId (4th value) or thumbnail (6th) to make them clickable tiles.

ADDING LINKS: see the instructions given with this build (Vimeo ID in js/data.js: vimeo:'ID' for films, reelVimeo for the showreel, 4th value for Other work items).

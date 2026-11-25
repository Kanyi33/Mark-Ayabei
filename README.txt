Mark Ayabei - static site (no build step)

Open index.html in a browser, or drag this whole folder onto Netlify / Vercel / any web host.

Files
  index.html      page shell
  css/styles.css  all styling
  js/data.js      ALL CONTENT: films, other work, special projects, video links
  js/app.js       navigation, pages, player
  media/          hero.jpg (Home banner, text removed - the name/titles are live text),
                  portrait.jpg (Biography), plus posters / mp4 files

Videos (js/data.js)
  Vimeo:   vimeo:'123456789'  (unlisted: '123456789/abcdef1234')
           In Vimeo > video settings > Privacy, allow embedding on the site's domain.
           Vimeo embeds need the site to be on http(s) (a hosted URL or localhost), not a double-clicked file.
  Self-hosted mp4: src:'media/clench/trailer.mp4'
  Poster image:    poster:'media/clench/poster.jpg'
  Showreel: reelVimeo:'...' (plays muted on loop, no controls) or reel:'media/reel.mp4'

Menu: Home, Categories (Films, TV series, Documentaries), Special Projects, Biography, Contact. Routes use #home, #categories, #special-projects, #biography, #contact, #clench, #wakariru, #road-home.

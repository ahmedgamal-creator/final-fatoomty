# Birthday Website for Fatoooomty

## Add your photos
Put two photos inside the `images/` folder named exactly `photo1.jpg` and `photo2.jpg`. (Square-ish photos look best; they are cropped automatically.) Until then a pink placeholder shows.

## Edit text
Open `index.html` in any text editor (Notepad, VS Code).
- Letters: find `const L=[` and edit the text inside each pair of quotes.
- Photo captions: search for `<figure class="pol">` and change the `<p>`.
- Secret message: search for `A secret for you`.
- Colors: the `:root{...}` line at the top of the style.

## Test
Double-click `index.html`. Tap the opening screen to start the music.

## Publish (Netlify, free, easiest)
1. Go to app.netlify.com/drop and sign up for free.
2. Drag the whole `fatoomty` folder (not the ZIP) onto the page.
3. Wait a few seconds. You get a link like `something.netlify.app`. Open it on your phone and check everything.
4. Optional: Site settings > Change site name to something nicer.

## Publish (GitHub Pages)
1. Create a free GitHub account and a new public repository.
2. Upload the files (`index.html`, `images/`) to it.
3. Settings > Pages > Source: Deploy from branch > `main` > Save.
4. After about a minute your link appears on that page.

## QR code
1. Open your real, working link on your phone first.
2. Use a free generator (for example qr-code-generator.com or qrcode-monkey.com), paste the link, download as PNG or SVG.
3. Scan the printed code with an Android and an iPhone camera before giving it to her.

## New sections
- Jar notes: edit `const R=[` in index.html (add or change reasons; more are added right after it with R.push).
- Coupons: edit `const C=[` (title, description).

## Your own song
Put an MP3 in the `music` folder named exactly `song.mp3`. It plays instead of the built-in melody. Keep it under ~5 MB so the page loads fast on phones.

## Counter
The date is in `const T0=new Date(2026,3,20);` (year, month starting from 0, day). April = 3.

## Our Moments (photos and videos)
Put files in `media/` and list them in `const G=[` in index.html. Photos: `{src:'media/pic.jpg',cap:'Caption'}`. Videos: add `,v:1` and use .mp4. Keep videos under ~10 MB (compress them first). Add or delete lines freely.

## Quiz
Edit `const Q=[`: `q` is the question, `o` the 3 answers, `a` the number of the right answer (0 = first, 1 = second, 2 = third).

## Our Photos (many photos)
Put photos in the `photos/` folder named 1.jpg, 2.jpg, 3.jpg ... up to 40 (jpg, jpeg, png or webp). Missing numbers are skipped automatically. To allow more, change `const COUNT=40`. Captions are optional: add them inside `PC={3:'caption for photo 3'}`. Resize photos to about 1200 px wide (200-400 KB each) so the page stays fast on phones.

## Fonts
Headings use Playfair Display (see the Google Fonts link at the top and `font-family` in the style). To try another readable romantic font, e.g. Dancing Script, replace the name in the link and in the CSS.

## Nicknames constellation
Edit the names in `const NM=[` (keep 7). Song: `music/song.mp3`.

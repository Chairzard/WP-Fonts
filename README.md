# WP Fonts - The internet's largest compilation of (quality) free/open-source fonts for KOReader, with fixes and other additions!

**I'm making the bold claim that basically every free & open-source *serif* font on the internet that's worth using can be found here**. By "worth using", I mean the font has no glaring technical issues and supports enough basic Latin glyphs for 99% of books you'll read in English.

This project started off to address a shortcoming of KOReader's engine at the time: No ability to synthesize small-caps that lacked them. As a secondary focus, I'd make improvements to the fonts I was tinkering with at the same time. As KOReader now can synthesize small-caps, the focus of the repo has flipped a bit on its head. Now, the focus is on fonts that have had technical improvements made to them (kerning fixes, missing opentype features, etc). I am also leaving my vast catalog of catalog of fonts that were modified to have small-caps, as their included small-caps are generally superior to KOReader's small-caps for the following reasons:

- Their kerning when they follow uppercase letters is superior (example: The glyph V following by the small-cap A will be kerned a lot tighter in my version versus the native sythesized fonts, *if* the font creator kerned them)
- I don't like how the engine handles scaled down small-caps for monospaced fonts, as it breaks monospacing (note: this is an issue with *all* ereader apps due to the technical limitations of faking small-caps)
- The KOReader engine scales glyphs to 75% of their height. This is a pretty decent choice, given the engine can only choose one number to scale by, but this is an imperect solution for every font. Small-capitals should ideally be at least a font's x-height % tall (when compared with the regular X's height), plus ideally a little taller than that (10-20% taller is generally the ideal). If the x-height of a font is, say, 80%, the small-caps will look anemic. My fonts have their small-caps based on the X-height (+10-20%, as needed), rather than a flat percentage, so they tend to be sized more appropriately.

**Why download my fonts?**  

- Unlike jumping into a sea of free fonts on a site like Google Fonts, every font here is at least passable for use on an ereader.
- Every font here can be freely downloaded and modified.
- Monospaced fonts have been edited to enable the monospace flag in KOReader (allowing them to be set as your default monospace fonts).
- The small-caps added to the monospaced fonts won't break monospacing.
- Fonts that included small-caps in their regular and/or bold style, but not in their italic and/or bold italic style, had those small-caps copied to the italic files with full kerning support (minus support for some Capital letter/small-cap kerning pairs).
- The most famous free & open-source sans-serif and monospaced fonts can also be found here. However, because they start to feel same-y after a while, my collection there is less comprehensive.

When possible, my license of choice is the SIL Open Font License (I've included an FAQ about it in the main folder of the repo). However, fonts are usually (maybe always!; I can't remember) distributed under their original licensing terms. All downloads contain a copy of the font licenses.  

Note: These fonts have **not** generally had their line heights adjusted and are tested to work best with [KOReader](https://koreader.rocks/) or other apps where users can make line height adjustments on the fly. If you need fonts modified for ereaders which *cannot* make such adjustments, I recommend looking at Nico Verbruggen's excellent [Ebook Fonts repository](https://github.com/nicoverbruggen/ebook-fonts).  

*IMPORTANT NOTE: If you have an ereader with a 300+ PPI display, I **strongly** recommend turning off font hinting in KOReader for the best font rendering experince. Leaving it on can cause glyphs to distort in unusual ways! If you're on a lower PPI display, you might need the hinting, though.*

**Q: How do I install these?**  
**A:** See the user guide here: https://koreader.rocks/user_guide/#L2-fonts. In general, you can just download the latest releases and drag all the font folders into KOReader's fonts folder and be done with (tip: you can also download fonts individually by exploring the repo a bit). Be advised that the TeX Gyre fonts (and possibly some others) are distributed in their original .zip files to comply with their license terms, so you'll need to extract those first before you can use them, too.

**Q: Now that KOreader can do fake small-caps, what's the plan for this repo?**  
**A: Going forward, I will no longer be creating my own scaled-down small-caps for non-monospaced fonts.** It's no longer worth the time investment with a "good enough" solution in place. If a font is missing small-caps in certain styles but has true small-caps in others, I'm *potentially* still open to porting them over to styles that lack them, but the font will need to be a banger and not have kerning designed in one of the circles of Hell for me to make that time commitment. I will continue to modify fonts that have bugs or really bad kerning issues that I can fix.  

## Current list of modified fonts available:

*Note: Fonts without Bold/Italic/Bold Italic files are still usable in KOReader. Many fonts distributed here lack at least one style. KOReader will create an artificial bold effect and/or apply an oblique effect, respectively, for fonts missing these files.*

Here's a complete list of modified fonts in this repo, and the modifications that were made. If you see no note listed in the far-right column, the only change made to the font was my addition of scaled-down small-caps from the era before KOReader could do that itself. Fonts marked as having "true" small caps use small capitals with the correct stroke width designed by the font creator, taken from other style files for the font. Fonts marked with an X just use my scaled-down capital letters. If there's a caution symbol, they use a mix of both true small capitals and my scaled-down ones.

|Original font name|Edited font name|Font license|Bold?|Italics?|Bold Italics?|"True" small caps?|Notes|
|---|---|---|---|---|---|---|---|
|**Adelphe**|WP Affinity|Open Inclusif·ve Fonte Licence|✅|✅|✅|❌|This release is based on the Mar 18, 2024 Adelphe font files, as the latest version uses the more restrictive CUTE License.|
|**Afacad**|WP Dacafa|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Afacad was chosen rather than Afacad Flux due to its italic/bold italic styles.|
|**Agave**|WP Spikes|MIT License|❌|❌|❌|✅|Monospaced font. Small caps are taken from the "duck" glyphs in the base font. The bold style is omitted, as it is incomplete and very buggy.|
|**Agrave Pro**|WP Gravy Pro|SIL Open Font License (version 1.1)|✅|❌|❌|✅|Fixes incorrect non-breaking space kerning.|
|**Alegreya**|WP Fexofenadine|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Left/right bearings of the left/right single/double quotation marks have been increased (I found them too tight by default, sometimes causing them to intersect with other glyphs). I also increased the distance between the "f" glyph and the exclamation/question marks and right parenthesis.|
|**Aleo**|WP Leo|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Almendra**|WP Amygdala|SIL Open Font License (version 1.1)|✅|✅|✅|⚠️|Small cap glyphs in the regular style were taken from the "SC" font file. Small-caps in the other styles were generated from scaled down capital letters.|
|**Amarna**|WP Armada|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Amstelvar**|WP Amsterdam|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Small caps were created from the variable font by setting capital height and width to 70%. Ligatures and Oldstyle Figures have been enabled. Word spacing was reduced.|
|**Anaheim**|WP Ducks|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Anonymous Pro**|WP Four Chan|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Antykwa Toruńska**|WP Antique|The GUST Font License (GFL) (version 1)|✅|✅|✅|✅|Fixes incorrect non-breaking space width. No further modifications.|
|**Anvers**|WP Anvil|SIL Open Font License (version 1.1)|❌|✅|❌|❌||
|**Archivo**|WP Archivist|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Aref Ruqaa**|WP Agile Ruqaa|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Arabic characters have been removed.|
|**Asul**|WP Lusa|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Custom fi/fl ligatures have also been added.|
|**Atkinson Hyperlegible Mono**|WP Hyperlegible Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Atkinson Hyperlegible Next**|WP Hyperlegible|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Averia Libre**|WP Mean|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Averia Sans Libre**|WP Mean Sans|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Averia Serif Libre**|WP Mean Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Baskervville**|WP Stapleton|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs. This font uses the Medium weight files rather than the regular weighted ones for better e-ink performance.|
|**Besley**|WP Bestley|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Made substantial kerning improvements to the SMCP glyphs and made the question mark more sane.|
|**BIZ UDPMincho**|WP B Mincho|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Japanese characters have been removed.|
|**Bona Nova**|WP Bona|SIL Open Font License (version 1.1)|✅|✅|❌|✅|Fixes a bug in the base italic file; no further changes.|
|**Caladea**|WP Calamari|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Cascadia Mono**|WP Dishwasher|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Cause**|WP Just|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Cohaerentia**|WP Coherent|SIL Open Font License (version 1.1)|❌|✅|❌|✅|Small caps merged from the standalone .sc file and copied into the Regular file. The same was done for the Italic file, with a reduced font weight and a little tweaking.|
|**Comic Relief**|WP Class Clown|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Comic Shanns**|WP Funny Shanns|MIT License|❌|❌|❌|❌|Monospaced font.|
|**Commit Mono**|WP Committed|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Cochineal**|WP Red Dye|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Fixes a glyph bug.|
|**Courier Prime**|WP Prime Time|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font. Ligatures have been disabled.|
|**Crete Round**|WP Cretan|SIL Open Font License (version 1.1)|❌|✅|❌|❌||
|**Crimson Pro**|WP Seeing Red|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Crimson Text**|WP Red Text|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Small-cap glyphs are copied from the roman styles. Kerning is copied from Cochineal, with some minor adjustments.|
|**Cuomotype**|WP Andrewtype|SIL Open Font License (version 1.1)|❌|❌|❌|❌||
|**Cutive Mono**|WP Executive Premier|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Monospaced font.|
|**DejaVu Sans Mono**|WP DR Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**DejaVu Serif**|WP DR Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**DM Mono**|WP Dredge|SIL Open Font License (version 1.1)|❌|✅|❌|❌|Monospaced font.|
|**Domine**|WP Dopamine|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**DP Sans Mono**|WP Proofreader|Other (see included license)|❌|❌|❌|❌|Monospaced font.|
|**Drafting Mono**|WP Drafting|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Monospaced font. Modified to enable the monospace flag in KOReader.|
|**DSE Typewriter**|WP DSE|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Monospaced font.|
|**EB Garamond**|WP Garamond|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Combines the small caps kerning used in Garamontio with Octavio Pardo's EB Garamond font. Out of an abudance of caution, I've disabled petite caps (ebooks *almost* never use them, but I didn't fix those, so I don't want books to accidentally call them).|
|**Eczar**|WP Ick|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Electrum ADF**|WP Electric|GNU GENERAL PUBLIC LICENSE Version 2|✅|✅|✅|✅|Fixes metadata bugs and enables oldstyle figures.|
|**Enriqueta**|WP Silkscreen|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Epunda Slab**|WP Upunda Slab|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**ETbb**|WPbb|MIT License|✅|✅|✅|❌|Fixes an annoying kerning error with the "s h" pair. Note that while this font includes the small-caps the original font creator used, they are scaled-down capital letters (so I don't consider them true small-caps).|
|**Fantasque Sans Mono**|WP Fantastic|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Fanwood Text**|WP Biggest Fan|SIL Open Font License (version 1.1)|❌|✅|❌|✅|The regular style already contained true small caps; small caps were created for the italic style based on those glyphs.|
|**Faustina**|WP Wolfgang|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Fira Mono**|WP Fox Mono|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Monospaced font.|
|**Fluxisch Else**|WP Or Else|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Various errors with the font's glyphs (there's "debris" that intersects with other glyphs) have been corrected. I omitted the bold file; it's not bold enough.|
|**Formera**|WP Past|SIL Open Font License (version 1.1)|❌|❌|❌|❌||
|**Frank Ruhl Libre**|WP Frank Rules|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**FreeSerif**|WP FreerSerif|GNU GENERAL PUBLIC LICENSE Version 3|✅|✅|✅|✅|Copies small-cap kerning from the italic style to the bold italic style.|
|**Gelasio**|WP Sorberto|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Gensco**|WP Lucretia|SIL Open Font License (version 1.1)|❌|❌|❌|❌||
|**Geom**|WP Geometry|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Glacial Indifference**|WP Titanic|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Glegoo**|WP Igloo|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Go**|WP Collect $200|The 3-Clause BSD License|✅|✅|✅|❌|Small caps in the regular & italic styles are true small caps, merged from the "SC" font files. Small caps in the Bold/Bold Italic styles are scaled down letters.|
|**Go Mono**|WP Collect $200 Mono|The 3-Clause BSD License|✅|✅|✅|⚠️|Monospaced font.|
|**Google Sans Code**|WP Search Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Hack**|WP Hacked|MIT License/Bitstream Vera License|✅|✅|✅|❌|Monospaced font.|
|**Happy Times at the IKOB**|WP Happy|SIL Open Font License (version 1.1)|✅|✅|❌|❌||
|**Hunck**|WP Amazing Bulk|SIL Open Font License (version 1.1)|❌|❌|❌|✅|Small-caps were merged in from the SC font file. Ligatures have been enabled. Added missing kerning for small-cap characters with diacritics.|
|**Hundar**|WP Charles|SIL Open Font License (version 1.1)|❌|❌|❌|❌|An interesting font that's in development. For some reason, the version available on the project's Github repo page is missing small caps, but I was able to pull them and add them into the font from sample docs on the project's website. I also fixed the broken ligature table and reduced word spacing.|
|**Hyde**|WP Jekyll|SIL Open Font License (version 1.1)|✅|✅|❌|⚠️|Kerning for the existing small capital letters has been improved. Small caps in the italicized file have had an oblique effect added. Small caps in the bold style are scaled-down letters.|
|**IBM 3270**|WP 3270|Other (see included license)|❌|❌|❌|❌|Monospaced font.|
|**IBM Plex Mono**|WP Perplex Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**IBM Plex Serif**|WP Perplex Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Based on the "Text" font weight from the variable font, for better e-ink performance. Otherwise, this is unmodified; there are no custom small-caps in this one.|
|**IM FELL Double Pica**|WP Fell Double Pica|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL DW Pica**|WP Fell DW Pica|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL English**|WP Fell English|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL French Canon**|WP Fell French Canon|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL Great Primer**|WP Fell Great Primer|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**Inika**|WP Eureka|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Inria Serif**|WP Calcul|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Intel One Mono**|WP CPU Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**JetBrains Mono**|WP PlaneBrains|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Jost**|WP Jasper|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Judson**|WP Judder|SIL Open Font License (version 1.1)|✅|✅|❌|❌||
|**Jura**|WP Ticket|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Karma**|WP Korma|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**KazukiReiwa**|WP Kazuki|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Japanese characters were removed to reduce font size.|
|**Kay Pho Du**|WP Kaye|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Kelvinch**|WP Kelvin|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The base fonts supports petite capitals; I created a small-capital opentype table to enable them to work with small-caps and fixed an error that cause ligatures to override the table. The broken kerning tables were removed to allow the font to save. The font has also been hinted.|
|**Kreon**|WP Crayon|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Kode Mono**|WP Koder|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Monospaced font.|
|**KPRoman**|WP KP|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Fixes an error that cause italics to override the normal style; no further changes made|
|**Labrada**|WP Kadabra|SIL Open Font License (version 1.1)|✅|✅|✅|❌|A kerning fix to the lowercase b was also made.|
|**Laconic**|WP Few Words|SIL Open Font License (version 1.1)|✅|❌|❌|❌|This fixes an issue which causes ligatures to have priority over small-caps in the base font.|
|**Laila**|WP Dominos|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Non-Latin characters have been removed.|
|**Lekton**|WP Lecturn|SIL Open Font License (version 1.1)|✅|✅|❌|✅|Monospaced font. Small caps in the Italic style are pulled from the regular style. Kerning has been removed in the italic file (who kerns a monospaced font? 😂)|
|**Lexend**|WP Luthor|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**LXGW Neo ZhiSong Screen**|WP Sing Sing|IPA Font License (version 1.0)|❌|❌|❌|❌|Japanese characters were removed to reduce font size.|
|**Liberation Mono**|WP Libertino Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Liberation Sans**|WP Libertino Sans|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Liberation Serif**|WP Libertino Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Ligatures have been enabled, and a kerning error was fixed (note that the kerning error was left in by design to match the metrics of Times New Roman; my changes mean the font is no longer metrically-compatible with it).|
|**Libre Baskerville**|WP Mortimer|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Libre Caslon Text**|WP Caslon|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Linden Hill**|WP Hill House|SIL Open Font License (version 1.1)|❌|✅|❌|✅|The regular style already contained true small caps; small caps were created for the italic style based on those glyphs.|
|**Literata**|WP Illiterata|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Reduces the space between the "H e" kerning pair in the Regular and Bold styles (I tried to live with it, as Literata is perhaps my favorite font, but I couldn't help myself on this one; it was insufferably wide!)|
|**Lora**|WP Arol|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Lotion**|WP In the Basket|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**LT Superior Serif**|WP Superior|SIL Open Font License (version 1.1)|✅|❌|❌|✅|Fixes font metadata.|
|**M PLUS Code Latin**|WP M MINUS|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Monospaced font.|
|**Maitree**|WP My Tree|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Mali**|WP Bamako|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Features substantial kerning improvements over the base font.|
|**Manuale**|WP Manually|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Maple Mono NL**|WP Toronto|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font (no ligature variant).|
|**Mate**|WP Checkmate|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps. Small caps in the Italic style are scaled down letters.|
|**Merriweather**|WP Merry Weather|SIL Open Font License (version 1.1)|✅|✅|✅|✅|This fixes an issue which causes ligatures to have priority over small-caps in the base font.|
|**Monaspace Argon**|WP MS A|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Monaspace Krypton**|WP MS K|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Monaspace Neon**|WP MS N|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Monaspace Radon**|WP MS R|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Monaspace Xenon**|WP MS X|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Nepomuk**|WP Nepogrimer|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Italic/Bold italics generated using the regular/bold style glyphs.|
|**New Computer Modern**|WP New Computer Moderner|Regular style file: GPL3 or later plus Font Exception (FE) plus Distribution Exception (DE). All other files: The GUST Font License (GFL) (version 1)|✅|✅|✅|✅|Copied small-caps kerning from the regular/bold files into the italic/bold italic files. Also fixed an issue with the non-breaking space.|
|**New Computer Modern Mono**|WP New Computer Moderner Mono|The GUST Font License (GFL) (version 1)|✅|❌|❌|✅|Monospaced font. Fixed a missing italic style flag and edited the font to use KOReader's monospace flag.|
|**New Tegomin**|WP Cigarette Burns|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Non-latin characters have been removed.|
|**New Telegraph**|WP Newer Telegraph|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Enables ligatures.|
|**Newt Serif**|WP Salamander|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Nimbus Mono PS**|WP Postal|GNU AFFERO GENERAL PUBLIC LICENSE Version 3|✅|✅|✅|❌|Monospaced font.|
|**Nocturne Serif**|WP Nocturnal|SIL Open Font License (version 1.1)|❌|❌|❌|✅|Fixes issue where ligatures overrode small-caps. There's a commercial version available with more font styles; as far as I'm aware, only the regular style is available under the OFL.|
|**Noticia Text**|WP Notice|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**OCR-A**|WP OCR-A|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Custom glyphs have also been added.|
|**OCR-B**|WP OCR-B|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Custom glyphs have also been added.|
|**OpenDyslexic 2**|WP OD 2|Creative Commons Attribution 4.0 International license (CC BY 4.0)|✅|✅|✅|❌|Based off OpenDyslexic 2.x.|
|**OpenDyslexic 4**|WP OD 4|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Based off OpenDyslexic 4.x. Font left/right bearings have been greatly reduced. The double-story "a" has replaced the single-story a in the Regular/Bold styles (it has been made bolder in the bold style, too).|
|**Orbit**|WP Galaxy|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Monospaced font. Ligatures and Korean removed.|
|**Outfit**|WP Outfitted Classic|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Removes the "outfit" ligature.|
|**Overlock**|WP Overlocked|SIL Open Font License (version 1.1)|✅|✅|✅|⚠️|Small caps were enabled in the regular style. Scaled-down small cap glyphs were added to the other files. Ligatures were enabled across all files.|
|**Overpass**|WP Underpass|SIL Open Font License (version 1.1)|✅|✅|✅|❌|
|**Patrick Hand**|WP Star|SIL Open Font License (version 1.1)|❌|❌|❌|✅|Fixes the font's broken small-caps opentype table.|
|**Pixel Code**|WP PixelC|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced.|
|**Półtawski Nowy**|WP Poltergeist|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Fixes incorrect non-breaking space kerning. No further modifications.|
|**Poly**|WP Polybius|SIL Open Font License (version 1.1)|❌|✅|❌|✅|The regular style already contained true small caps; small caps were created for the italic style based on those glyphs.|
|**Poppins**|WP Mary|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Proggy**|WP Froggy|MIT License|❌|❌|❌|❌|Monospaced font.|
|**Proza Libre**|WP Prose|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Ligatures have been enabled.|
|**PT Serif**|WP Petey Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Radley**|WP Radical|SIL Open Font License (version 1.1)|❌|✅|❌|❌||
|**Roboto Mono**|WP Bot Mono|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Monospaced font. Corrected the SMCP table in the font and added a C2SC table.|
|**Roboto Serif**|WP Bot Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Rosarivo**|WP Rosebud|SIL Open Font License (version 1.1)|❌|✅|❌|❌||
|**Sawarabi Mincho**|WP Zenith|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Japanese characters have been removed.|
|**Science Gothic**|WP Science|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Uses font instances generated from the variable file. I've used the Light/Semibold files rather than Normal/Bold for better e-ink performance.|
|**Secuela**|WP Seiklus|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Fixes the font's broken smcp tables.|
|**Sedan**|WP Vroom|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps. Small caps in the Italic style are scaled down letters. Custom ligatures were added, and a major kerning fix was made.|
|**Selectric Mono**|WP Selective|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Monospaced font.|
|**Share Tech Mono**|WP Shared Tech Mono|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Monospaced.|
|**Shippori Mincho**|WP S Mincho|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Japanese characters have been removed.|
|**Sometype Mono**|WP Sum Type Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Source Code Pro**|WP SCode Pro|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Source Serif 4**|WP SSerif|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs.|
|**Space Mono**|WP Space Invaders|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Special Elite**|WP Elite|Apache License (version 2.0)|❌|❌|❌|❌||
|**Splentinex (Splentino)**|WP Splenda|SIL Open Font License (version 1.1)|✅|✅|✅|⚠️|Small-caps in the regular style are true small-caps. Small-caps in the italic style are copied from the regular style. Small-caps in the Bold/Bold Italic styles are scaled-down letters. A kerning issue with old-style figures in the regular style was also corrected.|
|**Stilu**|WP Style U|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Fixes many font metadata bugs which broke the font.|
|**Sudo**|WP RM RF|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**SUSE**|WP Geeko|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**SUSE Mono**|WP Geeko Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Tagesschrift**|WP One Day|SIL Open Font License (version 1.1)|❌|❌|❌|❌||
|**TeX Gyre Cursor**|WP Click|The GUST Font License (GFL) (version 1)|✅|✅|✅|✅|Ligatures are removed.|
|**TeX Gyre Termes**|WP New Times|The GUST Font License (GFL) (version 1)|✅|✅|✅|✅|Fixes various kerning issues and left/right bearing issues, especially with ligatures and the lowercase "v".|
|**Texturina**|WP Texture|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Tienne**|WP Yours|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Enabled ligatures.|
|**Typey McTypeface**|WP Face Off|SIL Open Font License (version 1.1)|❌|✅|❌|❌||
|**Ubuntu Mono**|Ubuntu Mono WP|UBUNTU FONT LICENCE|✅|✅|✅|❌|Monospaced font. The font is named differently than other fonts in this repo due to the font's license terms.|
|**Ubuntu Sans**|Ubuntu Sans WP|UBUNTU FONT LICENCE|✅|✅|✅|✅|The font is named differently than other fonts in this repo due to the font's license terms. Italic/Bold Italic small caps are oblique versions of the true small caps from the regular/bold styles.|
|**Vesper Libre**|WP Venus|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Devanagari characters have been removed.|
|**Vollkorn**|WP Korn|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs.|
|**Winky Sans**|WP Rip Van Winkle|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Kerning is lifted from the "Rough" font style (it's more robust than the base file's kerning).|
|**XCharter**|WPCharter|Bitstream Free font license|✅|✅|✅|✅|Deleted the buggy and uneven small-cap glyphs. Changed made the oldstyle `1` glyph the alternate, and vice-versa.|
|**Young Serif**|WP Younger Serif|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Fixes broken font metadata.|
|**Ysabeau**|WP Eezahboh|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Italic/Bold italics generated using the regular/bold style glyphs.|
|**Ysabeau Medium**|WP Eezahboh 2|SIL Open Font License (version 1.1)|✅|✅|✅|✅|A heavier cut of this great font, for those who prefer it.|
|**Ysabeau Semibold**|WP Eezahboh 3|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The heaviest cut of this great font, for those who prefer it.|
|**Yuji Syuku**|WP Wesker|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Changes to ellipsis and bearings of quotation marks have been made. Japanese glyphs were removed to reduce font size.|
|**Zen Old Mincho**|WP Old Mincho|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Japanese characters have been removed. While a bold file is included (based on the Black file), it's very subtle. You may want to consider using only the regular file and having KOReader fake the bold effect.|
|**Zilla Slab**|WP Fox Slab|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The right side bearing of the lowercase r has been improved. Edited the font's small-cap table to work with the lastest version of crengine.|
|**erewhon**|WP Nowhere|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Adds kerning that was missing for the Italic/Bold Italic small-caps.|
|**mononoki**|WP Doki Doki|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|

## Other FAQs:

**Q: Should I use these fonts outside of KOReader?**  
**A:** On any ereader that supports true small-capitals via opentype features (such as Pocketbook's stock reader and Kindle books with "enhanced typsetting"), you'll set the full set of benefits mentioned earlier. Other fonts have various fixes that enhance the reading experience, such as kerning and other bug fixes, that will apply to basically all ereaders except for Kobo's stock software (if you're on a repo like this, you shouldn't be using Kobo's dreadfully outdated and limited reader anyway, though; join the KOReader gang 😉).

**Q: Will you add Bookerly, Rakuten Serif, or (insert proprietary font here)?**  
**A:** Unfortunately, I cannot legally edit, redistribute, or encourage pirating these proprietary font files due to their restrictive font licenses. FYI, the latest version of Bookerly contained on the Kindle’s downloadable firmware *does* have true small-caps built in (the version hosted on the Amazon Developer site for developers is outdated and lacks them).

**Q: Can you add or update (insert non-proprietary font here)?**  
**A:** I'll add any free & open source font serif or sans-serif font you request (throw an issue into the github issues section). Doing bugfixes beyond that will be at my discretion. Monospaced fonts will also be at my discretion, as they often take a bit more work to make them play nice with KOReader.

**Q: Can you add the glyphs from (insert language here)?**  
**A:** To save time, these files were created and use only the glyph sets I expect to run across in the books I read (Latin and Greek). I currently do not have plans to re-do any of these fonts with other glyph sets. However, I’ve provided instructions on how to make your own fake small-caps below. Fonts added after the big update should have their entire glyph sets, unless they're monospaced (in which case, I may prune some unused languages from them).

**Q: Can you create variable versions of these fonts?**  
**A:** I use FontForge, which currently doesn’t support this. KOReader technically will support variable fonts in this upcoming update, but I've found that static files still play nicer with it, so I will continue adding the static files.

**Q: I found an issue unrelated to small caps with the font. Should I let you know?**  
**A:** Yes! I'm open to fixing glaring kerning errors and other smaller issues with these fonts, provided I can do so in a reasonable amount of time (I'm not re-kerning an entire font, for example). Open an issue in the Issues tracker, and I'll let you know if I can handle it.

**Q: Why were the font files renamed?**  
**A:** To avoid confusion with the original font files, as well as to allow the modified files to coexist with the originals. Additionally, fonts under the OFL often have reserved font names. To legally redistribute them, I had to change the font names.

**Q: How were the font names chosen?**  
**A:** I just used references or puns that came to mind, most of the time.

**Q: Why are the Italic/Bold/Bold Italic files missing?**  
**A:** Font styles will be missing when the original font lacks them (or, in very rare cases, because those style files have severe issues, such as *extremely* incomplete glyph sets). I try to favor fonts that include all four styles, but oftentimes I liked the base font enough to include it anyway and deal with KOReader applying a fake oblique and/or bold effect when needed. Your ereader/app will probably fake these effects if they’re missing (one important exception I know of is Kindle, which won’t properly render Bold Italic if you are missing the Bold Italic File but have regular Bold and Italic; in that case, delete/don’t use the Bold file at all).

**Q: (Insert font here from the collection) just released an updated version!**  
**A:** If you see a substantially updated font that's out of date here, feel free to open an issue and I'll make sure it's updated, *unless* it's one of the fonts I modified and the core reasons I modified it in the first place remain unaddressed.

## How to create your own fake small caps in FontForge (this is no longer recommended, in most cases!):

*NOTE: Fonts sometimes keep their kerning classes in their dist/mark tables; if you don't see kerning classes under "kern", look there*.  

If you’re looking to create your own fake small-capital glyphs, here are the steps I used in FontForge (current as of version 20251009). I **strongly** recommend saving frequently when doing this, as FontForge has a bad habit of crashing, especially in step 4.

1. Use Encoding → Compact to limit the view to glyphs only (filtering out empty slots; this makes things a lot easier).
2. Use Edit → Select → Select by script to select all Latin (code: latn) glyphs.
3. *OPTIONAL: Select any other glyph sets you might want (I also included Greek (code grek) glyphs, when available). Merge the results.*
4. Select Element → Style → Add Small-Capitals and hit the OK button. This will create encoding slots for the small-capital glyphs, as well as create some that will probably look pretty bad (we’ll replace them).
	- NOTE: FontForge loves to crash on this step, usually for one of two reasons:
		1. There’s a glyph that it doesn’t like in your glyph set. This rarely happens in Latin (you can find out which glyph is making it crash via trial and error), but it is super common in Greek with the capital letter Omega, as there are often 2 omegas in the font file (you’ll need to figure out which of the two is causing the crash via trial and error).
		1. Less commonly, in the “Add Small-Capitals” dialog box, an invalid number labeled “nan” may appear. If this happens, replace the number with any valid number.
5. Repeat steps 1-2, then copy the selected glyphs and paste them into the small-cap glyphs slots. Pay attention to where each glyph is pasted; you may need to remove certain selected glyphs from your initial selection (you can do this by holding shift and clicking the glyphs you want removed) if repeat/s appear and the glyphs don’t line up correctly with their encoding slots.
6. Select all small-cap glyph slots, then unlink their references in Edit → Unlink Reference (also available in the right-click menu). This will prevent weird kerning issues and enable the glyphs to scale down properly.
7. OPTIONAL but highly recommended if your font has kerning (most good fonts that aren’t monospaced do): Repeat steps 1-2, remove any duplicates you previously needed to remove, then use Edit → Copy → Copy Lookup Data on the selected glyphs.
	- Select all the small-cap glyphs and paste. Select all entries on the list that list “’kern’”. There will always be multiples of two (there’s a “second glyph” entry at the bottom of the list and a first entry somewhere above it).
8. Select all the small-cap glyphs. Select Element → Transformations → Transform (also available in the right-click menu). The origin should have “Glyph Origin” selected, and the box under that (which defaults to Move) should be changed to “Scale Uniformly”. This part is subjective. I would typically recommend scaling by your font’s x-height percentage. You can find the percentage to scale by in most fonts by going to Element → Font Info → OS/2 → Metrics, dividing the X Height by the Capital height, and multiplying that by 100 (if you’re super lazy and want something that looks OK but may not be the ideal, you can just scale by 80%). Some badly made fonts may not include this info; in those cases, go to Element → Style → Add Small-Capitals and look at the number listed in the Horizontal and Vertical tabs and use that instead. If the default number results in small-caps that are too small for your liking, increase the number by 10-20%. IMPORTANT: When scaling non-monospace fonts, make sure “Transform Width Too” and “Transform simple positioning pairs and kern pairs” are checked. If you’re scaling a monospace font, uncheck transform width too.
9. *MONOSPACE FONTS ONLY: Select all small-cap glyphs in the font, then select edit → Unlink reference.*
10. *MONOSPACE FONTS ONLY (Optional, but I think it looks better): With all small-cap glyphs still selected, Select Metrics → Center in width.*
11. Go to Element → Font info → Lookups. Under GSUB, we’ll need to edit two tables so that smallcap lookups happen correctly. Move smcp and c2sc to the top of your list, if they aren't there already (the order of those two doesn’t matter; those two just need to be above everything else). Hit the plus button for each, then click the entry that pops up, and finally click Edit Data. IN ORDER, do the following: Remove All, Populate, Remove empty. You’ll know you messed this step up if you see dots about your small-capital “I”s when you test out the font!
12. Right click any lookup table, and click "Add 'DFLT' script, then click "Apply to All". I do the same for the GPOS tables, too (though that may not be necessary).
13. *OPTIONAL: If you want proper kerning for the small-capital glyphs, you’re going to have to manually add it in. Step 7 copied over any kerning pairs your font may have had, but if your font also uses kerning tables (common, especially for newer fonts), the process is nightmarish. See instructions below. I’m not going to sugarcoat it; that can be a brutal process and takes way, way too long, so if you can live without proper kerning, skip this step. I couldn’t, so all fonts here are kerned.*
14. Go to file → Generate fonts and generate your fonts!  

⚠️Masochists only!⚠️ - Kerning your fonts that include kerning classes.  

1. PREREQUISITE: Keep unaltered copies of your fonts handy.
2. You'll need to manually add all your small-cap glyphs to the kerning classes that the glyphs they’re based on are in (for example, you’d add “a.sc” to the Kerning classes “A” is in). Save a copy of the new font file(s) with these additions.
3. Create 2 new files titled Left and Right.
4. Remove all glyphs from ALL kerning classes on the left or right side, besides the .sc glyphs (you should delete any tables that don't have .sc glyphs on the side you're working on). Save.
5. Repeat step 4, but in the other file/on the other side. Save.
6. Load the file from step 2. Delete all kerning classes.
7. Load the vanilla font from step one from within the same window (this enables imports).
8. Go to the kerning class tables (element → font info → lookups → GPOS) and import the kerning tables from the other font (delete any "per glyph" tables; they'll be blank. The same goes for the following steps. Give the table and classes unique numbers/names (or you may run into wonky behavior).
9. Arrange the kerning classes in the same order as they are in the base font. Save and quit FontForge (this prevents crashes).
10. Open the file you're working on. Within that window, open the "left" or "right" file.
11. Import the kerning classes from that file. Arrange the imported classes below the existing ones. Save and quit.
12. Open the file you're working on. Within that window, open the "left" or "right" file not used in step 10.
13. Import the kerning classes from that file. Arrange the imported classes below the existing ones. Merge them into the classes from step 11 (merge them in the same order; for example, you'd merge kerning class 4 from the right file into class 4 from the left).
14. Export the font.

**IMPORTANT NOTE:** I recommend saving in the file format that the original font files were in to avoid losing the font’s hinting data. For ttf files, generate the fonts in “TrueType” format. Make sure that within the Options box, you have the following settings checked:
- Hints
- Flex Hints
- TrueType Hints
- PS Glyph Names
- OpenType
- FFTM

Make **very** sure that “Apple”, “windows-compatible kern”, “old style kern”, and “prefer native kerning” are NOT checked. If the font was originally an OTF file, save it as an “OpenType (CFF)” file. In very rare cases, usually with very old fonts, you may need to enable old-style kerning.

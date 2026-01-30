# WP Fonts - Customized fonts with added small-caps for KOReader!

One of the only shortcomings of KOReader is that the engine it uses can’t create fake small-capital letters when a font lacks them and instead renders the text in lowercase (according to the developers, this is not a feature that is viable to add in due to how the engine functions). Some of my most beloved fonts don't have small-caps baked in, and losing the small cap formatting hurts my soul. However, the engine does support small-capitals for fonts that include them already. To take advantage of this and feed my unchecked font addiction, I’ve created (too many) fonts with custom small-capitals and created a GitHub repository to host them (they’re spartan and just scaled-down capital letters like a web browser/the Kobo stock reader would do, but they’ll do the trick in a pinch). With these fonts, you can go from this:  

<img width="509" height="84" alt="image" src="https://github.com/user-attachments/assets/1acbdf2e-d6bd-4cf9-95b8-69c8ad2cf6fb" />

To this:

<img width="509" height="84" alt="image" src="https://github.com/user-attachments/assets/81048731-b9e8-4376-9c31-1fddf4804d4b" />

The various fonts contained within this repository are licensed under different licenses. When possible, my license of choice is the the SIL Open Font License (I've included an FAQ about it in the main folder of the repo).

Kerning was also added for the fake small-caps, provided the original font had kerning for its uppercase letters. I just copied over the kerning from the uppercase letters. This generally means that words in small-caps will have the same appearance as words in all uppercase. However, in many cases this results in kerning that is a little too tight. This may be addressed in future updates.

## Current list of fonts available:

You may also be interested in my [list of of fonts with real small-caps](https://github.com/Chairzard/WP-Fonts/blob/main/Recommend%20fonts%20with%20real%20small-caps.md). In most cases, I will not be releasing modified versions of those, unless they are missing small caps in certain styles (or have really bad kerning issues that I can fix).  

A few of these fonts need kerning refinements (because of how they were created, a few ended up with kerning for the small caps that was a little too tight). These may be corrected in future updates, if I have time; fixing these fonts takes much longer than creating them. You can see the list of affected fonts (here)[https://github.com/Chairzard/WP-Fonts/blob/main/Kerning%20optimizations%20still%20needed.md]

Fonts without Bold/Italic files are still usable in KOReader. KOReader will create an artificial bold effect or apply an oblique effect, respectively, for fonts missing these files. Fonts marked as "true" small caps use small capitals with the correct stroke width, taken from other style files for the font (fonts marked with an X just use generic, scaled-down capital letters).

|Original font name|Edited font name|Font license|Bold?|Italics?|Bold Italics?|"True" small caps?|Notes|
|---|---|---|---|---|---|---|---|
|**Adelphe**|WP Affinity|Open Inclusif·ve Fonte Licence|✅|✅|✅|❌|This release is based on the Mar 18, 2024 Adelphe font files, as the latest version uses the more restrictive CUTE License.|
|**Afacad**|WP Dacafa|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Afacad was chosen rather than Afacad Flux due to its italic/bold italic styles.|
|**Agave**|WP Spikes|MIT License|✅|❌|❌|❌|Monospaced font.|
|**Aleo**|WP Leo|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Almendra**|WP Amygdala|SIL Open Font License (version 1.1)|✅|✅|✅|⚠️|Small cap glyphs in the regular style were partially taken from the "SC" font file; all other small cap glyphs in the regular style, as well as all glyphs in the other styles, were generated from scaled down capital letters.|
|**Amarna**|WP Armada|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Anaheim**|WP Ducks|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Anonymous Pro**|WP Four Chan|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Aref Ruqaa**|WP Agile Ruqaa|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Arabic characters have been removed.|
|**Archivo**|WP Archivist|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Asul**|WP Lusa|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Custom fi/fl ligatures have also been added.|
|**Atkinson Hyperlegible Mono**|WP Hyperlegible Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Atkinson Hyperlegible Next**|WP Hyperlegible|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Averia Libre**|WP Mean|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Averia Sans Libre**|WP Mean Sans|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Averia Serif Libre**|WP Mean Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Baskervville**|WP Stapleton|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs. This font uses the Medium weight files rather than the regular weighted ones for better e-ink performance.|
|**Besley**|WP Bestley|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Made substantial kerning improvements to the SMCP glyphs and made the question mark more sane.|
|**BIZ UDPMincho**|WP B Mincho|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Japanese characters have been removed.|
|**Brawler**|WP Super Smash|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Cabin**|WP In the Woods|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Caladea**|WP Calamari|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Cascadia Mono**|WP Dishwasher|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**Cause**|WP Just|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Courier Prime**|WP Prime Time|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font. Ligatures have been disabled.|
|**Crimson Pro**|WP Seeing Red|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Comic Neue**|WP Comic New|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Cooper Hewitt**|WP Coop|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Cuomotype**|WP Andrewtype|SIL Open Font License (version 1.1)|❌|❌|❌|❌||
|**DP Sans Mono**|WP Proofreader|Other (see included license)|❌|❌|❌|❌|Monospaced font.|
|**DejaVu Sans Mono**|WP DR Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospaced font.|
|**DejaVu Serif**|WP DR Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Eczar**|WP Ick|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Enriqueta**|WP Silkscreen|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Epunda Slab**|WP Upunda Slab|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Fanwood Text**|WP Biggest Fan|SIL Open Font License (version 1.1)|❌|✅|❌|✅|The regular style already contained true small caps; small caps were created for the italic style based on those glyphs.|
|**Faustina**|WP Wolfgang|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Finlandica**|WP Finland|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Formera**|WP Past|SIL Open Font License (version 1.1)|❌|❌|❌|❌||
|**Frank Ruhl Libre**|WP Frank Rules|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Gelasio**|WP Sorberto|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Gensco**|WP Lucretia|SIL Open Font License (version 1.1)|❌|❌|❌|❌||
|**Granstander**|WP Sophist|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Google Sans**|WP Search Sans|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Gupter**|WP Reptar|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Hack**|WP Hacked|MIT License/Bitstream Vera License|✅|✅|✅|❌|Monospaced font.|
|**Happy Times at the IKOB**|WP Happy|SIL Open Font License (version 1.1)|✅|✅|❌|❌||
|**Hyde**|WP Jekyll|SIL Open Font License (version 1.1)|✅|✅|❌|✅|Kerning for the existing small capital letters has been improved, small caps in the bold style have been made bolder, and small caps in the italicized file have had an oblique effect added. Hinting has also been added to the fonts.|
|**IBM 3270**|WP 3270|Other (see included license)|❌|❌|❌|❌|Monospaced font.|
|**Inika**|WP Eureka|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**IM FELL Double Pica**|WP Fell Double Pica|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL DW Pica**|WP Fell DW Pica|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL English**|WP Fell English|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL French Canon**|WP Fell French Canon|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL Great Primer**|WP Fell Great Primer|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**Inria Serif**|WP Calcul|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Inter**|WP Between|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Jost**|WP Jasper|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Jura**|WP Ticket|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Kay Pho Du**|WP Kaye|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Kelvinch**|WP Kelvin|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The base fonts supports petite capitals; I created a small-capital opentype table to enable them to work with small-caps and fixed an error that cause ligatures to override the table. The broken kerning tables were removed to allow the font to save. The font has also been hinted.|
|**Labrada**|WP Kadabra|SIL Open Font License (version 1.1)|✅|✅|✅|❌|A kerning fix to the lowercase b was also made.|
|**Lexend**|WP Luthor|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Liberation Mono**|WP Libertino Mono|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Liberation Sans**|WP Libertino Sans|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Liberation Serif**|WP Libertino Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Libre Baskerville**|WP Mortimer|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Libre Caslon Text**|WP Caslon|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Linden Hill**|WP Hill House|SIL Open Font License (version 1.1)|❌|✅|❌|✅|The regular style already contained true small caps; small caps were created for the italic style based on those glyphs.|
|**Lora**|WP Arol|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Maitree**|WP My Tree|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Manuale**|WP Manually|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Mate**|WP Checkmate|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps. Small caps in the Italic style are scaled down letters.|
|**Merriweather**|WP Merry Weather|SIL Open Font License (version 1.1)|✅|✅|✅|✅|This fixes an issue which causes ligatures to have priority over small-caps in the base font.|
|**Newsreader**|WP Extra Extra|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Based on the 16 pt ("Text") version of the font.|
|**New Tegomin**|WP Cigarette Burns|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Non-latin characters have been removed.|
|**Nimbus Mono PS**|WP Postal| GNU AFFERO GENERAL PUBLIC LICENSE Version 3|✅|✅|✅|❌|Monospaced font.|
|**Noticia Text**|WP Notice|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**OCR-A**|WP OCR-A|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Custom glyphs have also been added.|
|**OCR-B**|WP OCR-B|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Custom glyphs have also been added.|
|**Old Timey Mono**|WP Old Timer|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Monospaced font.|
|**OpenDyslexic 2**|WP OD 2|Creative Commons Attribution 4.0 International license (CC BY 4.0)|✅|✅|✅|❌|Based off OpenDyslexic 2.x.|
|**OpenDyslexic 4**|WP OD 4|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Based off OpenDyslexic 4.x. Font left/right bearings have been greatly reduced. The double-story "a" has replaced the single-story a in the Regular/Bold styles (it has been made bolder in the bold style, too).|
|**Orbit**|WP Galaxy|SIL Open Font License (version 1.1)|❌|❌|❌|❌|Monospaced font. Ligatures and Korean removed.|
|**Outfit**|WP Outfitted|SIL Open Font License (version 1.1)|✅|❌|❌|❌|The "ft" ligature has been made a standard ligature.|
|**Overlock**|WP Overlocked|SIL Open Font License (version 1.1)|✅|✅|✅|⚠️|Small caps were enabled in the regular style. Scaled-down small cap glyphs were added to the other files. Ligatures were enabled across all files.|
|**Overpass**|WP Underpass|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Pixel Code**|WP PixelC|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Philospher**|WP Philosophy|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Poly**|WP Polybius|SIL Open Font License (version 1.1)|❌|✅|❌|✅|The regular style already contained true small caps; small caps were created for the italic style based on those glyphs.|
|**Poppins**|WP Mary|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Proza Libre**|WP Prose|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Ligatures have been enabled.|
|**PT Serif**|WP Petey Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Radley**|WP Radical|SIL Open Font License (version 1.1)|❌|✅|❌|❌||
|**Reddit Sans**|WP We Did It|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Roboto Mono**|WP Bot Mono|SIL Open Font License (version 1.1)|✅|✅|✅|✅|Monospaced font. Corrected the SMCP table in the font and added a C2SC table.|
|**Roboto Serif**|WP Bot Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Rosarivo**|WP Rosebud|SIL Open Font License (version 1.1)|❌|✅|❌|❌||
|**Sedan**|WP Vroom|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps. Small caps in the Italic style are scaled down letters. Custom ligatures were added, and a major kerning fix was made.|
|**Shippori Mincho**|WP S Mincho|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Japanese characters have been removed.|
|**Special Elite**|WP Elite|Apache License (version 2.0)|❌|❌|❌|❌||
|**Sorts Mill Goudy**|WP Out of Sorts|SIL Open Font License (version 1.1)|❌|✅|❌|✅|The regular style already contained true small caps; small caps were created for the italic style based on those glyphs.|
|**Source Serif 4**|WP SSerif|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs.|
|**SUSE**|WP Geeko|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Tagesschrift**|WP One Day|SIL Open Font License (version 1.1)|❌|❌|❌|❌||
|**Texturina**|WP Texture|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Typey McTypeface**|WP Face Off|SIL Open Font License (version 1.1)|❌|✅|❌|❌||
|**Ubuntu**|Ubuntu WP|UBUNTU FONT LICENCE|✅|✅|✅|❌|The font is named differently than other fonts in this repo due to the font's license terms.|
|**Vesper Libre**|WP Venus|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Devanagari characters have been removed.|
|**Vollkorn**|WP Korn|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs.|
|**Zen Old Mincho**|WP Old Mincho|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Japanese characters have been removed. While a bold file is included (based on the Black file), it's very subtle. You may want to consider using only the regular file and having KOReader fake the bold effect.|

## FAQs:

**Q: How do I install these?**  
**A:** See the user guide here: https://koreader.rocks/user_guide/#L2-fonts

**Q: Should I use these fonts outside of KOReader?**  
**A:** In many cases, there’s no advantage to using these files outside of KOReader, as most other popular ereaders (Kindle, Kobo, etc) and software (Calibre, etc) will automatically generate their own fake small-capital letters. There are also a handful of fonts (mostly the IM FELL collection) where I use true small-capital glyphs, as I was able to extract them from the “SC” font file from within the family and merge them into the regular font files; you would see a benefit from using those in Kindle or other apps that support true small-capitals. Kobo’s KEPUB engine is pretty bad when it comes to supporting proper typography (how do they not properly support kerning and ligatures out of the box in 2025?); among its many flaws, it won’t use small-caps even when present in the original file and will always fake them.

**Q: Did you make any other changes to these files?**  
**A:** Various other changes have occasionally been made; see the notes for each font above. Among the changes I tend to make:kerning adjustments (usually for glaring errors, but sometimes I'd improve the kerning classes), enabling ligatures that weren’t properly enabled in the original files, manually creating extra ligatures when they were badly needed, hinting the fonts using TTFAutohint, and removing scripts besides Latin and Greek to reduce file sizes (especially with the "Mincho" files).

**Q: Will you add Bookerly, Rakuten Serif, or (insert proprietary font here)?**  
**A:** Unfortunately, I cannot legally edit or redistribute these font files due to their restrictive font licenses. FYI, the latest version of Bookerly contained on the Kindle’s firmware *does* have small-caps built in (the version hosted on the Amazon Developer site for developers is outdated).

**Q: Can you add or update (insert non-proprietary font here)?**  
**A:** First, check to make sure the font you’re looking at doesn’t already include small-caps. If it does, I won’t have a version here (unless something is seriously messed up with the base font). I want to move on from this obsession of mine, so I only really would consider creating monospaced fonts (as they require no kerning, by far the most time-intensive step), fonts that lack kerning entirely, fonts that only use kerning pairs rather than classes (as they can have kerning copied effortlessly), or fonts that are so good that they feel worth the time investment for me. Create an issue in the GitHub issue tracker if a font catches your eye that you'd like to see a KOReader-friendly version of.

**Q: Can you add the glyphs from (insert language here)?**  
**A:** To save time, these files were created and use only the glyph sets I expect to run across in the books I read (Latin and Greek). I currently do not have plans to re-do any of these fonts with other glyph sets. However, I’ve provided instructions on how to make your own fake small-caps below.

**Q: Can you create variable versions of these fonts?**  
**A:** I use FontForge, which currently doesn’t support this.

**Q: I found an issue unrelated to small caps with the font. Should I let you know?**  
**A:** I'm open to fixing glaring kerning errors/encoding errors/etc with these fonts, provided I can do so in a reasonable amount of time (I'd fix a couple of really bad kerning pairs, but I'm not re-kerning an entire font, for example). Open an Issue in the Issues tracker and I'll let you know if I can handle it.

**Q: Why were the font files renamed?**  
**A:** To avoid confusion with the original font files, as well as to allow the modified files to coexist with the originals. Additionally, fonts under the OFL often have reserved font names. To legally redistribute them, I had to change the font names.

**Q: How were the font names chosen?**  
**A:** I just used references or puns that came to mind, most of the time.

**Q: Why are the Italic/Bold/Bold Italic files missing?**  
**A:** Font styles will be missing when the original font lacks them. I try to favor fonts that include all four styles, but oftentimes I liked the base font enough to include it anyway and deal with KOReader applying a fake oblique and/or bold effect when needed. Your ereader/app will probably fake these effects if they’re missing (The only exception I’m aware of is Kindle, which won’t properly render Bold Italic if you are missing the Bold Italic File but have regular Bold and Italic; in that case, delete/don’t use the Bold file at all).

**Q: (Insert font here from the collection) just released an updated version with true small-caps!**  
**A:** Please let me know if this happens and update your ereader/computer with the official files. I will retire the customized version in that case. Real small-caps always look better than fake, scaled-down ones.

## How to create your own fake small caps in FontForge:

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
9. MONOSPACE FONTS ONLY: Right click on any uppercase or lowercase letter (don't use one of the newly created small cap glyphs for this), then go to metrics → set width. Note the width somewhere (you'll need it soon).
10. *MONOSPACE FONTS ONLY: Select all glyphs in the font (edit → select → select all), then select edit → Unlink reference.*
11. *MONOSPACE FONTS ONLY: Select all glyphs, then select metrics → set width. Set the width of all glyphs in the font to the number from step 9. You need to do this so that FontForge flags the font as a monospace font (this is needed, in turn, so that KOReader recognizes the font as a monospace font).*
12. *MONOSPACE FONTS ONLY: Select Metrics → Center in width.*
13. Go to Element → Font info → Lookups. Under GSUB, we’ll need to edit two tables so that smallcap lookups happen correctly. Move smcp and c2sc to the top of your list, if they aren't there already (the order of those two doesn’t matter; those two just need to be above everything else). Hit the plus button for each, then click the entry that pops up, and finally click Edit Data. IN ORDER, do the following: Remove All, Populate, Remove empty. You’ll know you messed this step up if you see dots about your small-capital “I”s when you test out the font!
14. *OPTIONAL: If you want proper kerning for the small-capital glyphs, you’re going to have to manually add it in. Step 7 copied over any kerning pairs your font may have had, but if your font also uses kerning tables (common, especially for newer fonts), the process is nightmarish. See instructions below. I’m not going to sugarcoat it; that can be a brutal process and takes way, way too long, so if you can live without proper kerning, skip this step. I couldn’t, so all fonts here are kerned.*
15. Go to file → Generate fonts and generate your fonts!  

Masochists only: Kerning your fonts that include kerning classes.  

1. PREREQUISTE: Keep unaltered copies of your fonts handy.
2. You'll need to manually add all your small-cap glyphs to the kerning classes that the glyphs they’re based off of are in (for example, you’d add “a.sc” to the Kerning classes “A” is in). Save a copy of the new font file(s) with these additions.
3. Create 2 new files titled Left and Right.
4. Remove all glyphs from ALL kerning classes on the left or right side, besides the .sc glyphs (you should delete any tables that don't have .sc glyphs on the side you're working on). Save.
5. Repeat step 4, but in the other file/on the other side. Save.
6. Load the file from step 2. Delete all kerning classes.
7. Load the vanilla font from step one from within the same window (this enables imports).
8. Go to the kerning class tables (element → font info → lookups → GPOS) and import the kerning tables from the other font (delete any "per glyph" tables; they'll be blank. The same goes for the following steps). Give the table and classes unique numbers/names (or you may run into wonky behavior).
9. Arrange the kerning classes in the same order as the are in the base font. Save and quit FontForge (this prevents crashes).
10. Open the file you're working on. Within that window, open the "left" or "right" file.
11. Import the kerning classes from that file. Arrange the imported classes below the existing ones. Save and quit.
12. Open the file you're working on. Within that window, open the "left" or "right" file not used in step 10.
13. Import the kerning classes from that file. Arrange the imported classes below the existing ones. Merge them into the classes from step 11 (merge them in the same order; for example, you'd merge kerning class 4 from the right file into class 4 from the left).
14. Export the font.

**IMPORTANT NOTE:** I recommend saving in the file format that the original font files were in to avoid losing the font’s hinting data. For ttf files, generate the fonts in “TrueType” format, and make sure that within the Options box you have the following settings checked:
- Hints
- Flex Hints
- TrueType Hints
- PS Glyph Names
- OpenType
- FFTM

Make very sure that “Apple”, “windows-compatible kern”, “old style kern”, and “prefer native kerning” are NOT checked. If the font was originally an OTF file, save it as an “OpenType (CFF)” file.
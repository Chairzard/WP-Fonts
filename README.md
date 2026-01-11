# WP Fonts - Customized fonts with added small-caps for KOReader!

One of the only shortcomings of KOReader is that the engine it uses can’t create fake small-capital letters when a font lacks them and instead renders the text in lowercase (according to the developers, this is not a feature that is viable to add in due to how the engine functions). Some of my most beloved fonts don't have small-caps baked in, and losing the small cap formatting hurts my soul. However, the engine does support small-capitals for fonts that include them already. To take advantage of this and feed my unchecked font addiction, I’ve created (too many) fonts with custom small-capitals and created a GitHub repository to host them (they’re spartan and just scaled-down capital letters like a web browser/the Kobo stock reader would do, but they’ll do the trick in a pinch). With these fonts, you can go from this:  

<img width="509" height="84" alt="image" src="https://github.com/user-attachments/assets/1acbdf2e-d6bd-4cf9-95b8-69c8ad2cf6fb" />

To this:

<img width="509" height="84" alt="image" src="https://github.com/user-attachments/assets/81048731-b9e8-4376-9c31-1fddf4804d4b" />

The various fonts contained within this repository are licensed under different licenses. When possible, my license of choice is the the SIL Open Font License (I've included an FAQ about it in the main folder of the repo).

Kerning was also added for the fake small-caps, provided the original font had kerning for its uppercase letters (I just copied over the kerning from the uppercase letters, so a word in small-caps will have the same appearance as a word in all uppercase, just scaled-down to roughly the font’s x-height, +/- 0-20% depending on the font).

## Current list of fonts available:

You may also be interested in my [list of of fonts with real small-caps](https://github.com/Chairzard/WP-Fonts/blob/main/Recommend%20fonts%20with%20real%20small-caps.md). In most cases, I will not be releasing modified versions of those, unless they are missing small caps in certain styles (or have really bad kerning issues that I can fix).  

Fonts without Bold/Italic files are still usable in KOReader. KOReader will create an artificial bold effect or apply an oblique effect, respectively, for fonts missing these files. Fonts marked as "true" small caps use small capitals with the correct stroke width, taken from other style files for the font (fonts marked with an X just use generic, scaled-down capital letters).

|Original font name|Edited font name|Font license|Bold?|Italics?|Bold Italics?|"True" small caps?|Notes|
|---|---|---|---|---|---|---|---|
|**Adelphe**|WP Affinity|Open Inclusif·ve Fonte Licence|✅|✅|✅|❌|This release is based on the Mar 18, 2024 Adelphe font files, as the latest version uses the more restrictive CUTE License.|
|**Afacad**|WP Dacafa|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Afacad was chosen rather than Afacad Flux due to its italic/bold italic styles.|
|**Archivo**|WP Archivist|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Asul**|WP Lusa|SIL Open Font License (version 1.1)|✅|❌|❌|❌|Custom ligatures have also been added.|
|**Atkinson Hyperlegible Next**|WP Hyperlegible|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Baskervville**|WP Stapleton|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs.|
|**Courier Prime**|WP Prime Time|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Monospace. Ligatures have been disabled.|
|**Crimson Pro**|WP Seeing Red|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**IM FELL Double Pica**|WP Fell Double Pica|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL DW Pica**|WP Fell DW Pica|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL English**|WP Fell English|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL French Canon**|WP Fell French Canon|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**IM FELL Great Primer**|WP Fell Great Primer|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps, merged from the "SC" font files. Small caps in the Italic style are scaled down letters.|
|**Jost**|WP Jasper|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Lexend**|WP Luthor|SIL Open Font License (version 1.1)|✅|❌|❌|❌||
|**Libre Baskerville**|WP Mortimer|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Lora**|WP Arol|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Newsreader**|WP Extra Extra|SIL Open Font License (version 1.1)|✅|✅|✅|❌|Based on the 16 pt ("Text") version of the font.|
|**OpenDyslexic**|WP OD|Creative Commons Attribution 4.0 International license (CC BY 4.0)|✅|✅|✅|❌|Based off OpenDyslexic 2.x, not the latest version (4.x has weird kerning/spacing issues)|
|**PT Serif**|WP Petey Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Roboto Serif**|WP Bot Serif|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Sedan**|WP Vroom|SIL Open Font License (version 1.1)|❌|✅|❌|⚠️|Small caps in the regular style are true small caps. Small caps in the Italic style are scaled down letters. Custom ligatures were added, and a major kerning fix was made.|
|**Special Elite**|WP Elite|Apache License (version 2.0)|❌|❌|❌|❌||
|**Source Serif 4**|WP SSerif|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs.|
|**Texturina**|WP Texture|SIL Open Font License (version 1.1)|✅|✅|✅|❌||
|**Vollkorn**|WP Korn|SIL Open Font License (version 1.1)|✅|✅|✅|✅|The regular and bold styles already contained true small caps; small caps were created for the italic/bold italic styles based on those glyphs.|

## FAQs:

**Q:** How do I install these?  
**A:** See the user guide here: https://koreader.rocks/user_guide/#L2-fonts

**Q:** Should I use these fonts outside of KOReader?  
**A:** In many cases, there’s no advantage to using these files outside of KOReader, as most other popular ereaders (Kindle, Kobo, etc) and software (Calibre, etc) will automatically generate their own fake small-capital letters. There are also a handful of fonts (mostly the IM FELL collection) where I use true small-capital glyphs, as I was able to extract them from the “SC” font file from within the family and merge them into the regular font files; you would see a benefit from using those in Kindle or other apps that support true small-capitals. Kobo’s KEPUB engine is pretty bad when it comes to supporting proper typography (how do they not properly support kerning and ligatures out of the box in 2025?); among its many flaws, it won’t use small-caps even when present in the original file and will always fake them.

**Q:** Did you make any other changes to these files?  
**A:** In some cases, I made kerning adjustments or enabled ligatures that weren’t properly enabled in the original files. In one or two cases, I manually created extra ligatures when they were badly needed. In a couple of cases, I also rehinted the fonts using TTFAutohint.

**Q:** Will you add Bookerly, Rakuten Serif, or (insert proprietary font here)?  
**A:** Unfortunately, I cannot legally edit or share these font files due to their restrictive font licenses. FYI, the latest version of Bookerly contained on the Kindle’s firmware does have small-caps built in (the version hosted on the Amazon Developer site for developers is outdated). See the mobileread forums for more info on this.

**Q:** Can you add or update (insert non-proprietary font here)?  
**A:** First, check to make sure the font you’re looking at doesn’t already include small-caps. If it does, I won’t have a version here. If the font doesn’t have small-caps, as long as the font you want is available under an open font license such as the OFL/GUST license/etc, I’d consider adding it. I probably only want to update fonts already listed here if the base font has had a major change, and I primarily want to add Serif fonts at this point. There are more than enough good sans-serif fonts out there, some with true small-caps like Work Sans, TeX Gyre Heros, Roboto, Noto Sans, Fira Sans, Raleway, Montserrat, and Sofia Sans, just to name a few. However, if there’s a Sans Serif font that truly stands out or if I feel I can handle it quickly, I’d consider it (I can process a font that uses kerning classes only dramatically faster than one that uses kerning tables in FontForge). Create an issue in the GitHub issue tracker, and I’ll at least take a look.

**Q:** Can you add the glyphs from (insert language here)?  
**A:** To save time, these files were created and use only the glyph sets I expect to run across in the books I read (Latin and Greek). I currently do not have plans to re-do any of these fonts with other glyph sets. However, I’ve provided instructions on how to make your own fake small-caps below.

**Q:** Can you create variable versions of these fonts?  
**A:** I use FontForge, which currently doesn’t support this.

**Q:** I found an issue unrelated to small caps with the font. Should I let you know?  
**A:** I'm open to fixing glaring kerning errors/encoding errors/etc with these fonts, provided I can do so in a reasonable amount of time (I'd fix a couple of really bad kerning pairs, but I'm not re-kerning an entire font, for example). Open an Issue in the Issues tracker and I'll let you know if I can handle it.

**Q:** Why were the font files renamed?  
**A:** To avoid confusion with the original font files, as well as to allow the modified files to coexist with the originals. Additionally, fonts under the OFL often have reserved font names. To legally redistribute them, I had to change the font names.

**Q:** Why are the Italic/Bold/Bold Italic files missing?  
**A:** Font styles will be missing when the original font lacks them. I try to favor fonts that include all four styles, but oftentimes I liked the base font enough to include it anyway and deal with KOReader applying a fake oblique and/or bold effect when needed. Your ereader/app will probably fake these effects if they’re missing (The only exception I’m aware of is Kindle, which won’t properly render Bold Italic if you are missing the Bold Italic File but have regular Bold and Italic; in that case, delete/don’t use the Bold file at all).

**Q:** (Insert font here from the collection) just released an updated version with true small-caps!  
**A:** Please let me know if this happens and update your ereader/computer with the official files. I will retire the customized version in that case. Real small-caps always look better than fake, scaled-down ones.

## How to create your own fake small caps in FontForge:

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
14. *OPTIONAL: If you want proper kerning for the small-capital glyphs, you’re going to have to manually add it in. Step (insert) copied over any kerning pairs your font may have had, but if your font also uses kerning tables (common, especially for newer fonts), the only way that I know of to do this is to manually add all your small-cap glyphs to the kerning classes that the glyphs they’re based off of are in (for example, you’d add “a.sc” to the Kerning classes “A” is in). I’m not going to sugarcoat it; this can be a brutal process and take way too long, so if you can live without proper kerning, skip this step. I couldn’t, so all fonts here are kerned.*
15. Go to file → Generate fonts and generate your fonts!

**IMPORTANT NOTE:** I recommend saving in the file format that the original font files were in to avoid losing the font’s hinting data. For ttf files, generate the fonts in “TrueType” format, and make sure that within the Options box you have the following settings checked:
- Hints
- Flex Hints
- TrueType Hints
- PS Glyph Names
- OpenType
- FFTM

Make very sure that “Apple”, “windows-compatible kern”, “old style kern”, and “prefer native kerning” are NOT checked. If the font was originally an OTF file, save it as an “OpenType (CFF)” file.

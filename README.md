[English](README.md) ∷ [Bahasa Melayu Rumi](README_ms.md) ∷ [بهاس ملايو جاوي](README_ms-Arab.md)

# Jawi Font

Edited version of Arabic font files to add support for Jawi alphabets.


## What is this repository?

This repository contains the original release files of selected open-source Arabic fonts, the FontForge files of edited Arabic fonts, and the released packages of the edited Arabic fonts with support for [Jawi alphabet](https://en.wikipedia.org/wiki/Jawi_alphabet).


## Why did you edit the font files?

There is a limited number of open-source Arabic fonts, and out of those, only small amount of them actually support Jawi alphabet.

The fonts released from this repository will have full support for Jawi alphabet and they will also be usable in older applications where usage of styling sets (ss01 etc) are not possible.


## When was this repository created?

The repository was created on 30 May 2020 (UTF+8).


## Where are the font editing being done?

The fonts are edited on FontForge running on Ubuntu instance via UserLAnd app on my phone. I don't currently have access to any desktop device and will never have any desktop device unless I get accepted for job to earn enough money to build a desktop.


Technical details:

- FontForge version: 11:12 UTC 24-Sep-2017 (latest version available on APT as of 30 May 2020)
- Ubuntu version: Ubuntu 18.04.4 LTS aarch64 (default installation of Ubuntu on UserLAnd)
- UserLAnd version: UserLAnd 2.7.2 (latest version available on my Play store as of 30 May 2020)
- Android version: 8.0.0 (latest version available for this phone as of 30 May 2020)
- Phone model: Samsung Galaxy S7 Edge (SM-G935F), handed to me from my aunt in December 2019 (before that, I've been using Sony Xperia C5 Ultra Dual from 2014, it finally ended its life in March 2020, unable to boot anymore)


## Who maintain these edited fonts?

The owner of the repository, [Yaya MNH48](https://meta.mnh48.moe), acting as the sole owner of the organization jawi-mnh48.


## How the fonts are edited?

By following the steps in the tutorial titled "[Adding Glyphs to an Arabic Font](http://designwithfontforge.com/en-US/Adding_Glyphs_to_an_Arabic_Font.html)" on the website [Design With FontForge](http://designwithfontforge.com/).

The glyphs that I edit to make it support Jawi alphabet:

- Changing Arabic comma (،) at U+060C to Jawi comma.
  - Majority of digital users of Jawi alphabet uses U+060C for comma as it is what most keyboard have even though it is not actual character for Jawi comma, which doesn't exist in Unicode.
  - On some program and font, Jawi comma is displayed in place of Arabic comma when the program tells the font about the language used in the specified text being Malay, but not all programs or fonts supported this.
    - Known supported fonts are Calibri and Amiri.
    - Known supported programs are Microsoft Office and LibreOffice 6.1+, with limited support in GIMP.
  - In real life handwriting, all Jawi users write the comma the correct way, which is different from Arabic comma.
  - The edited font reversed this, so default would be Jawi comma, and Arabic comma will be displayed instead only if language is Arabic. This makes it display Jawi comma by default when no language is specified, useful for older programs to display Jawi.
  - Jawi comma looked like this: ![jawicomma](img/github/jawicomma.png).
- Point glyph of Reversed comma (⹁) at U+2E41 to Arabic comma U+060C after the change of glyph from Arabic comma to Jawi comma.
  - Some minority people used U+2E41 for comma as it looked more similar to Jawi comma compared to U+060C, but the character being outside Arabic block made some programs broke.
- Changing Arabic semicolon (؛) at U+061B to Jawi semicolon.
  - Majority of digital users of Jawi alphabet uses U+061B for semicolon as it is what most keyboard have even though it is not actual character for Jawi semicolon, which doesn't exist in Unicode.
  - On some program and font, Jawi semicolon is displayed in place of Arabic semicolon when the program tells the font about the language used in the specified text being Malay, but not all programs or fonts supported this.
    - Known supported fonts are Calibri and Amiri.
    - Known supported programs are Microsoft Office and LibreOffice 6.1+, with limited support in GIMP.
  - In real life handwriting, all Jawi users write the semicolon the correct way, which is different from Arabic semicolon.
  - The edited font reversed this, so default would be Jawi semicolon, and Arabic semicolon will be displayed instead only if language is Arabic. This makes it display Jawi semicolon by default when no language is specified, useful for older programs to display Jawi.
  - Jawi semicolon looked like this: ![jawisemicolon](img/github/jawisemicolon.png).
- Point glyph of Reversed semicolon (⁏) at U+204F to Arabic semicolon U+061B after the change of glyph from Arabic semicolon to Jawi semicolon.
  - Some minority people used U+204F for semicolon as it looked more similar to Jawi semicolon compared to U+061B, but the character being outside Arabic block made some programs broke.
- Add glyph for Jawi letter NGA (ڠ) at U+06A0, known in Unicode as Arabic Letter Ain with Three Dots Above, used in Malay for the sound /ŋ/.
- Add glyph for Jawi letter GA (ݢ) at U+0762, known in Unicode as Arabic Letter Keheh with Dot Above, used in Malay for the sound /g/.
- Add glyph for Jawi letter VA (ۏ) at U+06CF, known in Unicode as Arabic Letter Waw with Dot Above, used in Malay for the sound /v/.
- Add glyph for Jawi letter NYA (ڽ) at U+06BD, known in Unicode as Arabic Letter Noon with Three Dots Above, used in Malay for the sound /ɲ/.
- Changing the glyph for Arabic hamza (ء) at U+0621 to Jawi letter three quarter hamzah.
  - Majority of digital users of Jawi alphabet uses U+0621 for three quarter hamzah as it is what most keyboard have even though it is not actual character for Jawi letter three quarter hamzah, which doesn't exist in Unicode.
  - The three quarter positioning is sometimes emulated by putting U+0621 in superscript, but that only work in program that support superscripting non-superscript letters. The position is sometimes higher than expected and appears smaller in size when superscripted, which is different from what we actually use in Malay.
  - Jawi three quarter hamzah is not supported in any known fonts. 
  - In real life handwriting, all Jawi users write the three quarter hamzah the correct way, which is different from Arabic hamza.
  - The edited font make Jawi letter three quarter hamzah displayed by default in place of Arabic hamza, and Arabic hamza will be displayed instead only if language is Arabic. This makes it display Jawi three quarter hamzah by default when no language is specified, useful for older programs to display Jawi.
  - Jawi three quarter hamzah looked like this: ![jawi¾hamzah](img/github/jawi¾hamzah.png).
- Point glyph of Arabic high hamza (ٴ) at U+0674 to Arabic hamza U+0621 after the change of glyph from Arabic hamza to Jawi three quarter hamzah.
  - Some minority people used U+0674 for three quarter high hamza as it looked more similar to Jawi hamzah compared to U+0621, but the character is supposed to be part of diphtong and positioned with another vowel in other languages, unlike in Jawi where three quarter hamzah is a standalone letter.
- Add glyph for Jawi old letter GA (ڬ) at U+06AC, known in Unicode as Arabic Letter Kaf with Dot Above, formerly used in Malay for the sound /g/ when Arabic Letter Keheh with Dot Above (ݢ) at U+0762 was not accessible on keyboard.
  - Glyph is for compatibility purposes.
  - In real life handwriting, ڬ was never used in old writing, and it is not used unless for stylistic choice in new writing or used by mistake by people who learnt Jawi using digital tools created in those time when ݢ is not accessible on keyboard, it should always be ݢ in actual writing.
  - ڬ is not formally recognized as a letter in Malay.

Some Arabic fonts had even less glyph coverage and those need more works to do including:

- Add glyph for Jawi letter CA (چ) at U+0686, known in Unicode as Arabic Letter Tcheh, used in Malay for the sound /t͡ʃ/.
- Add glyph for Jawi letter PA (ڤ) at U+06A4, known in Unicode as Arabic Letter Veh, used in Malay for the sound /p/.
- Add glyph for Jawi letter KAF (ک) at U+06A9, known in Unicode as Arabic Letter Keheh, used in Malay for the sound /k/.
- Add glyph for Jawi letter YE (ى) at U+0649, known in Unicode as Arabic Letter Alef Maksura, used in Malay for the final sound /ə/.
- Add glyph for Jawi letter ALIF WITH HAMZAH (أ) at U+0623, known in Unicode as Arabic Letter Alef with Hamza Above, used as a part of diphtongs that can't be used with standalone three quarter hamzah nor without any hamzah. Example: أيمن (aiman) is different from اءيمن (a'iman) and ايمن (iman).
  - See image version below <br/> ![aiman](img/github/aiman.png)

For compatibility reason, a few more glyphs will also be checked and added if they don't exist:

- Add glyph for non-Jawi letter known in Unicode as Arabic Letter Yeh with Hamza Above (ئ) at U+0626.
  - Glyph added for compatibility reason.
  - This was used in old Jawi as the diphtongs /ai/ and /ae/ (both are now written as أي), and the sound /iʔ/ and /eʔ/ (both are now written as يء).
  - Still in used as part of the Malay family name Nik (نئ) such as [Nik Abdul Aziz](https://en.wikipedia.org/wiki/Nik_Abdul_Aziz_Nik_Mat) (نئ عبدالعزيز).
- Add glyph for non-Jawi letter known in Unicode as Arabic Letter Waw with Hamza Above (ؤ) at U+0624.
  - Glyph added for compatibility reason.
  - This was used in old Jawi as the diphtongs /ao/ and /au/ (both are now written as أو) and the sounds /uʔ/ and /oʔ/ (both are now written as وء).

All other letters should already exist in common Arabic fonts, including one deprecated letter:
- Jawi letter OLD KAF (ك) at U+0643, known in Unicode as Arabic Letter Kaf, formerly used in Malay for the sound /k/ when Arabic Letter Keheh (ک) at U+06A9 was not accessible on keyboard.
  - Glyph is for compatibility purposes.
  - In real life handwriting, ك was never used in old writing, and it is not used unless for stylistic choice in new writing or used by mistake by people who learnt Jawi using digital tools created in those time when ک is not accessible on keyboard, it should always be ک in actual writing.
  - ك is not formally recognized as a letter in Malay.
  - ك is called as Arabic Kaf by Malays, as opposed to just Kaf, because Kaf in Malay is ک.


Table of all letters in the Jawi alphabet used in Malay:

  <table>
    <tr>
      <th>Letter</th>
      <th>Malay Name</th>
      <th>Unicode Codepoint</th>
      <th>Unicode Name</th>
      <th>Sound represented</th>
      <th>Rumi equivalent</th>
      <th>Sample word (Jawi)</th>
      <th>Sample word (Rumi)</th>
      <th>Sample word (IPA)</th>
    </tr>
    <tr>
      <td rowspan="3"><span lang="ms-Arab">ا</span></td>
      <td rowspan="3">Alif</td>
      <td rowspan="3">U+0627</td>
      <td rowspan="3">Arabic letter alef</td>
      <td>/a/</td>
      <td>a</td>
      <td><span style="color:red;">ا</span>يم</td>
      <td><span style="color:red;">a</span>yam</td>
      <td>/<span style="color:red;">a</span>.jam/</td>
    </tr>
    <tr>
      <td>/ə/</td>
      <td>e (ĕ)</td>
      <td><span lang="ms-Arab">مميتابوليسم<span style="color:red;">ا</span>کن</span></td>
      <td>memetabolism<span style="color:red;">e</span>kan</td>
      <td>/mə.me.ta.bo.lis.m<span style="color:red;">ə</span>.kan/</td>
    </tr>
    <tr>
      <td>No sound</td>
      <td>(Vowel starter)</td>
      <td><span lang="ms-Arab"><span style="color:red;">ا</span>ينده</span></td>
      <td><span style="text-decoration:underline;-webkit-text-decoration-color:red;text-decoration-color:red;">i</span>ndah</td>
      <td>/<span style="text-decoration:underline;-webkit-text-decoration-color:red;text-decoration-color:red;">i</span>n.dah/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ب</span></td>
      <td>Ba</td>
      <td>U+0628</td>
      <td>Arabic Letter Beh</td>
      <td>/b/</td>
      <td>b</td>
      <td><span lang="ms-Arab"><span style="color:red;">ب</span>اچ</span></td>
      <td><span style="color:red;">b</span>aca</td>
      <td>/<span style="color:red;">b</span>a.t͡ʃa/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ت</span></td>
      <td>Ta</td>
      <td>U+062A</td>
      <td>Arabic letter teh</td>
      <td>/t/</td>
      <td>t</td>
      <td><span lang="ms-Arab"><span style="color:red;">تت</span>يکوس</span></td>
      <td><span style="color:red;">t</span>e<span style="color:red;">t</span>ikus</td>
      <td>/<span style="color:red;">t</span>ə.<span style="color:red;">t</span>i.kus/</td>
    </tr>
    <tr>
      <td rowspan="2"><span lang="ms-Arab">ث</span></td>
      <td rowspan="2">Sa</td>
      <td rowspan="2">U+062B</td>
      <td rowspan="2">Arabic letter theh</td>
      <td>/θ/</td>
      <td rowspan="2">s</td>
      <td rowspan="2"><span lang="ms-Arab"><span style="color:red;">ث</span>لا<span style="color:red;">ث</span></span></td>
      <td rowspan="2"><span style="color:red;">s</span>ela<span style="color:red;">s</span>a</td>
      <td>/<span style="color:red;">θ</span>a.laː.<span style="color:red;">θ</span>ah/</td>
    </tr>
    <tr>
      <td>/s/</td>
      <td>/<span style="color:red;">s</span>ə.la.<span style="color:red;">s</span>a/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ج</span></td>
      <td>Jim</td>
      <td>U+062C</td>
      <td>Arabic letter jeem</td>
      <td>/d͡ʒ/</td>
      <td>j</td>
      <td><span lang="ms-Arab"><span style="color:red;">ج</span>اري</span></td>
      <td><span style="color:red;">j</span>ari</td>
      <td>/<span style="color:red;">d͡ʒ</span>a.ri/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">چ</span></td>
      <td>Ca</td>
      <td>U+0686</td>
      <td>Arabic letter tcheh</td>
      <td>/t͡ʃ/</td>
      <td>c</td>
      <td><span lang="ms-Arab"><span style="color:red;">چ</span>ريتا</span></td>
      <td><span style="color:red;">c</span>erita</td>
      <td>/<span style="color:red;">t͡ʃ</span>ə.ri.ta/</td>
    </tr>
    <tr>
      <td rowspan="4"><span lang="ms-Arab">ح</span></td>
      <td rowspan="4">Ha kecil / Ha pedas</td>
      <td rowspan="4">U+062D</td>
      <td rowspan="4">Arabic letter hah</td>
      <td>/ḥ/</td>
      <td rowspan="4">h</td>
      <td rowspan="2"><span lang="ms-Arab"><span style="color:red;">ح</span>روف</span></td>
      <td rowspan="2"><span style="color:red;">h</span>uruf</td>
      <td>/<span style="color:red;">ḥ</span>urūf/</td>
    </tr>
    <tr>
      <td rowspan="2">/h/</td>
      <td>/<span style="color:red;">h</span>u.rof/</td>
    </tr>
    <tr>
      <td rowspan="2"><span lang="ms-Arab"><span style="color:red;">ح</span>ال</span></td>
      <td rowspan="2"><span style="color:red;">h</span>al</td>
      <td>/<span style="color:red;">h</span>al/</td>
    </tr>
    <tr>
      <td>/ħ/</td>
      <td>/<span style="color:red;">ħ</span>aːl/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">خ</span></td>
      <td>Kha</td>
      <td>U+062E</td>
      <td>Arabic letter khah</td>
      <td>/x/</td>
      <td>kh</td>
      <td><span lang="ms-Arab"><span style="color:red;">خ</span>بر</span></td>
      <td><span style="color:red;">kh</span>abar</td>
      <td>/<span style="color:red;">x</span>a.bar/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">د</span></td>
      <td>Dal</td>
      <td>U+062F</td>
      <td>Arabic letter dal</td>
      <td>/d/</td>
      <td>d</td>
      <td><span lang="ms-Arab"><span style="color:red;">د</span>ا<span style="color:red;">د</span>و</span></td>
      <td><span style="color:red;">d</span>a<span style="color:red;">d</span>u</td>
      <td>/<span style="color:red;">d</span>a.<span style="color:red;">d</span>u/</td>
    </tr>
    <tr>
      <td rowspan="2"><span lang="ms-Arab">ذ</span></td>
      <td rowspan="2">Zal</td>
      <td rowspan="2">U+0630</td>
      <td rowspan="2">Arabic letter thal</td>
      <td>/ð/</td>
      <td rowspan="2">z</td>
      <td rowspan="2"><span lang="ms-Arab">بي<span style="color:red;">ذ</span>ا</span></td>
      <td rowspan="2">be<span style="color:red;">z</span>a</td>
      <td>/be.<span style="color:red;">ð</span>a/</td>
    </tr>
    <tr>
      <td>/z/</td>
      <td>/be.<span style="color:red;">z</span>a/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ر</span></td>
      <td>Ra</td>
      <td>U+0631</td>
      <td>Arabic letter reh</td>
      <td>/r/</td>
      <td>r</td>
      <td><span lang="ms-Arab"><span style="color:red;">ر</span>ڠکاين</span></td>
      <td><span style="color:red;">r</span>angkaian</td>
      <td>/<span style="color:red;">r</span>aŋ.kaj.jan/</td>
    </tr>
    <tr>
      <td rowspan="2"><span lang="ms-Arab">ز</span></td>
      <td rowspan="2">Zai</td>
      <td rowspan="2">U+0632</td>
      <td rowspan="2">Arabic letter zain</td>
      <td rowspan="2">/z/</td>
      <td>z</td>
      <td><span lang="ms-Arab"><span style="color:red;">ز</span>و</span></td>
      <td><span style="color:red;">z</span>oo</td>
      <td>/<span style="color:red;">z</span>u/</td>
    </tr>
    <tr>
      <td>x</td>
      <td><span lang="ms-Arab"><span style="color:red;">ز</span>ينون</span></td>
      <td><span style="color:red;">x</span>enon</td>
      <td>/<span style="color:red;">z</span>i.non/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">س</span></td>
      <td>Sin</td>
      <td>U+0633</td>
      <td>Arabic letter seen</td>
      <td>/s/</td>
      <td>s</td>
      <td><span lang="ms-Arab"><span style="color:red;">س</span>الين</span></td>
      <td><span style="color:red;">s</span>alin</td>
      <td>/<span style="color:red;">s</span>a.len/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ش</span></td>
      <td>Syin</td>
      <td>U+0634</td>
      <td>Arabic letter sheen</td>
      <td>/ʃ/</td>
      <td>sy</td>
      <td><span lang="ms-Arab"><span style="color:red;">ش</span>يليڠ</span></td>
      <td><span style="color:red;">sy</span>iling</td>
      <td>/<span style="color:red;">ʃ</span>i.liŋ/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ص</span></td>
      <td>Sad</td>
      <td>U+0635</td>
      <td>Arabic letter sad</td>
      <td>/s/</td>
      <td>s</td>
      <td><span lang="ms-Arab">ف<span style="color:red;">ص</span>ل</span></td>
      <td>fa<span style="color:red;">s</span>al</td>
      <td>/fa.<span style="color:red;">s</span>al/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ض</span></td>
      <td>Dad</td>
      <td>U+0636</td>
      <td>Arabic letter dad</td>
      <td>/d/</td>
      <td>d</td>
      <td><span lang="ms-Arab"><span style="color:red;">ض</span>رورة</span></td>
      <td><span style="color:red;">d</span>arurat</td>
      <td>/<span style="color:red;">d</span>a.ro.rat/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ط</span></td>
      <td>To</td>
      <td>U+0637</td>
      <td>Arabic letter tah</td>
      <td>/t/</td>
      <td>t</td>
      <td><span lang="ms-Arab"><span style="color:red;">ط</span>لاق</span></td>
      <td><span style="color:red;">t</span>alak</td>
      <td>/<span style="color:red;">t</span>a.laʔ/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ظ</span></td>
      <td>Zo</td>
      <td>U+0638</td>
      <td>Arabic letter zah</td>
      <td>/z/</td>
      <td>z</td>
      <td><span lang="ms-Arab"><span style="color:red;">ظ</span>هر</span></td>
      <td><span style="color:red;">z</span>ohor</td>
      <td>/<span style="color:red;">z</span>o.hor/</td>
    </tr>
    <tr>
      <td rowspan="4"><span lang="ms-Arab">ع</span></td>
      <td rowspan="4">Ain</td>
      <td rowspan="4">U+0639</td>
      <td rowspan="4">Arabic letter ain</td>
      <td rowspan="3">/ʕ/</td>
      <td>a</td>
      <td><span lang="ms-Arab">سا<span style="color:red;">ع</span>ة</span></td>
      <td>sa<span style="color:red;">a</span>t</td>
      <td>/sa.<span style="color:red;">ʕa</span>t/</td>
    </tr>
    <tr>
      <td>i</td>
      <td><span lang="ms-Arab"><span style="color:red;">ع</span>لمو</span></td>
      <td><span style="color:red;">i</span>lmu</td>
      <td>/<span style="color:red;">ʕi</span>l.mu/</td>
    </tr>
    <tr>
      <td>u</td>
      <td><span lang="ms-Arab"><span style="color:red;">ع</span>لماء</span></td>
      <td><span style="color:red;">u</span>lama</td>
      <td>/<span style="color:red;">ʕu</span>.la.maʔ/</td>
    </tr>
    <tr>
      <td>/ʔ/</td>
      <td>k</td>
      <td><span lang="ms-Arab">م<span style="color:red;">ع</span>نا</span></td>
      <td>ma<span style="color:red;">k</span>na</td>
      <td>/ma<span style="color:red;">ʔ</span>.na/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">غ</span></td>
      <td>Ghain</td>
      <td>U+063A</td>
      <td>Arabic letter ghain</td>
      <td>/ɣ/</td>
      <td>gh</td>
      <td><span lang="ms-Arab"><span style="color:red;">غ</span>يب</span></td>
      <td><span style="color:red;">gh</span>aib</td>
      <td>/<span style="color:red;">ɣ</span>a.eb/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ڠ</span></td>
      <td>Nga</td>
      <td>U+06A0</td>
      <td>Arabic letter ain with three dots above</td>
      <td>/ŋ/</td>
      <td>ng</td>
      <td><span lang="ms-Arab">ڤ<span style="color:red;">ڠ</span>ݢيل</span></td>
      <td>pa<span style="color:red;">ng</span>gil</td>
      <td>/pa<span style="color:red;">ŋ</span>.gel/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ف</span></td>
      <td>Fa</td>
      <td>U+0641</td>
      <td>Arabic letter feh</td>
      <td>/f/</td>
      <td>f</td>
      <td><span lang="ms-Arab"><span style="color:red;">ف</span>يلم</span></td>
      <td><span style="color:red;">f</span>ilem</td>
      <td>/<span style="color:red;">f</span>i.ləm/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ڤ</span></td>
      <td>Pa</td>
      <td>U+06A4</td>
      <td>Arabic letter veh</td>
      <td>/p/</td>
      <td>p</td>
      <td><span lang="ms-Arab"><span style="color:red;">ڤڤ</span>يجت</span></td>
      <td><span style="color:red;">p</span>e<span style="color:red;">p</span>ijat</td>
      <td>/<span style="color:red;">p</span>ə.<span style="color:red;">p</span>i.d͡ʒat/</td>
    </tr>
    <tr>
      <td rowspan="2"><span lang="ms-Arab">ق</span></td>
      <td rowspan="2">Qaf</td>
      <td rowspan="2">U+0642</td>
      <td rowspan="2">Arabic letter qaf</td>
      <td>/ʔ/</td>
      <td>k</td>
      <td><span lang="ms-Arab">تيد<span style="color:red;">ق</span></span></td>
      <td>tida<span style="color:red;">k</span></td>
      <td>/ti.da<span style="color:red;">ʔ</span>/</td>
    </tr>
    <tr>
      <td>/q/</td>
      <td>q</td>
      <td><span lang="ms-Arab"><span style="color:red;">ق</span>اريء</span></td>
      <td><span style="color:red;">q</span>ari</td>
      <td>/<span style="color:red;">q</span>a.riʔ/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ک</span></td>
      <td>Kaf</td>
      <td>U+06A9</td>
      <td>Arabic letter keheh</td>
      <td>/k/</td>
      <td>k</td>
      <td><span lang="ms-Arab"><span style="color:red;">ک</span>ريتا</span></td>
      <td><span style="color:red;">k</span>ereta</td>
      <td>/<span style="color:red;">k</span>ə.re.ta/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ݢ</span></td>
      <td>Ga</td>
      <td>U+0762</td>
      <td>Arabic letter keheh with dot above</td>
      <td>/ɡ/</td>
      <td>g</td>
      <td><span lang="ms-Arab"><span style="color:red;">ݢ</span>نتيان</span></td>
      <td><span style="color:red;">g</span>entian</td>
      <td>/<span style="color:red;">g</span>ən.ti.jan/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ل</span></td>
      <td>Lam</td>
      <td>U+0644</td>
      <td>Arabic letter lam</td>
      <td>/l/</td>
      <td>l</td>
      <td><span lang="ms-Arab"><span style="color:red;">ل</span>اما</span></td>
      <td><span style="color:red;">l</span>ama</td>
      <td>/<span style="color:red;">l</span>a.ma/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">م</span></td>
      <td>Mim</td>
      <td>U+0645</td>
      <td>Arabic letter meem</td>
      <td>/m/</td>
      <td>m</td>
      <td><span lang="ms-Arab"><span style="color:red;">م</span>ينو<span style="color:red;">م</span></span></td>
      <td><span style="color:red;">m</span>inu<span style="color:red;">m</span></td>
      <td>/<span style="color:red;">m</span>i.no<span style="color:red;">m</span>/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ن</span></td>
      <td>Nun</td>
      <td>U+0646</td>
      <td>Arabic letter noon</td>
      <td>/n/</td>
      <td>n</td>
      <td><span lang="ms-Arab">م<span style="color:red;">ن</span>اڠيس</span></td>
      <td>me<span style="color:red;">n</span>angis</td>
      <td>/mə.<span style="color:red;">n</span>a.ŋes/</td>
    </tr>
    <tr>
      <td rowspan="4"><span lang="ms-Arab">و</span></td>
      <td rowspan="4">Wau</td>
      <td rowspan="4">U+0648</td>
      <td rowspan="4">Arabic letter waw</td>
      <td>/w/</td>
      <td>w</td>
      <td><span lang="ms-Arab"><span style="color:red;">و</span>اڠ</span></td>
      <td><span style="color:red;">w</span>ang</td>
      <td>/<span style="color:red;">w</span>aŋ/</td>
    </tr>
    <tr>
      <td>/u/</td>
      <td>u</td>
      <td><span lang="ms-Arab">ا<span style="color:red;">و</span>نتوڠ</span></td>
      <td><span style="color:red;">u</span>ntung</td>
      <td>/<span style="color:red;">u</span>n.toŋ/</td>
    </tr>
    <tr>
      <td>/o/</td>
      <td rowspan="2">o</td>
      <td rowspan="2"><span lang="ms-Arab">ڤ<span style="color:red;">و</span>ت<span style="color:red;">و</span>ڠ</span></td>
      <td rowspan="2">p<span style="color:red;">o</span>t<span style="color:red;">o</span>ng</td>
      <td>/p<span style="color:red;">o</span>.t<span style="color:red;">o</span>ŋ/</td>
    </tr>
    <tr>
      <td>/ɔ/</td>
      <td>/p<span style="color:red;">ɔ</span>.toŋ/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ۏ</span></td>
      <td>Va</td>
      <td>U+06CF</td>
      <td>Arabic letter waw with dot above</td>
      <td>/v/</td>
      <td>v</td>
      <td><span lang="ms-Arab"><span style="color:red;">ۏ</span>ن</span></td>
      <td><span style="color:red;">v</span>an</td>
      <td>/<span style="color:red;">v</span>an/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ه</span></td>
      <td>Ha besar / Ha simpul</td>
      <td>U+0647</td>
      <td>Arabic letter heh</td>
      <td>/h/</td>
      <td>h</td>
      <td><span lang="ms-Arab"><span style="color:red;">ه</span>نتو</span></td>
      <td><span style="color:red;">h</span>antu</td>
      <td>/<span style="color:red;">h</span>an.tu/</td>
    </tr>
    <tr>
      <td rowspan="3"><span lang="ms-Arab">ة</span></td>
      <td rowspan="3">Ta marbutah</td>
      <td rowspan="3">U+0629</td>
      <td rowspan="3">Arabic letter teh marbuta</td>
      <td rowspan="2">/t/</td>
      <td rowspan="2">t</td>
      <td rowspan="2"><span lang="ms-Arab">عباد<span style="color:red;">ة</span></span></td>
      <td rowspan="2">ibada<span style="color:red;">t</span></td>
      <td>/i.ba.da<span style="color:red;">t</span>/</td>
    </tr>
    <tr>
      <td>/ʕi.ba.da<span style="color:red;">t</span>/</td>
    </tr>
    <tr>
      <td>/h/</td>
      <td>h</td>
      <td><span lang="ms-Arab">سور<span style="color:red;">ة</span></span></td>
      <td>sura<span style="color:red;">h</span></td>
      <td>/su.ra<span style="color:red;">h</span>/</td>
    </tr>
    <tr>
      <td rowspan="3"><span lang="ms-Arab">ء</span></td>
      <td rowspan="3">Hamzah</td>
      <td rowspan="3">U+0621</td>
      <td rowspan="3">Arabic letter hamza</td>
      <td rowspan="2">No sound</td>
      <td>(Diphtong marker)</td>
      <td><span lang="ms-Arab">ما<span style="color:red;">ء</span>ين</span></td>
      <td>m<span style="text-decoration:underline;-webkit-text-decoration-color:red;text-decoration-color:red;">ai</span>n</td>
      <td>/m<span style="text-decoration:underline;-webkit-text-decoration-color:red;text-decoration-color:red;">ai</span>n/</td>
    </tr>
    <tr>
      <td>(Pause marker)</td>
      <td><span lang="ms-Arab">لا<span style="color:red;">ء</span>وق</span></td>
      <td>l<span style="text-decoration:underline;-webkit-text-decoration-color:red;text-decoration-color:red;">au</span>k</td>
      <td>/l<span style="text-decoration:underline;-webkit-text-decoration-color:red;text-decoration-color:red;">a<span style="color:red;">.</span>o</span>ʔ/</td>
    </tr>
    <tr>
      <td>/ʔ/</td>
      <td>’</td>
      <td><span lang="ms-Arab">داتو<span style="color:red;">ء</span></span></td>
      <td>dato<span style="color:red;">’</span></td>
      <td>/da.to<span style="color:red;">ʔ</span>/</td>
    </tr>
    <tr>
      <td rowspan="4"><span lang="ms-Arab">ي</span></td>
      <td rowspan="4">Ya</td>
      <td rowspan="4">U+064A</td>
      <td rowspan="4">Arabic letter yeh</td>
      <td>/j/</td>
      <td>y</td>
      <td><span lang="ms-Arab">وا<span style="color:red;">ي</span>ر</span></td>
      <td>wa<span style="color:red;">y</span>ar</td>
      <td>/wa.<span style="color:red;">y</span>ar/</td>
    </tr>
    <tr>
      <td>/i/</td>
      <td>i</td>
      <td><span lang="ms-Arab">ت<span style="color:red;">ي</span>ڠݢ<span style="color:red;">ي</span></span></td>
      <td>t<span style="color:red;">i</span>ngg<span style="color:red;">i</span></td>
      <td>/t<span style="color:red;">i</span>ŋ.g<span style="color:red;">i</span>/</td>
    </tr>
    <tr>
      <td>/e/</td>
      <td>e (é)</td>
      <td><span lang="ms-Arab">مر<span style="color:red;">ي</span>ک</span></td>
      <td>mer<span style="color:red;">e</span>ka</td>
      <td>/mə.r<span style="color:red;">e</span>.ka/</td>
    </tr>
    <tr>
      <td>/ɛ/</td>
      <td>e (é)</td>
      <td><span lang="ms-Arab">ب<span style="color:red;">ي</span>ݢ</span></td>
      <td>b<span style="color:red;">e</span>g</td>
      <td>/b<span style="color:red;">ɛ</span>g/</td>
    </tr>
    <tr>
      <td><span lang="ms-Arab">ڽ</span></td>
      <td>Nya</td>
      <td>U+06BD</td>
      <td>Arabic letter noon with three dots above</td>
      <td>/ɲ/</td>
      <td>ny</td>
      <td><span lang="ms-Arab"><span style="color:red;">ڽ</span>ا<span style="color:red;">ڽ</span>ي</span></td>
      <td><span style="color:red;">ny</span>a<span style="color:red;">ny</span>i</td>
      <td>/<span style="color:red;">ɲ</span>a.<span style="color:red;">ɲ</span>i/</td>
    </tr>
    <tr>
      <td rowspan="2"><span lang="ms-Arab">ى</span></td>
      <td rowspan="2">Ye / Alif maqsurah</td>
      <td rowspan="2">U+0649</td>
      <td rowspan="2">Arabic letter alef maksura</td>
      <td>/ə/</td>
      <td>e (ĕ)</td>
      <td><span lang="ms-Arab">ناسيوناليسم<span style="color:red;">ى</span></span></td>
      <td>nasionalism<span style="color:red;">e</span></td>
      <td>/na.sjo.na.lis.m<span style="color:red;">ə</span>/</td>
    </tr>
    <tr>
      <td>/a/</td>
      <td>a</td>
      <td><span lang="ms-Arab">فتو<span style="color:red;">ى</span></span></td>
      <td>fatw<span style="color:red;">a</span></td>
      <td>/fat.tw<span style="color:red;">a</span>/</td>
    </tr>
    <caption style="text-align:center;font-size:0.75em">
      Modern Jawi alphabet as defined by <a href="https://en.wikipedia.org/wiki/Dewan_Bahasa_dan_Pustaka">Dewan Bahasa dan Pustaka</a>, the government body responsible for coordinating the use of the Malay language and Malay-language literature in Malaysia.
    </caption>
  </table>
  
# Localization guide

This guide will help you to translate Waltheri's go pattern search into your language. It is preferred to use GitHub and its features to manage translations. You will need GitHub account for it. However I will survive, if you send me files on email thebestgoplayer@gmail.com.

## Add translations

1) Click on **New file** button in top right corner of this page.

2) Put content of [en.hson](https://github.com/waltheri/go-pattern-search/blob/master/i18n/en.hson) into the new file and translate all text strings between brackets `"` into your language. Name of the new file should be **[lang_code].hson**, where **[lang_code]** stands for [ISO 639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) code of your language.

3) When your translation file is ready, continue with **Propose new file** and then click on **Create pull request** button. It is not necessary to fill any description or comment.

4) And that should be it. I will get notified and upload the translation on the pattern search.

## Edit translations

1) On this page select translation file you want to edit and open it.

2) Click on the pencil in top right corner (Fork this project and edit the file).

3) Edit the file, save changes and continue with  **Create pull request**.

## Translation guidelines

* Don't translate texts literally - texts should feel as naturally as possible in your language.
* Feel free to edit English file as well to improve English and fix typos.
* If you want to use characters `"` or `\` you have to use their escaped form `\"` or `\\`.
* Include name of your language in that language as well (at the top of the file).
 
### Pluralization ###

The pattern search uses [polyglot.js](http://airbnb.io/polyglot.js/) library for localization and it supports pluralization systems of more than 30 languages. For example in Czech, there are three separate forms: 1, 2 through 4, and 5 and up; so  translation string in Czech can look like this `"%{count} (one) |||| %{count} (a few) |||| %{count} (a lot)"`. German on the other side has only two plural form, so translation string will look like this `"%{count} (one) |||| %{count} (two or more)"`. Of course this only matters if there is some number to display. 

---
title: Localization team
description: A large localization project requires a team that consists of a program manager, one or more localization engineers, and many localizers.
ms.assetid: 0516657d-a48c-4e0c-968c-61308a866eb3
ms.date: 03/16/2016
---
# Localization team

A large localization project requires a team that consists of a program manager, one or more localization engineers, and many localizers.
The program manager should coordinate between the development team and the localization team, making sure that developers use code practices that are conducive to localization.
(For more information on these practices, see [Localization introduction](overview.md).)
The program manager should also deal with the external teams that do localization and, of course, manage the internal localization process.

Localization engineers are responsible for handling the localization database and maintaining the proper localization instructions in the commenting model, if this model exists.
For standardization purposes, localization engineers should prepare localizability and localization guidelines for the different product teams to educate them about the localization process.
In addition, they need to make sure that localizers have enough information to translate the string resources correctly.
Once localization is complete, localization engineers also need to verify that the localization instructions were implemented.
Localizers translate strings and make other localization changes such as changing the layout of the user interface, localizing graphics and multimedia, adapting the build process, and redesigning packaging.
Since technical experience is such an integral part of localization, localizers should possess technical resources in addition to language skills.

Localizing an operating system or complex software project is somewhat different from translating literature.
While translating literature requires more-than-excellent language skills, the localization of an operating system definitely requires extensive knowledge about the product and related fields in addition to some solid language skills in both the source and target language.
It's hard to translate a sentence like "Precreate CR for domain %s1 (a DN) allowing server %s2 (a full DNS name) to dcpromo." when you have no idea at all what a CR or DN could possibly be.
Thus, a Ph.D. in linguistics is not necessarily the right qualification for this kind of task (though it probably helps to produce grammatically correct sentences in the target language).
Without some in-depth knowledge of the product, a localizer may not be able to make sense of the source text, and thus won't be able to translate the text adequately in the target language.
The technical level, however, can vary widely.
For the localization of a rich application or an operating system, technical skills and knowledge of the product are essential.
On the other hand, for the localization of a children's game that contains a lot of spoken text, language skills are much more important and there's still enough time to get familiar with the product while working on it.

Comprehensive understanding of the source text, however, is only one reason why technical skills are as important as language skills for localization.
The localizable resources of a product are extracted from the resource files and are imported into a localization database.
At the very least, the resources are placed into some kind of tabular format to make them accessible to localization.
As a result, the individual resources are usually localized without any indication of the context or how they are used in the actual product at run time.
Since the translation in many cases and in many languages can vary widely depending on the context, it is important for the localizer to know how a string is used in the product and what the context is.
If the surrounding strings don't provide any clues, the only way to find out how the text is actually used at run time is to install the original-language product and click through the application until the string shows up.
Particularly in the case of error messages, that might be not an easy task, since a certain scenario has to be reproduced in order to bring up the error message.

A localizer with the appropriate technical skills will be able to correctly perform the fundamental task of translating functionality-sensitive content; this accuracy is crucial, since a mistranslation could break the product.
**Commenting** supplies localizers with valuable information to prevent functionality from breaking.
For example, comments can provide information about the maximum allowed string length.
The localizer should heed these instructions and should avoid exceeding this limit to prevent buffer overrun.
Strings that are blocked from localization must remain untranslated.
There might be special localization instructions to change certain functionality-sensitive strings in accordance with the target language.
For example, a font name that exists in the translation table and that is used to display text on application dialog boxes needs to be translated according to the conventions used in the target language.
The technical localizer will know which font name to use for a specific language or locale.
The same will apply to other string types like font sizes, locale values, and locale-specific file names.

Likewise, the localizer needs to be able to test the localized product in order to check if the translations are appropriate.
Consistent translation lookup tables are useful to ensure correct translation of the text that has content dependency.
These lookup tables can be created as part of the localization process and can be reviewed after translation is finished.

In addition to using good tools and having localization team members who perform defined functions, you should also have some basic process guidelines in place that will enable localization to run smoothly.


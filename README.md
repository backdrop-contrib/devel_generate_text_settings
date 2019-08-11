Devel Generate Text Settings
============================

This module allows you to control the length and format of generated content
for text and long text fields. This only applies to generation of node content
for now.



Installation
------------

- Install as normal
- After enabling you will find additional settings at the bottom of the
"Devel Generate > Generate content" form.

Instructions
------------

Two new fields will be added to the bottom of the 
"Devel Generate > Generate content" form:

**Prefix for title values**

If set, this value will be prepended to the auto-generated node title.

**Text field settings**

Controls the length and format of generated content for text and long text fields.
- Configure one field per line
- If the min and max are the same, that exact value will be used
- Set the fifth parameter to "true" to use title formatting (capital words, no punctuation) - only works with char and word counts
- Format: field_machine_name, count_type, min, max, treat_as_title

**Examples:** (for Text field settings)

*Between 100 and 250 characters, with sentences:*

field_blog_preview, char, 100, 250

*Between 3 and 7 words, no sentences, all words start with capital letter:*

field_program_name, word, 3, 7, true

*One paragraph, with sentences:*

body, para, 1, 1


License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.

Maintainers
-----------

This module is seeking maintainers.

Originally written for Drupal by

- Adam Courtemanche (https://www.drupal.org/u/agileadam)

Ported to Backdrop CMS by

- Docwilmot (https://www.github.org/docwilmot
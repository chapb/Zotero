

# Zotero

Zotero is a free and open-source reference management software. 

[Quick Start Guide](https://www.zotero.org/support/quick_start_guide)

This document describes some Zotero best-practices assembled from the Zotero [documentation](https://www.zotero.org/support/) and Zotero [forums](https://forums.zotero.org/discussions). This is not a complete user guide -- some familarity with the application is useful before addressing the best-practices. See guides below.

- [Zotero](#zotero)
  - [Why Zotero?](#why-zotero)
  - [Zotero Guides](#zotero-guides)
- [Application Configuration](#application-configuration)
  - [File Management](#file-management)
    - [TLDR](#tldr)
    - [File/Attachment Types](#fileattachment-types)
    - [Application Paths](#application-paths)
    - [File Management Approaches](#file-management-approaches)
      - [Use Zotero Storage](#use-zotero-storage)
      - [Use Linked Attachments](#use-linked-attachments)
    - [Copy all PDF's in Zotero Storage to a single folder](#copy-all-pdfs-in-zotero-storage-to-a-single-folder)
  - [Profiles](#profiles)
    - [Using multiple profiles](#using-multiple-profiles)
      - [How do I move a profile?](#how-do-i-move-a-profile)
      - [How do I open multiple instances?](#how-do-i-open-multiple-instances)
  - [Extensions](#extensions)
- [Library Best Practices](#library-best-practices)
  - [Data](#data)
    - [Use Rich Text in Titles](#use-rich-text-in-titles)
    - [Store Titles in Sentence-Case](#store-titles-in-sentence-case)
    - [Use Extra Fields](#use-extra-fields)
    - [Handle Journal Abbreviations](#handle-journal-abbreviations)
  - [Manage Objects](#manage-objects)
    - [Duplicates](#duplicates)
    - [Tag Multiple Objects at Once](#tag-multiple-objects-at-once)
  - [Use Groups for Sharing](#use-groups-for-sharing)
    - [Considerations for a Hybrid Library Approach](#considerations-for-a-hybrid-library-approach)
  - [Odds and Ends](#odds-and-ends)
    - [How to Use Short Titles / BibTex Keys](#how-to-use-short-titles--bibtex-keys)
    - [Other Links](#other-links)


## Why Zotero?

- It's free. 
- It's open-source. 
- It's not owned by [Elsevier](https://en.wikipedia.org/wiki/Elsevier). 
- It includes file management. 
- It has browser integrations for chromium-based browsers and Firefox.
- It has office-suite integrations for Microsoft Office and LibreOffice.
- [Zotero Groups](https://www.zotero.org/support/groups).

## Zotero Guides

- https://www.zotero.org/support/quick_start_guide
- https://guides.lib.uoguelph.ca/zotero
- https://uottawa.libguides.com/how_to_use_zotero
- https://guides.lib.berkeley.edu/zotero
- https://www.library.yorku.ca/web/research-learn/citing-your-work-academic-integrity/citations/zotero-vs-mendeley-comparison/






# Application Configuration 

## File Management

Zotero can be used -- and generally *is used* -- [as a file manager](https://www.zotero.org/support/attaching_files) with built-in [file syncing and cloud storage](https://www.zotero.org/support/sync). There are important implications for your library if you choose not to use Zotero's storage.

### TLDR

**TLDR**: I reccommend purchasing a storage subscription if (more likely: when) you exceed the alloted free storage. There are significant benefits of Zotero storage, including large group libraries and simpler workflows. Additionally, your subscription supports the continued development of an open-source project.

### File/Attachment Types

There are two types of attachments (with fairly self-explanatory names) that lend to cooresponding approaches:

- stored files/attachments are stored in Zotero storage
- linked files/attachments are stored in a linked attachment directory

Zotero cannot backup, share, or sync linked attachments. You can use Zotero's local storage with a library > 200 MB in size, without purchasing a Zotero subscription. However, these files will not be syncronized to Zotero's servers, or other computers. It is possible to use a hybrid approach, where only a subset of objects are in Zotero storage.

### Application Paths

There are two important paths (regardless if multiple profiles are used or not):

- the Zotero data directory
  - this also contains /storage, for stored attachments
  - this should not be in cloud storage, as it includes the dataabase
- the Zotero attachment directory
  - this is the folder used for linked attachments

### File Management Approaches

#### Use Zotero Storage

Using a stored files/attachment approach is strongly reccommended. Using a linked attachment approach or hybrid approach introduces so many complexities, that it is not worthwhile in most scenarios.

The primary benefits are:

- simplier workflows
- sharing via (large) group libraries

The primary drawback(s) are:

- cost
- user-unfriendly storage structure
  

#### Use Linked Attachments

Usimg a linked attachment approach with your own backup, sync, and sharing solutions is fesible, but not reccommended unless absolutely necessary to keep costs at zero.

The primary benefits are:

- no cost
- flat storage structure
- sharing via cloud storage provider (e.g. share link in Dropbox/OneDrive)

The primary drawback(s) are:

- workflow implications
- coarse sharing; access to the cloud storage folder shares your entire library

There are two significant interruptions to the standard workflow when using linked attachments:

- Usually (when using Zotero storage), adding .PDFs to Zotero is a simple drag-and-drop operation. When using a linked attachment approach, this becomes ctrl+shift drag-and-drop. In addition, if the object is added from outside the linked attachment directory, you must ensure a rename and move operation is run to import the PDF into the directory.
- When copying an object with a linked attachment to a Zotero group, the object must first be converted to a stored attachment, then copied, then the object must be reverted to a linked attachment. 


### Copy all PDF's in Zotero Storage to a single folder

TODO



## Profiles

Upon installation and first-run, Zotero will create a default profile. A profile stores application settings; you will need one profile per Zotero account. 

### Using multiple profiles

To [use multiple profiles](https://www.zotero.org/support/kb/multiple_profiles) (i.e. use multiple Zotero accounts on one computer), we start Zotero with the `-P` flag. This launches the profile manager. 

The [default profile path](https://www.zotero.org/support/kb/profile_directory) is specified in Zotero's documentation. A `profiles.ini` file is created in this directory. 

The format is self-explanatory:

```
[Profile#]                                # Where # is a sequential number zero-indexed
Name=ProfileName                          # The profile name as it will appear in the profile manager.
IsRelative=0                              # 1 if path is relative to the profile.ini file
Path=C:\path\to\directory                 # The path to the profile directory. 

# Spaces in the path seem acceptable with no special handling.
```

#### How do I move a profile?

You can edit the contents of profiles.ini to add or move a profile directory.


#### How do I open multiple instances?

To launch a second instance, you can use the `-no-remote` command line option. However, this is counter-indicated in some articles.



## Extensions

- http://zotfile.com/
- https://github.com/jlegewie/zotfile
- https://github.com/wshanks/Zutilo





# Library Best Practices

## Data

### Use Rich Text in Titles

Zotero supports [rich text formatting in titles](https://www.zotero.org/support/kb/rich_text_bibliography). You can apply rich text formatting by adding the following HTML-like tags in the title field:

```
- <i> and </i> for italics
- <b> and </b> for bold
- <sub> and </sub> for subscript
- <sup> and </sup> for superscript
- <span style="font-variant:small-caps;"> and </span> for smallcaps
- <span class="nocase"> and </span> to suppress capitalization rules 
  - (e.g., for foreign phrases within English titles)
```
>Zotero will automatically replace these tags by the specified formatting in bibliographic output. E.g. “<i>Pseudomonas aureofaciens</i> nov. spec. and its pigments” will become “*Pseudomonas aureofaciens* nov. spec. and its pigments”.

>Note that if rich text formatting has to be applied indiscriminately to entire fields (e.g. a style guide may dictate that titles should be in italics), you can modify the relevant Citation Style Language (CSL) style (see the CSL documentation and the CSL field formatting options).

### Store Titles in Sentence-Case

Just do it. You can automatically capitalize all words (with easy exception) later if neccessary (why thou?). You cannot do the inverse.


### Use Extra Fields

If a Zotero item type is missing one or more required fields, it is possible to add these fields using the Extra field. 

From the [documentation](https://www.zotero.org/support/kb/item_types_and_fields):

Enter each variable on a separate line at the top of the Extra field in the following format: `CSL Variable: Value`. For example:

```
DOI: 10.1128/AEM.02591-07
Original Date: 1824
PMCID: PMC3531190
```

With the exception of Item Type (CSL Type) and Date variables (CSL Issued, etc.), variables entered in Extra will not override corresponding values entered in proper Zotero fields. There are specific considerations for dates and names; see the documentation for more details.


### Handle Journal Abbreviations

> Journal articles are often cited with the abbreviated journal title. Zotero stores the journal title and journal title abbreviation in separate fields (“Publication” and “Journal Abbr”, respectively). There is no automatic abbreviation of journal titles.

> While some citation styles require different abbreviations, most of the variation is in whether or not the abbreviation contain periods (e.g., “PLoS Biol” or “PLoS Biol.”). Because removing periods is more accurate than adding them, we recommend that you store title abbreviations in your Zotero library with periods. Zotero can then reliably strip out the periods in rendered bibliographies when the chosen citation style calls for it. 


## Manage Objects

### Duplicates

To remove duplicates, use the Duplicate Items folder to identify candidates, and merge them after reviewing meta-data. **Note, the folder structure will be preserved; if duplicate references are in different folders, this organization will be mainatined after de-duplication**. 


### Tag Multiple Objects at Once

To tag multiple items, you can drag them onto the tag in the *tags pane* (in the lower-left corner). If no tags exist, none will be shown - tag one item first, then add the tags to all items.



## Use Groups for Sharing

### Considerations for a Hybrid Library Approach

Some users may use a hybrid-library approach, where some objects are in storage (e.g. group libraries) and some are linked (e.g. personal library). Groups do not support linked attachments. **When a linked-attachment object is copied to a group library, the attachment is silently removed**.

If you have copied a large number of objects and lost many attachments, one option is delete and start over. If you've made changes to the library you do not want to lose, you can (in the personal library) convert all linked attachments to stored attachments, and then copy them over, merging via duplicate detection.


## Odds and Ends

### How to Use Short Titles / BibTex Keys

- https://forums.zotero.org/discussion/80810/is-there-a-way-to-fill-in-the-short-title-automatically


### Other Links

- https://forum.obsidian.md/t/zotero-best-practices/164/57
- https://felix11h.github.io/blog/zotero-zotfile-config

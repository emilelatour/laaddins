
laaddins
--------

Additional Addins for RStudio

### Description

I'm a really big fan of some of the RStudio Addins. Most notable: [datapasta](https://github.com/MilesMcBain/datapasta), [clipr](https://github.com/daattali/addinslist), and [snippetsaddins](https://github.com/sfr/RStudio-Addin-Snippets). There are so many other greats ones but I use these over and over. The most comprehensive list can be found at the [addinslist](https://github.com/daattali/addinslist). A cool thing with Addins is that you can assign them to Keyboard Shortcuts.

As I write code in R, some things I type repetitively. Especially as I style and commment my code. I created these Addins to turn some of those things into keyboard shortcuts. I did pretty much the same thing using RStudio [snippets](https://support.rstudio.com/hc/en-us/articles/204463668-Code-Snippets), but this project gave me the personal benefit of learning about Addins.

Inspiration from

-   [RStudio Addins](https://github.com/rstudio/addinexamples)
-   [hrbraddins](https://github.com/hrbrmstr/hrbraddins)
-   [datapasta](https://github.com/MilesMcBain/datapasta)

### What's in the box?

-   `insertBigBreakAddin`: Inserts the text that I use when I am coding and want to indicate a big section break.
-   `insertLittleBreakAddin`: Inserts the text that I use when I am coding and want to indicate a little section break.

Once installed, in RStudio, I navigate to Tools &gt; Modify keyboard shortcuts, and make the following assignments

-   `Ctrl+Alt+B` for the Big Break, and
-   `Ctrl+Alt+L` for the Little Break

Not sure if these conflict with other keyboard shortcuts (as of 2018-05-03).

### Examples

#### `insertBigBreakAddin`

Inserts the following text into your code:

``` r
#### ----------------------------
```

Then type a title or header for that section

``` r
#### Section One -------------------------------

# Sections are separated visually with 4 comment characters and 32 dashes


# The last 4 dashes at the end of the comment are a section marker supported by
# RStudio
```

#### `insertLittleBreakAddin`

Inserts the following text into your code:

``` r
## ---------------- 
```

Combined with the Big Section Break code is organized like so

``` r

#### Section One -------------------------------

# Sections are separated visually with 4 comment characters and 32 dashes

## Sub-section One ----------------

# Subsection with 2 comment characters and 16 dashes


# The last 4 dashes at the end of the comment are a section marker supported by
# RStudio
```

Installation
------------

``` r
devtools::install_github("emilelatour/laaddins")
```

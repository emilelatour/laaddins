# laaddins
Additional Addins for RStudio

## Description

I'm a really big fan of some of the RStudio Addins. Most notable: [datapasta](https://github.com/MilesMcBain/datapasta), [clipr](https://github.com/daattali/addinslist), and [snippetsaddins](https://github.com/sfr/RStudio-Addin-Snippets). There are so many other greats ones but I use these over and over. The most comprehensive list can be found at the [addinslist](https://github.com/daattali/addinslist).

The cool thing is that you can assign Addins to Keyboard Shortcuts. There are some things that I type over and over again and I really just want to make my life easier (general goal not just an R related one), so I followed some others examples and created my own Addins.

Inspiration from 

- [RStudio Addins](https://github.com/rstudio/addinexamples)
- [hrbraddins](https://github.com/hrbrmstr/hrbraddins)
- [datapasta](https://github.com/MilesMcBain/datapasta)


## What's in the box?

- `insertBigBreakAddin`: Inserts the text that I use when I am coding and want to indicate a big section break.
- `insertLittleBreakAddin`: Inserts the text that I use when I am coding and want to indicate a little section break.

Once installed, in RStudio, I navigate to Tools > Modify keyboard shortcuts, and make the following assignments

- `Ctrl+Alt+B` for the Big Break, and 
- `Ctrl+Alt+L` for the Little Break

Not sure if these conflict with other keyboard shortcuts (as of 2018-05-03).

## Examples

### `insertBigBreakAddin`

Just inserts the following text into your code:

```
#### ----------------------------
```
Then I will type a title or header for that section

```
#### Here's a big ol' section break ----------------------------
```

### `insertLittleBreakAddin`

Just inserts the following text into your code:

```
## ---------------- 
```
Combined with the Big Section Break my code is organized like so

```
#### Big section break -------------------------------- 

# Here is where I start to work on something that is very different than the
# work that came before

## Little section break ---------------- 

# This section still is worth an indicator that it is separate from what came
# before, but not so different from what I am currently working on that it
# warrants another Big Break
```

## Installation

```{r eval=FALSE}
devtools::install_github("emilelatour/laaddins")
```

# Changes in this update

# HMDHFDplus 2.0.6
21 January 2025
* minor change to DESCRIPTION to comply w CRAN.
* Fixes minor OpenInterval coding error for HFD denominators. HT @alysonvanraalte

# HMDHFDplus 2.0.5
07 July 2024
* `getHFDdate()` modified to pull date from country page footer rather than from table dates. The HFD website sometimes has inconsistent labeling of last update dates, leading to url failures unless we get the date right. Page footer was consistent with file urls so far.

# HMDHFDplus 2.0.4
25 July 2023
* `getHMDitemAvail()` now fixed HT @samhyunyoo

# HMDHFDplus 2.0.3
20 June 2023
* removes `closeAllConnections()` from all functions. HT mbs2016
* `readHFCweb()` temporarily deprecated due to source website upgrade. This function will be reintroduced in the future.

# HMDHFDplus 2.0.2
24 March 2023
* `getHMDcountries()` adds in HMD subpopulations that weren't scraped from the main page

# HMDHFDplus 2.0.0
1 Feb 2023

* `getHMDcountries()` adapted to the new HMD website
* `getJMDprefectures()` refactored, now returns `tibble` object instead of named vector
* `readHMDweb()` refactored ro work with new HMD website and new HMD credentials, HT Markus Sauerberg for Python example
* `getHMDitemavail()` adapted to the new website and now returns an informative table
* `getHMDcountries()` adapted to new HMD website


# HMDHFDplus 1.9.19
5 November 2022

* `getHFDdate()` adapted to the new HFD website
* `getHFDcountries()` adapted. Now rather than a vector of codes we return a tibble with more information per source.
* `getHFDitemavail()` adapted. Now rather than a vector of items, we return an informative table of all available files for the given country with lots of metadata that might help a user figure out what file is needed.
* `extract_HFD_items()` removed.
* `readHFDweb()` refactored to authenticate and grab from the new HFD website. The old HMD mirror site will no longer be accessed as of this update, so users may need to re-register at the HMD.
* `getHFDitemavail()` now returns an informative table
* 

# HMDHFDplus 1.9.18
16 June 2022

* `readHMDweb()` and related functions now temporarily point 
   to a new url to grab data: `https://former.mortality.org`. This
   is a patch until a new API will be released.

# HMDHFDplus 1.9.16
22 December 2021

* `readJMDweb()` adapted to changing website specifications
* `readHFCcountries()` fixed
* `readHFDweb()` adapted to changing website specifications
* `getJMDprefectures()` fixed

# HMDHFDplus 1.9.14
7 April 2021

* `HMDparse()` handles territorial adjustments properly now. HT Jim Oeppen

# HMDHFDplus 1.9.13
20 Feb 2020.

*  `readHFDweb()` documentation Warning fixed.
*  incomplete url NOTE fixed

# HMDHFDplus 1.9.1
9 Aug 2018.  

*  `readHFDweb()` fixed, now relies on `hhtr` HT @jasonhilton
*  `readHMDweb()` fixed, now relies on `httr`





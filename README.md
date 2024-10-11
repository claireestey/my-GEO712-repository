
# Claire Estey’s GEOG 712 Repository

------------------------------------------------------------------------

This README document is for my first repository in GEOG 712. Within the
repository, the file organization is as follows:

| File Name    | Contents                                     |
|--------------|----------------------------------------------|
| **data_raw** | raw, unprocessed data saved as .csv files    |
| **data**     | manipulated data saved as .csv files         |
| **figures**  | saved figures and plots I generate           |
| **images**   | .jpg files to be inserted into the documents |
| **tables**   | saved output tables I generate               |

# My Research Interests

------------------------------------------------------------------------

For my MSc research, I am looking at the effects of **quaternary
ammonium compounds** (QACs) on the diversity, community composition, and
reproductive rates of freshwater zooplankton. Zooplankton are
micro-crustaceans that live pelagically in the water column of lakes and
oceans, typically feeding on phytoplankton or other zooplankton. QACs
are a class of high-production volume chemicals that have a wide variety
of uses, including as anti-static agents, disinfectants, and
emulsifiers. The QAC I study in particular is called **benzalkonium
chloride** (BAC) and is a potent antimicrobial compound. It’s use since
the onset of the COVID-19 pandemic has increased *drastically*,
resulting in concerning levels being found in our freshwater systems,
with unknown effects on aquatic biota.

``` r
knitr::include_graphics(paste0(here(), "/images/bosmina.jpg"))
```

![](images/bosmina.jpg)<!-- -->

*Bosmina sp.*, a crustaceous zooplankton commonly found in Boreal lakes.

# Favourites

------------------------------------------------------------------------

## Favourite Music

My five favourite songs are as follows:

1.  *Jackie and Wilson* by Hozier
2.  *August* by flipturn
3.  *Heat Above* by Greta Van Fleet
4.  *And She Was* by Talking Heads
5.  *Going Gets Tough* by The Growlers

``` r
knitr::include_graphics(paste0(here(), "/images/albums.jpg"))
```

![](images/albums.jpg)<!-- -->

## Favourite Equation

My favourite equation is the Inverse Simpson Index ($^2D$, where $S$ is
species richness and $p_i$ is the proportion of individuals belonging to
species $i$) as it is used in my research as a measure of zooplankton
community diversity:

$$
^2D = \frac{1}{\sum_{i=1}^S(p_i)^2}
$$

## Favourite Artists

| Name                   | Achievements                                                                                                                                        |
|------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| **Georgia O’Keefe**    | Celebrated early twentieth century painter focusing on desert landscapes and animal skulls.                                                         |
| **Tim Gardner**        | Pastel and oil painter creating hyper-realistic depictions of everyday life in North America.                                                       |
| **Ai Weiwei**          | Contemporary artist, sculptor, and human rights activist most known for the controversial photography pieces titled *“Dropping a Han Dynasty Urn”*. |
| **Lawren Harris**      | Original Group of Seven member known for stunning Canadian landscape paintings.                                                                     |
| **Auguste Toulmouche** | Widely known nineteenth century painter and creator of one of my favourite paintings, *“The Hesitant Fiancee”*.                                     |

``` r
knitr::include_graphics(paste0(here(), "/images/hesitant_fiancee.jpg"))
```

![](images/hesitant_fiancee.jpg)<!-- -->

# A Chunk of Code

------------------------------------------------------------------------

``` r
x <- c(1, 2, 3, 4)
y <- c(1, 2, 3, 4)

plot(x, y, xlab = "Months Enrolled in GEOG 712", ylab = "The Reproducibility of My Research", type = "l")
```

![](README_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->

# Project Data Analysis

------------------------------------------------------------------------

**List of data I have collected for my project:**

1.  Water Chemistry: Weekly YSI water quality measurements (dissolved
    oxygen, chlorophyll *a*, pH, specific conductance, water
    temperature)
2.  BAC Analytical Samples: Water grab samples on days 0, 1, 2, 4, 7,
    and 75 to determine actual concentration of BAC and percentage of
    homologs present.
3.  Zooplankton samples from each enclosure on days 0, 14, 35, 56, and
    77 taken with a 15 L Schindler-Patalas plankton trap.
4.  Site metadata (date, time of collection, coordinates, name of person
    sampling, relevant notes)

With this data I will be looking at the zooplankton community
composition and reproductive rates. I will be using the Inverse Simpson
Index to assess diversity, and generating principal response curves to
look at changes in diversity independent of temporal trends.

**Legal and ethical restrictions:**

The main consideration while collecting this data is handling large
amounts of BAC in order to spike the enclosures to the desired
concentrations. Permission has been granted by ELA’s Research Advisory
Board (RAB) to transport pre-portioned volumes of BAC to the field to be
added to the enclosures. No mixing of the chemical to reach the desired
concentration is allowed in the field and must be done in ELA’s
chemistry lab prior to transporting to the field.

**Quick Hits for Data Management**

Raw data will be kept in the *data_raw* folder within the repository, to
be saved locally on a hard drive as well as backed up to GitHub. Raw
data is also in a shared Microsoft Teams folder with my supervisor.

To keep file formats open, spreadsheets are saved as .csv files, word
documents and power point presentations are saved as .pdf files (or .txt
in the case of word docs).

Snake case will be used for naming files
(this_is_an_example_of_snake_case) to eliminate the inconsistencies of
capitalization and special characters. Names will be specific (for
example, zooplankton_raw_counts.csv instead of my_data.csv).

Relevant standards for zooplankton collection include using a plankton
trap with a standardized mesh size (53 microns) to allow data between
sites and studies to be comparable. Standardized methods also exist for
identifying and counting zooplankton and should be used for all ELA
projects to keep data consistent between years, as well as between a
reference lake and an experimental lake (for example, community
composition can only be reliable if a minimum of 300 adults has been
reached). ELA also has standardized data storage requirements for its
researchers, and does this by creating collaborative projects on GitHub.

To document my data throughout my project, I will not only keep the raw
data raw (i.e. save manipulated data sets in a separate folder while
keeping the raw data intact), but I will create a GitHub repository so
that every version of my data will be available, even after I have made
changes.

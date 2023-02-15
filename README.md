# danebadawczeuw-extension
danebadawczeuw extensions that can plugged into dataverse instance 

## danebadawczeuw theme

Theme files can be found under `src/main/theme` directory.
The main file that is taken as the theme file is `theme.css` and it should `@import "theme-base.scss"` to extend it.

> Note that scss compiler requires the original theme files, so Maven will copy them for you during build,
> then copy over danebadawczeuw files possibly overriding original ones and run the compiler on the result. 
> Everything is done automatically during Maven build, just be aware when adding files that you can use
> and overwrite files from `resources/velcer` directory.

## Logo customization

For the superior and main logo to be properly displayed, these values need to be set in `dataverse.properties`:

```
SiteName=Dane Badawcze UW
SiteFullName=R e p o z y t o r i u m
SiteFullName.pl=R e p o z y t o r i u m

SuperiorLogoLink=https://en.uw.edu.pl
SuperiorLogoLink.pl=https://www.uw.edu.pl
SuperiorLogoPath=/images/superior-logo/logo-uw-en.png
SuperiorLogoPath.pl=/images/superior-logo/logo-uw-pl.png
SuperiorLogoResponsivePath=/images/superior-logo/logo-uw-en-responsive.png
SuperiorLogoResponsivePath.pl=/images/superior-logo/logo-uw-pl-responsive.png
SuperiorLogoContrastPath=/images/superior-logo/logo-uw-en-contrast.png
SuperiorLogoContrastPath.pl=/images/superior-logo/logo-uw-pl-contrast.png
SuperiorLogoContrastResponsivePath=/images/superior-logo/logo-uw-en-contrast-responsive.png
SuperiorLogoContrastResponsivePath.pl=/images/superior-logo/logo-uw-pl-contrast-responsive.png
SuperiorLogoAlt=Warsaw University website
SuperiorLogoAlt.pl=Witryna Uniwersytetu Warszawskiego
```

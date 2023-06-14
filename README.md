# WSU-DAESA-CSS-WDS
This is a front-end development project for producing CSS source files used on the websites of the [Division of Academic Engagement and Student Achievement (DAESA)](https://daesa.wsu.edu/) at Washington State University which are running the [Web Design System (WDS) theme](https://github.com/wsuwebteam/wsuwp-theme-wds) in WSU WordPress. This project is designed to produce CSS for deployment to websites through the following modalities:

- WSUWP theme's CSS Stylesheet Editor interface working in add-on mode.
- Theme customizer's additional CSS panel for WordPress users with a network admin permissions level.

Style rules in this project are written in the [Less language extension of CSS](https://lesscss.org/#overview) and intended to be compiled into CSS using [Gulp workflow automation](https://gulpjs.com/) and the [gulp-less plugin for Gulp](https://github.com/gulp-community/gulp-less). It is assumed that this project will be incorporated into other front-end development projects as a submodule so that developers can combine its code with code from their own source files.

## Design Approach
The style rules written for this project are organized into folders and Less modules generally structured around the elements, components, and modules that make up the [WSU WDS](https://github.com/wsuwebteam/web-design-system). Style rules are written in blocks of code labeled by a persistent CSS comment, with each code block designed to impart one of three effects on a particular WDS element, component, or module:

- Fix a (typically minor) technical or design issue that remains unaddressed in the stylesheets packaged with the WDS theme.
- Impart an enhancment to the default layout or presentation of a WDS element, component, or module.
- Provide a customization whereby:
  - An existing WDS element, component, or module can be presented in a significantly different and novel manner.
  - A novel element, component, module, or assembly of WordPress Gutenberg blocks not included in the WDS can be presented on a WDS themed website hosted on WSU WordPress.
- Extend WDS stylesheets with additional utility classes.

By using this approach, modules can quickly be dropped or added when building a CSS stylesheet for deployment to a website. This enables the custom code from this project to be easily adapted in response to ongoing changes to the WDS theme as it continues to be developed and evolve.

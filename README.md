# jekyll-theme-cayman

Usage

To use the Cayman theme:

    Add the following to your site's _config.yml:


           theme: jekyll-theme-cayman



    Optionally, if you'd like to preview your site on your computer, add the following to your site's Gemfile:

         
            gem "github-pages", group: :jekyll_plugins



Customizing
Configuration variables

Cayman will respect the following variables, if set in your site's _config.yml:

title: [The title of your site]
description: [A short description of your site's purpose]

Additionally, you may choose to set the following optional variables:

show_downloads: ["true" or "false" to indicate whether to provide a download URL]
google_analytics: [Your Google Analytics tracking ID]

Stylesheet

If you'd like to add your own custom styles:

    Create a file called /assets/css/style.scss in your site
    Add the following content to the top of the file, exactly as shown:

    ---
    ---

    @import "{{ site.theme }}";

    Add any custom CSS (or Sass, including imports) you'd like immediately after the @import line


Previewing the theme locally

If you'd like to preview the theme locally (for example, in the process of proposing a change):

    Clone down the theme's repository (git clone https://github.com/pages-themes/cayman)
    cd into the theme's directory
    Run script/bootstrap to install the necessary dependencies
    Run bundle exec jekyll serve to start the preview server
    Visit localhost:4000 in your browser to preview the theme

Running tests

The theme contains a minimal test suite, to ensure a site with the theme would build successfully. To run the tests, simply run script/cibuild. 
You'll need to run script/bootstrap once before the test script will work.

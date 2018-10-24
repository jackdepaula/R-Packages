R Packages
================

R Packages
----------

<table>
<colgroup>
<col width="2%" />
<col width="6%" />
<col width="68%" />
<col width="22%" />
</colgroup>
<thead>
<tr class="header">
<th>Package</th>
<th>Category</th>
<th>Description</th>
<th>Sample Use</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>slackr</td>
<td>collaboration</td>
<td>Do you use Slack? If so, you can send messages and files into a Slack channel, as long as you've got a token from that Slack. Useful to run analysis and then quickly share results with a team. GitHub hrbrmstr/slackr</td>
<td>See the GitHub repo .</td>
</tr>
<tr class="even">
<td>Hmisc</td>
<td>data analysis</td>
<td>There are a number of useful functions in here. Two of my favorites: describe, a more robust summary function, and Cs, which creates a vector of quoted character strings from unquoted comma-separated text. Cs(so, it, goes) creates c(&quot;so&quot;, &quot;it&quot;, &quot;goes&quot;). CRAN.</td>
<td>describe(mydf) Cs(so, it, goes)</td>
</tr>
<tr class="odd">
<td>diffobj</td>
<td>data analysis</td>
<td>Base R's identical() function tells you whether or not two objects are the same; but if they're not, it won't tell you why. diffobj gives you a visual representation of how two R objects differ. CRAN.</td>
<td>diffObj(x,y)</td>
</tr>
<tr class="even">
<td>knitr</td>
<td>data display</td>
<td>Add R to a markdown document and easily generate reports in HTML, Word and other formats. A must-have if you're interested in reproducible research and automating the journey from data analysis to report creation. CRAN.</td>
<td>See the Minimal Examples page.</td>
</tr>
<tr class="odd">
<td>officeR</td>
<td>data display</td>
<td>Import and edit Microsoft Word and PowerPoint documents, making it easy to add R-generated analysis and visualizations to existing as well as new reports and presentations. CRAN.</td>
<td>my_doc &lt;- read_docx() %&gt;% body_add_img(src = myplot) The package website has many more examples.</td>
</tr>
<tr class="even">
<td>DT</td>
<td>data display</td>
<td>Create a sortable, searchable table in one line of code with this R interface to the jQuery DataTables plug-in. GitHub rstudio/DT.</td>
<td>datatable(mydf)</td>
</tr>
<tr class="odd">
<td>listviewer</td>
<td>data display, data wrangling</td>
<td>While RStudio has since added a list-viewing option, this HTML widget still offers an elegant way to view complex nested lists within R. GitHub timelyportfolio/listviewer.</td>
<td>jsonedit(mylist)</td>
</tr>
<tr class="even">
<td>plumber</td>
<td>data export, programming</td>
<td>Turn any R function into a host-able API with a line or two of code. This well-thought-out package makes it easy to use R for data handling in other, non-R coding projects. CRAN.</td>
<td>See the documentation or my article Create your own Slack bots -- and Web APIs -- with R</td>
</tr>
<tr class="odd">
<td>readxl</td>
<td>data import</td>
<td>Fast way to read Excel files in R, without dependencies such as Java. CRAN.</td>
<td>read_excel(&quot;my-spreadsheet.xls&quot;, sheet = 1)</td>
</tr>
<tr class="even">
<td>readr</td>
<td>data import</td>
<td>Base R handles most of these functions; but if you have huge files, this is a speedy and standardized way to read tabular files such as CSVs into R data frames, as well as plain text files into character strings with read_file. CRAN.</td>
<td>read_csv(myfile.csv)</td>
</tr>
<tr class="odd">
<td>datapasta</td>
<td>data import</td>
<td>Data copy and paste: Meet reproducible research. If you've copied data from the Web, a spreadsheet, or other source into your clipboard, datapasta lets you paste it into R as an R object, with the code to reproduce it . It includes RStudio add-ins as well as command-line functions for transposing data, turning it into markdown format, and more. CRAN.</td>
<td>df_paste() to create a data frame, vector_paste() to create a vector.</td>
</tr>
<tr class="even">
<td>googleAuthR</td>
<td>data import</td>
<td>If you want to use data from a Google API in an R project and there's not yet a specific package for that API, this is the place to turn for authenticating CRAN.</td>
<td>See examples on the package website and this gist for use with Google Calendars. CRAN.</td>
</tr>
<tr class="odd">
<td>googlesheets</td>
<td>data import, data export</td>
<td>Easily read data from and post data to Google Sheets. While no longer under active development (it will be replaced by the googledrive and googlesheets4 packages), I find the package still works well. CRAN.</td>
<td>mysheet &lt;- gs_title(&quot;Google Spreadsheet Title&quot;) mydata &lt;- mydata &lt;- gs_read(mysheet, ws = WorksheetTitle)</td>
</tr>
<tr class="even">
<td>rio</td>
<td>data import, data export</td>
<td>rio has a good idea: Pull a lot of separate data-reading packages into one, so you just need to remember 2 functions: import and export. CRAN.</td>
<td>import(&quot;myfile&quot;)</td>
</tr>
<tr class="odd">
<td>feather</td>
<td>data import, data export</td>
<td>This binary data-file format can be read by both Python and R, making data interchange easier between the two languages. It's also built for I/O speed. CRAN.</td>
<td>write_feather(mydf, &quot;myfile&quot;)</td>
</tr>
<tr class="even">
<td>fst</td>
<td>data import, data export</td>
<td>Another alternative for binary file storage (R-only), fst was built for fast storage and retrieval, with access speeds above 1 GB/sec. It also offers compression that doesn't slow data access too much, as well as the ability to import a specific range of rows (by row number). CRAN.</td>
<td>write.fst(mydf, &quot;myfile.fst&quot;, 100)</td>
</tr>
<tr class="odd">
<td>cloudyR project</td>
<td>data import, data export</td>
<td>This is a collection of packages aimed at making it easier for R to work with cloud platforms such as Amazon Web Services, Google and Travis-CI. Some are already on CRAN, some can be found on GitHub.</td>
<td>See the list of packages .</td>
</tr>
<tr class="even">
<td>quantmod</td>
<td>data import, data visualization, data analysis</td>
<td>Even if you're not interested in analyzing and graphing financial investment data, quantmod has easy-to-use functions for importing economic as well as financial data from sources like the Federal Reserve. CRAN.</td>
<td>getSymbols(&quot;AITINO&quot;, src=&quot;FRED&quot;)</td>
</tr>
<tr class="odd">
<td>tidyquant</td>
<td>data import, data visualization, data analysis</td>
<td>Another financial package that's useful for importing, analyzing and visualizing data, integrating aspects of other popular finance packages as well as tidyverse tools. With thorough documentation. CRAN.</td>
<td>aapl_key_ratios &lt;- tq_get(&quot;AAPL&quot;, get = &quot;key.ratios&quot;)</td>
</tr>
<tr class="even">
<td>jsonlite</td>
<td>data import, data wrangling</td>
<td>Parse json within R or turn R data frames into json. CRAN.</td>
<td>myjson &lt;- toJSON(mydf, pretty=TRUE) mydf2 &lt;- fromJSON(myjson)</td>
</tr>
<tr class="odd">
<td>XML</td>
<td>data import, data wrangling</td>
<td>Many functions for elegantly dealing with XML and HTML, such as readHTMLTable. CRAN.</td>
<td>mytables &lt;- readHTMLTable(myurl)</td>
</tr>
<tr class="even">
<td>httr</td>
<td>data import, data wrangling</td>
<td>An R interface to http protocols; useful for pulling data from APIs. See the httr quickstart guide . CRAN.</td>
<td>r &lt;- GET(&quot;<a href="http://httpbin.org/get" class="uri">http://httpbin.org/get</a>&quot;) content(r, &quot;text&quot;)</td>
</tr>
<tr class="odd">
<td>rvest</td>
<td>data import, web scraping</td>
<td>Web scraping: Extract data from HTML pages. Inspired by Python's Beautiful Soup. Works well with Selectorgadget. CRAN.</td>
<td>See the package vignette</td>
</tr>
<tr class="even">
<td>ggplot2</td>
<td>data visualization</td>
<td>Powerful, flexible and well-thought-out dataviz package following 'grammar of graphics' syntax to create static graphics, but be prepared for a steep learning curve. CRAN.</td>
<td>qplot(factor(myfactor), data=mydf, geom=&quot;bar&quot;, fill=factor(myfactor)) See my searchable ggplot2 cheat sheet and time-saving code snippets .</td>
</tr>
<tr class="odd">
<td>patchwork</td>
<td>data visualization</td>
<td>Easily combine ggplot2 plots and keep the new, merged plot a ggplot2 object. plot_layout() adds ability to set columns, rows, and relative sizes of each component graphic. GitHub.</td>
<td>plot1 + plot2 + plot_layout(ncol=1)</td>
</tr>
<tr class="even">
<td>ggiraph</td>
<td>data visualization</td>
<td>Make ggplot2 plots interactive with this extension's new geom functions such geom_bar_interactive and arguments for tooltips and JavaScript onclicks. CRAN.</td>
<td>g &lt;- ggplot(mpg, aes( x = displ, y = cty, color = drv) ) my_gg &lt;- g + geom_point_interactive(aes(tooltip = model), size = 2) ggiraph(code = print(my_gg), width = .7).</td>
</tr>
<tr class="odd">
<td>esquisse</td>
<td>data visualization</td>
<td>This RStudio add-in offers a drag-and-drop interface for ggplot2. And, it generates codes for the graph you create with the GUI. It's a useful tool for exploring different color palettes and themes, even if you're comfortable creating your visualizations directly in R. CRAN.</td>
<td>See examples on the project's website .</td>
</tr>
<tr class="even">
<td>dygraphs</td>
<td>data visualization</td>
<td>Create HTML/JavaScript graphs of time series - one-line command if your data is an xts object. CRAN.</td>
<td>dygraph(myxtsobject)</td>
</tr>
<tr class="odd">
<td>googleVis</td>
<td>data visualization</td>
<td>Tap into the Google Charts API using R. CRAN.</td>
<td>mychart &lt;- gvisColumnChart(mydata) plot(Column) Numerous examples here</td>
</tr>
<tr class="even">
<td>metricsgraphics</td>
<td>data visualization</td>
<td>R interface to the metricsgraphics JavaScript library for bare-bones line, scatterplot and bar charts. GitHub hrbrmstr/metricsgraphics.</td>
<td>See package intro</td>
</tr>
<tr class="odd">
<td>taucharts</td>
<td>data visualization</td>
<td>This html widget library is especially useful for scatterplots where you want to view multiple regression options. However, it does much more than that, including line and bar charts with legends and tooltips. GitHub hrbrmstr/taucharts.</td>
<td>See the author's post on RPubs</td>
</tr>
<tr class="even">
<td>RColorBrewer</td>
<td>data visualization</td>
<td>Not a designer? RColorBrewer helps you select color palettes for your visualizations. CRAN. Note: For even more palettes, check out packages viridis for colors that print well in greyscale and are easier to read if you're color blind, pals , rcartcolor for map colors, colorr for sports-team colors, nord for &quot;Northern-themed Color palettes,&quot; and wesanderson for color schemes used by director Wes Anderson.</td>
<td>See Jennifer Bryan's tutorial</td>
</tr>
<tr class="odd">
<td>shiny</td>
<td>data visualization</td>
<td>Turn R data into interactive Web applications. I've seen some nice (if sometimes sluggish) apps and it's got many enthusiasts. CRAN.</td>
<td>See the tutorial</td>
</tr>
<tr class="even">
<td>flexdashboard</td>
<td>data visualization</td>
<td>If Shiny is too complex and involved for your needs, this package offers a simpler (if somewhat less robust) solution based on R Markdown. CRAN.</td>
<td>More info in Using flexdashboard</td>
</tr>
<tr class="odd">
<td>rcdimple</td>
<td>data visualization</td>
<td>R interface to the dimple JavaScript library with numerous customization options. Good choice for JavaScript bar charts, among others. GitHub timelyportfolio/rcdimple.</td>
<td>dimple(mtcars, mpg ~ cyl, type = &quot;bar&quot;)</td>
</tr>
<tr class="even">
<td>plotly</td>
<td>data visualization</td>
<td>R interface to the Plotly JavaScript library that was open-sourced in late 2015. Basic graphs have a distinctive look which may not be for everyone, but it's full-featured, relatively easy to learn (especially if you know ggplot2) and includes a ggplotly() function to turn graphs created with ggplot2 interactive. CRAN.</td>
<td>d &lt;- diamonds[sample(nrow(diamonds), 1000), ] plot_ly(d, x = carat, y = price, text = paste(&quot;Clarity: &quot;, clarity), mode = &quot;markers&quot;, color = carat, size = carat)</td>
</tr>
<tr class="odd">
<td>highcharter</td>
<td>data visualization</td>
<td>R wrapper for the robust and well documented Highcharts JavaScript library, one of my favorite choices for presentation-quality interactive graphics. The package uses ggplot2-like syntax, including options for handling both long and wide data, and comes with plenty of examples. Note that a paid Highcharts license is needed to use this for commercial or government work (it's free for personal and non-profit projects). CRAN. . CRAN.</td>
<td>hchart(mydf, &quot;charttype&quot;, hcaes(x = xcol, y = ycol, group = groupbycol))</td>
</tr>
<tr class="even">
<td>echarts4r</td>
<td>data visualization</td>
<td>R wrapper for the powerful and flexible ECharts JavaScript library. It features dozens of chart and graph types, from bar and line charts to sunbursts, heat maps, and geographical maps. Hundreds of customizations not explicitly mentioned in the package docs are nevertheless available; you just need to peruse the original ECharts documentation . (ECharts is an Apache Software Foundation incubator project.) CRAN.</td>
<td>mtcars %&gt;% e_charts(wt) %&gt;% e_line(mpg)</td>
</tr>
<tr class="odd">
<td>geofacet</td>
<td>data visualization, mapping</td>
<td>To be honest, I rarely need the ability create &quot;geofacets&quot; -- maps with same-sized blocks in geospatially appropriate locations. However, this package is so cool that I had to include it. Geofaceting is best understood by looking at an example . The package lets you create your own geofacet visualizations using ggplot2 and built-in grids such as US states, EU countries and San Francisco Bay Area counties. Even more impressive, it comes with design-your-own geofacet grid capabilities. CRAN.</td>
<td>grid_design()</td>
</tr>
<tr class="even">
<td>purrr</td>
<td>data wrangling</td>
<td>purrr makes it easy to apply a function to each item in a list and return results in the format of your choice. It's more complex to learn than the older plyr package, but also more robust. And, its functions are more standardized than base R's apply family -- plus it's got functions for tasks like error-checking. CRAN.</td>
<td>map_df(mylist, myfunction) More: Charlotte Wickham's purr tutorial video , the purrr cheat sheet PDF download.</td>
</tr>
<tr class="odd">
<td>tidyr</td>
<td>data wrangling</td>
<td>tidyr initially won me over with specialized functions like fill (fill in missing columns from data above) and replace_na. But now I also use it for its main purpose too: helping you change data row and column formats from &quot;wide&quot; to &quot;long&quot;. CRAN.</td>
<td>See my step-by-step instructions and video in R tip: Reshape data with tidyr .</td>
</tr>
<tr class="even">
<td>splitstackshape</td>
<td>data wrangling</td>
<td>It's rare that I'd recommend a package that hasn't been updated in years, but the cSplit() function solves a rather complex shaping problem in an astonishingly easy way. If you have a data frame column with one or more comma-separated values (think a survey question with &quot;select all that apply&quot;), this is worth an install if you want to separate each item into its own new data frame row. . CRAN.</td>
<td>cSplit(mydata, &quot;multi_val_column&quot;, sep = &quot;,&quot;, direction = &quot;long&quot;).</td>
</tr>
<tr class="odd">
<td>magrittr</td>
<td>data wrangling</td>
<td>This package gave us the %&gt;% symbol for chaining R operations, but it's got other useful operators such as %&lt;&gt;% for mutating a data frame in place and and . as a placeholder for the original object being operated upon. CRAN.</td>
<td>mydf %&lt;&gt;% mutate(newcol = myfun(colname))</td>
</tr>
<tr class="even">
<td>validate</td>
<td>data wrangling</td>
<td>Intuitive data validation based on rules you can define, save and re-use. CRAN.</td>
<td>See the introductory vignette .</td>
</tr>
<tr class="odd">
<td>stringr</td>
<td>data wrangling</td>
<td>Numerous functions for text manipulation. Some are similar to existing base R functions but in a more standard format, including working with regular expressions. Some of my favorites: str_pad and str_trim. CRAN.</td>
<td>str_pad(myzipcodevector, 5, &quot;left&quot;, &quot;0&quot;)</td>
</tr>
<tr class="even">
<td>lubridate</td>
<td>data wrangling</td>
<td>Everything you ever wanted to do with date arithmetic, although understanding &amp; using available functionality can be somewhat complex. CRAN.</td>
<td>mdy(&quot;05/06/2015&quot;) + months(1) More examples in the package vignette</td>
</tr>
<tr class="odd">
<td>glue</td>
<td>data wrangling</td>
<td>Main function, also glue, evaluates variables and R expressions within a quoted string, as long as they're enclosed by {} braces. This makes for an elegant paste() replacement. CRAN.</td>
<td>glue(&quot;Today is {Sys.Date()}&quot;)</td>
</tr>
<tr class="even">
<td>car</td>
<td>data wrangling</td>
<td>car's recode function makes it easy to bin continuous numerical data into categories or factors. While base R's cut accomplishes the same task, I find recode's syntax to be more intuitive - just remember to put the entire recoding formula within double quotation marks. dplyr's case_when() function is another option worth considering. CRAN.</td>
<td>recode(x, &quot;1:3='Low'; 4:7='Mid'; 8:hi='High'&quot;)</td>
</tr>
<tr class="odd">
<td>scales</td>
<td>data wrangling</td>
<td>While this package has many more sophisticated ways to help you format data for graphing, it's worth a download just for the comma(), percent() and dollar() functions. CRAN.</td>
<td>comma(mynumvec)</td>
</tr>
<tr class="even">
<td>dplyr</td>
<td>data wrangling, data analysis</td>
<td>The essential data-munging R package when working with data frames. Especially useful for operating on data by categories. CRAN.</td>
<td>See the intro vignette</td>
</tr>
<tr class="odd">
<td>sqldf</td>
<td>data wrangling, data analysis</td>
<td>Do you know a great SQL query you'd use if your R data frame were in a SQL database? Run SQL queries on your data frame with sqldf. CRAN.</td>
<td>sqldf(&quot;select * from mydf where mycol &gt; 4&quot;)</td>
</tr>
<tr class="even">
<td>data.table</td>
<td>data wrangling, data analysis</td>
<td>Popular package for heavy-duty data wrangling. While I typically prefer dplyr, data.table has many fans for its speed with large data sets. CRAN.</td>
<td>Useful tutorial</td>
</tr>
<tr class="odd">
<td>zoo</td>
<td>data wrangling, data analysis</td>
<td>Robust package with a slew of functions for dealing with time series data; I like the handy rollmean function with its align=right and fill=NA options for calculating moving averages. CRAN.</td>
<td>rollmean(mydf, 7)</td>
</tr>
<tr class="even">
<td>gmodels</td>
<td>data wrangling, data analysis</td>
<td>There are several functions for modeling data here, but the one I use, CrossTable, simply creates cross-tabs with loads of options -- totals, proprotions and several statistical tests. CRAN.</td>
<td>CrossTable(myxvector, myyvector, prop.t=FALSE, prop.chisq = FALSE)</td>
</tr>
<tr class="odd">
<td>janitor</td>
<td>data wrangling, data analysis</td>
<td>Basic data cleaning made easy, such as finding duplicates by multiple columns, making R-friendly column names and removing empty columns. It also has some nice tabulating tools, like adding a total row, as well as generating tables with percentages and easy crosstabs. CRAN.</td>
<td>tabyl(mydf, sort = TRUE) %&gt;% adorn_totals(&quot;row&quot;)</td>
</tr>
<tr class="even">
<td>Prophet</td>
<td>forecasting</td>
<td>I don't do much forecasting analysis; but if I did, I'd start with this package. CRAN.</td>
<td>See the Quick start guide .</td>
</tr>
<tr class="odd">
<td>leaflet</td>
<td>mapping</td>
<td>Map data using the Leaflet JavaScript library within R. GitHub rstudio/leaflet.</td>
<td>See my tutorial</td>
</tr>
<tr class="even">
<td>ggmap</td>
<td>mapping</td>
<td>Although I don't use this package often for its main purpose of pulling down background map tiles, it's my go-to for geocoding up to 2,500 addresses with the Google Maps API with its geocode and mutate_geocode functions. CRAN.</td>
<td>geocode(&quot;492 Old Connecticut Path, Framingham, MA&quot;)</td>
</tr>
<tr class="odd">
<td>rgeocodio</td>
<td>mapping</td>
<td>This is a useful geocoding alternative, especially when ggmap generates messages that you're over your Google Maps API quota when you're not. It uses the geocod.io service . An API key is needed, but you can get one free that includes 2,500 lookups a day. GitHub hrbrmstr/rgeocodio.</td>
<td>gio_geocode(&quot;492 Old Connecticut Path, Framingham, MA&quot;)</td>
</tr>
<tr class="even">
<td>tmap &amp; tmaptools</td>
<td>mapping</td>
<td>These package offer an easy way to read in shape files and join data files with geographic info, as well as do some exploratory mapping. Recent functionality adds support for simple features, interactive maps and creating leaflet objects. Plus, tmaptools::palette_explorer() is a great tool for picking ColorBrewer palettes. CRAN.</td>
<td>See the package vignette or my mapping in R tutorial</td>
</tr>
<tr class="odd">
<td>sf</td>
<td>mapping, data wrangling</td>
<td>This package makes it much easier to do GIS work in R. Simple features protocols make geospatial data look a lot like regular data frames, while various functions allow for analysis such as determining whether points are in a polygons. A GIS game-changer for R. CRAN.</td>
<td>See the package vignettes, starting with the introduction, Simple Features for R .</td>
</tr>
<tr class="even">
<td>mapsapi</td>
<td>mapping, data wrangling</td>
<td>This interface to the Google Maps Direction and Distance Matrix APIs let you analyze and map distances and driving routes. CRAN.</td>
<td>google_directions( origin = c(my_longitude, my_latitude), destination = c(my_address), alternatives = TRUE Also see the vignette</td>
</tr>
<tr class="odd">
<td>tidycensus</td>
<td>mapping, data wrangling</td>
<td>Want to analyze and map U.S. Census Bureau data from 5-year American Community Surveys or 10-year censuses? This makes it easy to download numerical and geospatial info in R-ready format. CRAN.</td>
<td>See Basic usage of tidycensus .</td>
</tr>
<tr class="even">
<td>openxlsx</td>
<td>misc</td>
<td>If you need to write to an Excel file as well as read, this package is easy to use and offers a lot of options for formatting your spreadsheet. CRAN.</td>
<td>write.xlsx(mydf, &quot;myfile.xlsx&quot;)</td>
</tr>
<tr class="odd">
<td>installr</td>
<td>misc</td>
<td>Windows only: Update your installed version of R from within R. On CRAN.</td>
<td>updateR()</td>
</tr>
<tr class="even">
<td>reinstallr</td>
<td>misc</td>
<td>Seeks to find packages that had previously been installed on your system and need to be re-installed after upgrading R. CRAN.</td>
<td>reinstallr()</td>
</tr>
<tr class="odd">
<td>here</td>
<td>misc</td>
<td>This package has one function with a single, useful purpose: find your project's working directory. Surprisingly helpful if you want your code to run on more than one system. CRAN.</td>
<td>my_project_directory &lt;- here()</td>
</tr>
<tr class="even">
<td>beepr</td>
<td>misc</td>
<td>This is pretty much pure fun. Yes, getting an audible notification when code finishes running or encounters an error could be useful; but here, the available sounds include options like a fanfare flourish, a Mario Brothers tune, and even a scream. CRAN.</td>
<td>beep(&quot;wilhelm&quot;)</td>
</tr>
<tr class="odd">
<td>pacman</td>
<td>misc, package installation</td>
<td>This package is another that aims to solve one problem, and solve it well: package installation. The main functions will loadi a package that's already installed or installing it first if it's not available. While this is certainly possible to do with base R's require() and an if statement, p_load() is so much more elegant for CRAN packages, or p_load_gh() for GitHub. Other useful options include p_temp(), which allows for a temporary, this-session-only package installation. CRAN.</td>
<td>p_load(dplyr, here, tidycensus)</td>
</tr>
<tr class="even">
<td>roxygen2</td>
<td>package development</td>
<td>Useful tools for documenting functions within R packages. CRAN.</td>
<td>See this short, easy-to-read blog post on writing R packages , as well as the roxygen2 introductory vignette .</td>
</tr>
<tr class="odd">
<td>devtools</td>
<td>package development, package installation</td>
<td>devtools has a slew of functions aimed at helping you create your own R packages, such as automatically running all example code in your help files to make sure everything works. Requires Rtools on Windows and XCode on a Mac. On CRAN.</td>
<td>run_examples()</td>
</tr>
<tr class="even">
<td>usethis</td>
<td>package development, programming</td>
<td>Initially aimed at package development, usethis now includes useful functions for any coding project. Among its handy features are an edit family that lets you easily update your .Renvironment and .Rprofile files. On CRAN, but install GitHub version from &quot;r-lib/usethis&quot; for latest updates.</td>
<td>edit_r_environ()</td>
</tr>
<tr class="odd">
<td>remotes</td>
<td>package installation</td>
<td>If you want to install R packages from GitHub, devtools was long the go-to. However, it has a ton of other functions and some hefty dependences. remotes is a lighter-weight alternative if all you want is to install packages from GitHub as well as Bitbucket and some other sources. CRAN. ( ghit is another option, but is GitHub-only.)</td>
<td>remotes::install_github(&quot;mangothecat/franc&quot;)</td>
</tr>
<tr class="even">
<td>githubinstall</td>
<td>package installation</td>
<td>Do you want to install a package from GitHub without typing out the GitHub user name along with the repo name? Whether because you can't remember a package's GitHub owner's name, that name is long/complex to type out, or you just want to save yourself a little typing, this package is a handy option. Simply run githubinstall(&quot;packagename&quot;) and the package will suggest an account; then you respond Y to install or n if it's the wrong one. It even includes fuzzy matching if you misspell a package name!</td>
<td>githubinstall::githubinstall::(&quot;AnomalyDetection&quot;)</td>
</tr>
<tr class="odd">
<td>testthat</td>
<td>programming</td>
<td>Package that makes it easy to write unit tests for your R code. CRAN.</td>
<td>See the testing chapter of Hadley Wickham's book on R packages.</td>
</tr>
<tr class="even">
<td>profvis</td>
<td>programming</td>
<td>Is your R code sluggish? This package gives you a visual representative of your code line by line so you can find the speed bottlenecks. CRAN.</td>
<td>profvis({ your code here })</td>
</tr>
<tr class="odd">
<td>reticulate</td>
<td>programming</td>
<td>If you know Python as well as R, this package offers a suite of tools for calling Python from within R, as well as &quot;translating&quot; between R and Python objects such as Pandas data frames and R data frames. CRAN.</td>
<td>See the reticulate package website .</td>
</tr>
<tr class="even">
<td>tidytext</td>
<td>text mining</td>
<td>Elegant implementation of text mining functions using Hadley Wickham's &quot;tidy data&quot; principles. CRAN.</td>
<td>See tidytextmining.com for numerous examples.</td>
</tr>
<tr class="odd">
<td>rga</td>
<td>Web analytics</td>
<td>Use Google Analytics with R. GitHub skardhamar/rga.</td>
<td>See package README file and my tutorial</td>
</tr>
<tr class="even">
<td>googleanalyticsR</td>
<td>Web analytics</td>
<td>Another option for using Google Analytics with R, including adding features from GA's version 4 API. Also has anti-sampling options. CRAN.</td>
<td>See package website .</td>
</tr>
<tr class="odd">
<td>RSiteCatalyst</td>
<td>Web analytics</td>
<td>Use Adobe Analytics with R. GitHub randyzwitch/RSiteCatalyst.</td>
<td>See intro video</td>
</tr>
</tbody>
</table>

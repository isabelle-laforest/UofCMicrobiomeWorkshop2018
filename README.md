---
layout: workshop      # DON'T CHANGE THIS.
root: .               # DON'T CHANGE THIS EITHER.  (THANK YOU.)
venue: "University of Calgary"        # brief name of host site without address (e.g., "Euphoric State University")
address: "Health Research Innovation Centre, 3330 Hospital Drive N.W., Calgary, Alberta"      # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria")
country: "ca"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1)
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/ISO_639-1)
latlng: "51.066295, -114.134511"       # decimal latitude and longitude of workshop venue (e.g., "41.7901128,-87.6007318" - use http://www.latlong.net/)
humandate: "Nov 19-20-26-27, 2018"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "8:00 am - 12:00 pm"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2018-11-19      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2018-11-27        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
instructor: ["Isabelle Lafore-Lapointe"]
contact: "isabelle.laforestlap@ucalgary.ca"      # contact email address for host, lead instructor, or whoever else is handling questions
---

<!-- See instructions in the comments below for how to edit specific sections of this workshop template. -->

<!--
  HEADER
  Edit the values in the block above to be appropriate for your workshop.
  If the value is not 'true', 'false', 'null', or a number, please use
  double quotation marks around the value, unless specified otherwise.
  And run 'tools/check' *before* committing to make sure that changes are good.
-->

<h2 id="general">General Information</h2>

<!--
  AUDIENCE
  Explain who your audience is.  (In particular, tell readers if the
  workshop is only open to people from a particular institution.
-->
<p id="who">
  <strong>Who:</strong>
  The course is aimed at graduate students and other researchers.
  <strong>You need to have an interest in learning R and advanced statistical analysis of microbial DNA sequences.</strong>
</p>

<!--
  LOCATION
  This block displays the address and links to maps showing directions
  if the latitude and longitude of the workshop have been set.  You
  can use http://itouchmap.com/latlong.html to find the lat/long of an
  address.
-->
{% if page.latlng %}
<p id="where">
  <strong>Where:</strong>
  {{page.address}}.
  Get directions with
  <a href="//www.openstreetmap.org/?mlat={{page.latlng | replace:',','&mlon='}}&zoom=16">OpenStreetMap</a>
  or
  <a href="//maps.google.com/maps?q={{page.latlng}}">Google Maps</a>.
</p>
{% endif %}

<!--
  SPECIAL REQUIREMENTS
  Modify the block below if there are any special requirements.
-->
<p id="requirements">
  <strong>Requirements:</strong> Participants must bring a laptop with a
  Mac, Linux, or Windows operating sytem (not a tablet, Chromebook, etc.) that they have administrative privileges
  on. They should have a few specific software packages installed (listed
  <a href="#setup">below</a>).
</p>

<!--
  CONTACT EMAIL ADDRESS
  Display the contact email address set in the configuration file.
-->
<p id="contact">
  <strong>Contact</strong>:
  Please mail
  <a href="mailto:{{page.contact}}">{{page.contact}}</a> for more
  information.
</p>

<hr/>

<!--
  SCHEDULE
  Show the workshop's schedule.  Edit the items and times in the table
  to match your plans.  You may also want to change 'Day 1' and 'Day
  2' to be actual dates or days of the week.
-->
<h2 id="schedule">Schedule</h2>

<div class="row">
  <div class="col-md-6">
    <h3>Day 1</h3>
    <table class="table table-striped">
      <tr> <td>08:00</td>  <td>Introduction to R and Rstudio interface</td> </tr>
      <tr> <td>08:30</td> <td>Installing Packages and Accessing Online Resources</td> </tr>
      <tr> <td>09:00</td>  <td>Create objects (i.e. matrix, vector) in R</td> </tr>
      <tr> <td>10:00</td>  <td>20min Break</td> </tr>
      <tr> <td>10:20</td>  <td>How to Load Data</td> </tr>
      <tr> <td>11:00</td>  <td>Receiving your Sequencing Data</td> </tr>
      <tr> <td>11:30</td>  <td>Loading Sequencing Data in R</td> </tr>
    </table>
  </div>
  <div class="col-md-6">
    <h3>Day 2</h3>
    <table class="table table-striped">
      <tr> <td>08:00</td>  <td>Workflow to Prepare DNA Sequences</td> </tr>
      <tr> <td>08:30</td>  <td>Dada2 Tutorial Beguinning</td> </tr>
      <tr> <td>09:00</td>  <td>Quality and Trimming</td> </tr>
      <tr> <td>10:00</td>  <td>20min Break</td> </tr>
      <tr> <td>10:20</td>  <td>Chimeras and Filtering</td> </tr>
      <tr> <td>11:00</td>  <td>Assigning Taxonomy</td> </tr>
    </table>
  </div>
  <div class="col-md-6">
    <h3>Day 3</h3>
    <table class="table table-striped">
      <tr> <td>08:00</td>  <td>Main Results from Microbial Ecology</td> </tr>
      <tr> <td>08:30</td>  <td>What is Beta-Diversity</td> </tr>
      <tr> <td>09:00</td>  <td>Bdiv Indices and NMDS/PCoAs, and Permanovas</td> </tr>
      <tr> <td>10:00</td>  <td>20min Break</td> </tr>
      <tr> <td>10:20</td>  <td>Manipulating Graph with Ggplot2</td> </tr>
    </table>
  </div>
  <div class="col-md-6">
    <h3>Day 4</h3>
    <table class="table table-striped">
      <tr> <td>08:00</td>  <td>Alpha-Diversity and Richness</td> </tr>
      <tr> <td>09:30</td>  <td>Community composition</td> </tr>
      <tr> <td>10:00</td>  <td>20min Break</td> </tr>
      <tr> <td>10:20</td>  <td>Barcharts and Boxplots</td> </tr>
      <tr> <td>11:00</td>  <td>Anovas, linear, and non-parametric models</td> </tr>
      <tr> <td>11:30</td>  <td>Wrap-up</td> </tr>
    </table>
  </div>
</div>

<!--
  SETUP
  Delete irrelevant sections from the setup instructions.  Each
  section is inside a 'div' without any classes to make the beginning
  and end easier to find.
  This is the other place where people frequently make mistakes, so
  please preview your site before committing, and make sure to run
  'tools/check' as well.
-->

<h2 id="setup">Setup</h2>

<p>
  To participate in the Microbiome Workshop, you will need
  access to the software described below. In addition, you will
  need an up-to-date web browser.
</p>

<!--
<div id="r"> Start of 'R' section.
  <h3>R</h3>
  <p>
    <a href="http://www.r-project.org">R</a> is a programming language
    that is especially powerful for data exploration, visualization, and
    statistical analysis. To interact with R, we use
    <a href="http://www.rstudio.com/">RStudio</a>.
  </p>
  <div class="row">
    <div class="col-md-4">
      <h4 id="r-windows">Windows</h4>
      <a href="https://www.youtube.com/watch?v=q0PjTAylwoU">Video Tutorial</a>
      <p>
        Install R by downloading and running
        <a href="http://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a>
        from <a href="http://cran.r-project.org/index.html">CRAN</a>.
        Also, please install the
        <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
        Note that if you have separate user and admin accounts, you should run the 
        installers as administrator (right-click on .exe file and select "Run as 
        administrator" instead of double-clicking). Otherwise problems may occur later, 
        for example when installing R packages.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-macosx">Mac OS X</h4>
      <a href="https://www.youtube.com/watch?v=5-ly3kyxwEg">Video Tutorial</a>
      <p>
        Install R by downloading and running
        <a href="http://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a>
        from <a href="http://cran.r-project.org/index.html">CRAN</a>.
        Also, please install the
        <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-linux">Linux</h4>
      <p>
        You can download the binary files for your distribution
        from <a href="http://cran.r-project.org/index.html">CRAN</a>. Or
        you can use your package manager (e.g. for Debian/Ubuntu
        run <code>sudo apt-get install r-base</code> and for Fedora run
        <code>sudo yum install R</code>).  Also, please install the
        <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
  </div>
</div> <!-- End of 'R' section. -->

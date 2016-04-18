---
layout: workshop
root: .
venue: "ITM 2016 Software Carpentry Tutorials: Python, Git, and R"
address: Innovations in Travel Modeling 2016, Denver, CO
country: us    # country (lowercase two-letter ISO code such as "fr" - see https://en.wikipedia.org/wiki/ISO_3166-1)
language: en   # language (lowercase two-letter ISO code such as "fr" - see https://en.wikipedia.org/wiki/ISO_639-1)
latlng: "39.74,-104.99"     # fractional latitude and longitude (e.g., "39.74,-104.99"; you can use http://www.latlong.net/)
humandate: "May, 2016"
humantime: "TBD"
startdate: "2016-05-01"  # use YYYY-MM-DD format like "2015-01-01"
enddate: "2016-05-03"    # use YYYY-MM-DD format like" 2015-01-02"
instructor: ["Billy Charlton", "Josie Kressner", "Greg Macfarlane", "Brice Nichols"]
helper:
contact: "bcharlton@psrc.org"
---

<!--
  HEADER

  Edit the values in the block above to be appropriate for your workshop.
  If the value is not 'true', 'false', 'null', or a number, please use
  double quotation marks around the value, unless specified otherwise.
  And run 'tools/check' *before* committing to make sure that changes are good.
-->

<!--
  EVENTBRITE

  This block includes the Eventbrite registration widget if
  'eventbrite' has been set in the header.  You can delete it if you
  are not using Eventbrite, or leave it in, since it will not be
  displayed if the 'eventbrite' field in the header is not set.
-->
{% if page.eventbrite %}
<iframe
  src="https://www.eventbrite.com/tickets-external?eid={{page.eventbrite}}&ref=etckt"
  frameborder="0"
  width="100%"
  height="248px"
  scrolling="auto">
</iframe>
{% endif %}

<h2 id="general">General Information</h2>

<!--
  INTRODUCTION

  Edit the general explanatory paragraph below if you want to change
  the pitch.
-->

Hi there! These sessions are introductory workshops that can help get you up to speed on tools that will make your work day easier. This course is based on materials produced by [Software Carpentry]({{site.swc_site}}). Software Carpentry's mission is to help scientists and engineers get more research done in less time and with less pain by teaching them basic lab skills for scientific computing.

We've hand-picked three topics that are relevant to the demand modeler profession. Participants will be encouraged to
help one another and to apply what they have learned to their own research problems.

<!--
  AUDIENCE

  Explain who your audience is.  (In particular, tell readers if the
  workshop is only open to people from a particular institution.
-->

<table><tr>
<td><b>Who:</b></td>

<td>The course is aimed at practitioners, researchers and data scientists in the modeling field. <i>You don't need to have any previous knowledge of the tools that will be presented at the workshop.</i></td></tr>

<td><b>Where:</b></td>

<td>{{page.address}}</td>

<tr><td valign="top"><b>Requirements:</b></td>

<td>All participants will need to set up a few specific software packages on their computer <a href="#setup">(listed below)</a>.
<ul><b>you must bring your own laptop</b>, set up with the software below. These are interactive sessions!</li>
</ul>
</td></tr>

</table>

Email {% if page.contact %}
[{{page.contact}}](mailto:{{page.contact}})
{% else %}
[{{site.contact}}](mailto:{{site.contact}})
{% endif %} for more information.


---

## Syllabus

<div class="row">
  <div class="col-md-4">
    <h3 id="syllabus-git">Git Version Control</h3>
    <ul>
      <li>Creating a repository</li>
      <li>Recording changes to files: <code>add</code>, <code>commit</code>, ...</li>
      <li>Viewing changes: <code>status</code>, <code>diff</code>, ...</li>
      <li>Ignoring files</li>
      <li>Working on the web: <code>clone</code>, <code>pull</code>, <code>push</code>, ...</li>
      <li>Collaborating with others</li>
      <li>Resolving conflicts</li>
      <li>Where to host work, and why</li>
      <li><a href="{{site.swc_githubio}}/git-novice/reference.html">Reference...</a></li>
    </ul>
  </div>

  <div class="col-md-4">
    <h3 id="syllabus-python">Programming in Python</h3>
    <ul>
      <li>Using libraries</li>
      <li>Working with arrays</li>
      <li>Reading and plotting data</li>
      <li>Creating and using functions</li>
      <li>Loops and conditionals</li>
      <li>Defensive programming</li>
      <li>Using Python from the command line</li>
      <li><a href="{{site.swc_githubio}}/python-novice-inflammation/reference.html">Reference...</a></li>
    </ul>
  </div>

  <div class="col-md-4">
    <h3 id="syllabus-r">Programming in R</h3>
    <ul>
      <li>Working with vectors and data frames</li>
      <li>Reading and plotting data</li>
      <li>Creating and using functions</li>
      <li>Loops and conditionals</li>
      <li>Using R from the command line</li>
      <li><a href="{{site.swc_githubio}}/r-novice-inflammation/reference.html">Reference...</a></li>
    </ul>
  </div>
</div>


------

## Setup

To participate in a workshop, you will need
access to the software described below. In addition, you will
need an up-to-date web browser.

**Be sure to set up all software items below on your laptop computer ahead of time -- before the day of the course.** We will not have time to troubleshoot software installation problems in the session, so if these tools are not installed you will not be able to participate fully.

We maintain a list of common issues that occur during installation as a reference for instructors that may be useful on the [Configuration Problems and Solutions wiki page](https://github.com/swcarpentry/workshop-template/wiki/Configuration-Problems-and-Solutions).


---

### Windows Instructions

#### A. Git and the 'Bash' Prompt

***You need the latest version of Git. Even if you already have Git installed on your PC, replace it with this new version.***

Git is a version control system that lets you track who made changes to what when and has options for easily updating a shared or public version of your code
on [github.com](https://github.com). You will need a [supported web browser](https://help.github.com/articles/supported-browsers) (current versions of Chrome, Firefox or Safari, or Internet Explorer version 9 or above).

Bash is a commonly-used shell that gives you the power to do simple tasks more quickly. On Windows, the easiest way to get Bash is to use the copy that is included in the Git for Windows installer.

Easy install for Git:

1. Download the [Git for Windows Installer](https://git-for-windows.github.io).
2. Run the installer and click next through the installer prompts, paying attention to these settings:
   * Select **"Use Git from the Windows Command Prompt"**. If you forget to do this, programs that you need for the workshop will not work properly. If this happens, rerun the installer and select the appropriate option.
   * Keep **"Checkout Windows-style, commit Unix-style line endings"** selected.
   * Select **"Use Windows' default console window"**
   * The other settings are mostly benign and the defaults should suffice.

#### B. Text Editor

When you're writing code, it's nice to have a text editor that is optimized for writing code, with features like automatic
color-coding of key words.  If you don't already have a text editor of your preference on your machine, follow these instructions.

The default text editor on Mac OS X and Linux is usually set to Vim, which is a really bad choice for beginners. Notepad isn't much better for Windows users. If you accidentally find yourself stuck in Vim, try typing the escape key, followed by <code>:q!</code> (colon, lower-case 'q',
exclamation mark), then hitting Return to return to the shell.

**nano** is a basic editor and the default that instructors use in the workshop.

* To install nano, download the [Software Carpentry Windows installer](https://github.com/swcarpentry/windows-installer/releases/latest) and double click on the file to run it. *This installer requires an active internet connection.*

* **Others editors** that you may want to use are [Notepad++](http://notepad-plus-plus.org) or [Sublime Text](http://www.sublimetext.com). Be aware that you must add the editor's installation directory to your system path.


#### C. Python

[Python](http://python.org) is a very popular language for
scientific computing, and great for general-purpose programming as
well.  Installing all of its scientific packages individually can be
a bit difficult, so we recommend [Anaconda](https://www.continuum.io/anaconda), an all-in-one installer.

Regardless of how you choose to install it, **please make sure you install Python version 2.7**. We are not ready to move to Python 3 just yet.

We will teach Python using the IPython notebook, a programming environment
that runs in a web browser. For this to work, you will need an
up-to-date browser. The current versions of the Chrome, Safari and
Firefox browsers are [all supported](http://ipython.org/ipython-doc/2/install/install.html#browser-compatibility). Some older browsers, including Internet Explorer version 9 and below, are not.

To install Anaconda Python:

* Open the Continuum Ananaconda [download page](http://continuum.io/downloads) with your web browser.
* Download the Python 2.7 installer for Windows.
* Install Python 2.7 using all of the defaults for installation **except** make sure to check **Make Anaconda the default Python**.

If you decide not to install the all-in-one Continuum Anaconda Python, ensure that you have python libraries numpy, pandas, matplotlib, and ipython-notebook installed.


#### D. R-Project (Statistics Software)

[R](http://www.r-project.org) is a programming language that is especially powerful for data exploration, visualization, and statistical analysis. To interact with R, we use [RStudio](http://www.rstudio.com).

Install R by downloading and running
        <a href="http://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a>
        from <a href="http://cran.r-project.org/index.html">CRAN</a>.</p>

Then install the <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.


#### E. Check your setup

**To check you have the correct version of Python:**

* Download [swc-installation-test-1.py](/itm-tutorial-2016/setup/swc-installation-test-1.py)
* Open up a Bash shell - start "Git Bash" on Windows, or "Terminal" on Mac
* Change into the directory where you put the script by typing in the bash window:
   * <code>cd ~/Downloads</code>
* Run the script:
   * <code>python swc-installation-test-1.py</code>

**To check you have set up the other software requirements correctly:**

* Download [swc-installation-test-2.py](/itm-tutorial-2016/setup/swc-installation-test-2.py)
* Open up a Bash shell. Change into the directory where you put the script by typing in the bash window:
   * <code>cd ~/Downloads</code>
* Run the script:
   * <code>python swc-installation-test-2.py</code>

If anything is missing, the script output will specify what needs to be corrected.

---

### Mac OS X

* **Git:**
  * For OS X 10.9 and higher, install Git for Mac by downloading and running the most recent "mavericks" installer from
        [this list](http://sourceforge.net/projects/git-osx-installer/files/). After installing Git, there will not be anything in your <code>/Applications</code> folder, as Git is a command line program.
  * For older versions of OS X (10.5-10.8), use the most recent available installer labelled "snow-leopard" [available here](http://sourceforge.net/projects/git-osx-installer/files).
* **Python:** We recommend the Continuum Ananconda Python all-in-one python installer, which installs a basic Python system as well as the scientific computing modules required for this course.
  * Open [http://continuum.io/downloads](http://continuum.io/downloads) with your web browser.
  * Download the Python 2.7 installer for OS X.  We are not using Python 3 yet.
  * Install Python 2.7 using all of the defaults for installation.
* **R:** Install R by downloading and running
        <a href="http://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a>
        from <a href="http://cran.r-project.org/index.html">CRAN</a>.
        <br/>Also, please install the <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.

---

### Linux

Use your system's package manager to install python, sqlite, git, and nano. I can't help with all of the different linux flavors out there.

* Python -- also be sure to install numpy, ipython, and pandas
* R -- install R and R-Studio
* Git -- the basic git tools in your distribution are probably sufficient.



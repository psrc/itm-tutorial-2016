---
layout: workshop
root: .
venue: "ITM 2016 Tutorials: Python, Git, and R"
address: Innovations in Travel Modeling 2016, Denver, CO
country: us    # country (lowercase two-letter ISO code such as "fr" - see https://en.wikipedia.org/wiki/ISO_3166-1)
language: en   # language (lowercase two-letter ISO code such as "fr" - see https://en.wikipedia.org/wiki/ISO_639-1)
latlng: "39.74,-104.99"     # fractional latitude and longitude (e.g., "39.74,-104.99"; you can use http://www.latlong.net/)
humandate: "Sunday, May 1, 2016 and Tuesday, May 3, 2016"
humantime: ""
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

At this year's TRB Innovations in Travel Modeling Conference, we will host three tutorials that can help get you up to speed on tools to make your work day easier. This course is based on materials produced by [Software Carpentry]({{site.swc_site}}). Software Carpentry's mission is to help scientists and engineers get more research done in less time and with less pain by teaching them basic lab skills for scientific computing.

These hands-on workshops will cover basic concepts and workflow with Python, Git, and R.

<b>Travel Analysis and Modeling using Python</b><br>
Sunday, May 1, 2016 1:00 p.m. - 2:45 p.m.<br>
Moderators: Brice Nichols and Billy Charlton (Puget Sound Regional Council)<br>
Interested in learning Python but don't know where to start? Join us for this laptops-open tutorial that starts with the very basics and builds the basic skills you will need to use Python for travel analysis.

<b>Tools for Collaborative Open Source Model Development: GitHub and beyond!</b><br>
Sunday, May 1, 2016 3:00 p.m. - 5:00 p.m.<br>
Moderators: Billy Charlton and Brice Nichols (Puget Sound Regional Council)<br>
This laptops-open tutorial will build skills necessary for effective collaborative software development including version control, issue-tracking, documentation, release planning, testing, and code review using GitHub and other associated tools.

<b>Using R for Data Cleaning, Munging, Visualizing, and Modeling</b><br>
Tuesday, May 3, 2016 1:30 p.m. - 3:00 p.m.<br>
Moderators: Josie Kressner (Transport Foundry) and Greg Macfarlane (Parsons Brinckerhoff)<br>
This laptops-open tutorial will help you get your data munging, cleaning, and mathematical modeling done fast and cleanly in R. Hands-on experience during this session will use ACS PUMS, CTPP, NHTS, and other travel datasets you are familiar with for travel analysis.

<!--
  AUDIENCE

  Explain who your audience is.  (In particular, tell readers if the
  workshop is only open to people from a particular institution.
-->

<table><tr>
<td><b>Who:</b></td>

<td>The course is aimed at transportation practitioners and researchers. <i>You don't need to have any previous knowledge of the tools that will be presented at the workshop.</i></td></tr>

<td><b>Where:</b></td>

<td>{{page.address}}.</td>

<tr><td valign="top"><b>Requirements:</b></td>

<td>All participants will need to bring a laptop to these tutorials with a few specific software packages installed on their computer <a href="#setup">(listed below)</a>.
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
    <h3 id="syllabus-git">Git</h3>
    <ul>
      <li>Creating a repository</li>
      <li>Recording changes to files: <code>add</code>, <code>commit</code>, ...</li>
      <li>Viewing changes: <code>status</code>, <code>diff</code>, ...</li>
      <li>Ignoring files</li>
      <li>Working on the web: <code>clone</code>, <code>pull</code>, <code>push</code>, ...</li>
      <li>Collaborating with others</li>
      <li>Resolving conflicts</li>
      <li>Where to host work, and why</li>
      <li><a href="http://psrc.github.io/itm-tutorial-git">Reference...</a></li>
    </ul>
  </div>

  <div class="col-md-4">
    <h3 id="syllabus-python">Python</h3>
    <ul>
      <li>Using libraries</li>
      <li>Working with arrays</li>
      <li>Reading and plotting data</li>
      <li>Creating and using functions</li>
      <li>Loops and conditionals</li>
      <li>Defensive programming</li>
      <li>Using Python from the command line</li>
      <li><a href="http://psrc.github.io/itm-tutorial-python">Reference...</a></li>
    </ul>
  </div>

  <div class="col-md-4">
    <h3 id="syllabus-r">R</h3>
    <ul>
      <li>Working with vectors and data frames</li>
      <li>Reading and plotting data</li>
      <li>Creating and using functions</li>
      <li>Loops and conditionals</li>
      <li>Using R from the command line</li>
      <li><a href="http://psrc.github.io/itm-tutorial-R">Reference...</a></li>
    </ul>
  </div>
</div>


------

## Setup

To participate in the tutorials, you will need to install the software described below. You only need to install the software required for each tutorial you will attend. In addition, you will need an up-to-date web browser.

Software Carpentry maintain a list of common issues that occur during installation as a reference: [configuration problems and solutions](https://github.com/swcarpentry/workshop-template/wiki/Configuration-Problems-and-Solutions).

+ Git Tutorial
  + Text editor
  + Bash
  + Git
+ Python Tutorial
  + Text editor
  + Python 2.7
+ R Tutorial
  + R
  + RStudio
  + Two example data files

### Text Editor
When you're writing code, it's nice to have a text editor that is optimized for writing code, with features like automatic color-coding of key words. **nano** is a very basic editor and the default that instructors use in the workshop.

#### Windows
* To install nano, download the [Software Carpentry Windows installer](https://github.com/swcarpentry/windows-installer/releases/latest) and double click on the file to run it. *This installer requires an active internet connection.* Even if you choose not to use nano, we recommend you run the Software Carpentry installer because it also sets sane defaults for some other tools such as SQLite and Make.
* **Other editors** that you may prefer are [Notepad++](http://notepad-plus-plus.org), [Sublime Text](http://www.sublimetext.com), or [Atom](https://atom.io/). Be aware that you must add the editor's installation directory to your system path so that you can follow along in the tutorials. Please ask your instructor to help you do this.

#### Mac/Linux
* **nano** is usually installed by default on Mac and Linux. If you're on a Linux systetm that does not preinstall it, use your system's package manager to install **nano**.
* Note that the default text editor on Mac OS X and Linux is usually set to Vim, which is difficult for beginners. If you accidentally find yourself stuck in it, try typing the escape key, followed by <code>:q!</code> (colon, lower-case 'q', exclamation mark), then hitting Return to return to the shell.


### Bash
Bash is a commonly-used shell that gives you the power to do simple tasks more quickly.

#### Windows
On Windows, the easiest way to get Bash is to use the copy that is included in the Git for Windows installer. Skip to the Git section.

#### Mac/Linux
The default shell in all versions of Mac OS X is Bash, so no need to install anything. You access Bash from the Terminal, which is found in <code>/Applications/Utilities</code>. You may want to keep Terminal in your dock for this workshop. Linux also by default usually includes Bash as the shell. If not, use your package manager to install it.


### Git
***You need the latest version of 64-bit Git. Even if you already have Git installed on your laptop, replace it with this new version.*** Git is a version control system that lets you track who made changes to what when and has options for easily updating a shared or public version of your code on [github.com](https://github.com). You will need a [supported web browser](https://help.github.com/articles/supported-browsers) (current versions of Chrome, Firefox or Safari, or Internet Explorer version 9 or above).

#### Windows
1. Download the [Git for Windows Installer](https://git-for-windows.github.io).
2. Run the installer and click next through the installer prompts, paying attention to these settings:
   * Select **"Use Git from the Windows Command Prompt"**. If you forget to do this, programs that you need for the workshop will not work properly. If this happens, rerun the installer and select the appropriate option.
   * Keep **"Checkout Windows-style, commit Unix-style line endings"** selected.
   * Select **"Use Windows' default console window"**
   * The other settings are mostly benign and the defaults should suffice.

#### Mac/Linux
* For OS X 10.9 and higher, install Git for Mac by downloading and running the most recent "mavericks" installer from [this list](http://sourceforge.net/projects/git-osx-installer/files/). After installing Git, there will not be a Git application in your <code>/Applications</code> folder, as Git is a command line program.
* For older versions of OS X (10.5-10.8), use the most recent available installer labelled "snow-leopard" [available here](http://sourceforge.net/projects/git-osx-installer/files). After installing Git, there will not be a Git application in your <code>/Applications</code> folder, as Git is a command line program.



### Python 2.7
[Python](http://python.org) is a very popular language for scientific computing, and great for general-purpose programming as well.  Installing all of its scientific packages individually can be a bit difficult, so we recommend [Anaconda](https://www.continuum.io/anaconda), an all-in-one installer. Regardless of how you choose to install it, **please make sure you install Python version 2.7**. We are not ready to move to Python 3 just yet.

We will teach Python using the IPython notebook, a programming environment that runs in a web browser. For this to work, you will need an up-to-date browser. The current versions of the Chrome, Safari and Firefox browsers are [all supported](http://ipython.org/ipython-doc/2/install/install.html#browser-compatibility). Some older browsers, including Internet Explorer version 9 and below, are not.

#### Windows
To install Anaconda Python:

* Open the Continuum Ananaconda [download page](http://continuum.io/downloads) with your web browser.
* Download the Python 2.7 installer for Windows.
* Install Python 2.7 using all of the defaults for installation **except** make sure to check **Make Anaconda the default Python**.

#### Mac/Linux
We recommend the Continuum Ananconda Python all-in-one python installer, which installs a basic Python system as well as the scientific computing modules required for this course.

* Open [http://continuum.io/downloads](http://continuum.io/downloads) with your web browser.
* Download the Python 2.7 installer for OS X or your Linux.  We are not using Python 3 yet.
* Install Python 2.7 using all of the defaults for installation.

### R
[R](http://www.r-project.org) is a programming language that is especially powerful for data exploration, visualization, and statistical analysis. To interact with R, we use [RStudio](http://www.rstudio.com).

Download these two files before arriving: [nhts_day.csv](http://psrc.github.io/itm-tutorial-R/data/nhts_day.csv) and [nhts_per.csv](http://psrc.github.io/itm-tutorial-R/data/nhts_per.csv). These only include the first 200 lines of the full NHTS files. We will tell you where to put them during the tutorial. Just make sure you have them accessible offline before arriving.

#### Windows
Install R by downloading and running <a href="http://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a> from <a href="http://cran.r-project.org/index.html">CRAN</a>. Then install the <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.

#### Mac
Install R by downloading and running <a href="http://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a> from <a href="http://cran.r-project.org/index.html">CRAN</a>. Also, please install the <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.

#### Linux
You can download the binary files for your distribution from <a href="http://cran.r-project.org/index.html">CRAN</a>. Or you can use your package manager (e.g. for Debian/Ubuntu run <code>sudo apt-get install r-base</code> and for Fedora run <code>sudo yum install R</code>). Also, please install the <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.


## Check Your Setup

**To check you have the correct version of Python:**

* Download [swc-installation-test-1.py](/itm-tutorial-2016/setup/swc-installation-test-1.py)
* Open up a Bash shell - start "Git Bash" on Windows, "Terminal" on Mac, or your bash shell on Linux.
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

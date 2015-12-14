---
layout: workshop
root: .
venue: "Scripting Carpentry"
address: Puget Sound Regional Council, 1011 Western Ave, Suite 500, Seattle WA
country: us    # country (lowercase two-letter ISO code such as "fr" - see https://en.wikipedia.org/wiki/ISO_3166-1)
language: en   # language (lowercase two-letter ISO code such as "fr" - see https://en.wikipedia.org/wiki/ISO_639-1)
latlng: 47.6054148,-122.337372     # fractional latitude and longitude (e.g., "41.7901128,-87.6007318"; you can use http://www.latlong.net/)
humandate: "December, 2015"
humantime: "12:30 pm - 4:30 pm daily"
startdate: "2015-12-15"  # use YYYY-MM-DD format like "2015-01-01"
enddate: "2015-12-16"    # use YYYY-MM-DD format like" 2015-01-02"
instructor: ["Billy Charlton", "Peter&nbsp;Caballero", "Suzanne&nbsp;Childress", "Brice&nbsp;Nichols", "Hana&nbsp;Ševčíková", "Stefan&nbsp;Coe"]
helper: ['TBD']
contact: "bcharlton@psrc.org"
etherpad: "https://public.etherpad-mozilla.org/p/psrc-scripting-workshop-2015"
eventbrite:       # optional (insert the alphanumeric key for Eventbrite registration, e.g., "1234567890AB")
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

Hi there! Scripting Carpentry is a set of introductory workshops that can help get you up to speed on tools that will make your work day easier. This course is based on materials produced by [Software Carpentry]({{site.swc_site}}). Software Carpentry's mission is to help scientists and engineers get more research done in less
time and with less pain by teaching them basic lab skills for
scientific computing.

This hands-on workshop will cover basic
  concepts and tools, including program design, version control, data
  management, and task automation. Participants will be encouraged to
  help one another and to apply what they have learned to their own
  research problems.

<!--
  AUDIENCE

  Explain who your audience is.  (In particular, tell readers if the
  workshop is only open to people from a particular institution.
-->

<table><tr>
<td><b>Who:</b></td>

<td>The course is aimed at practitioners, researchers and data scientists in any technical field. <i>You don't need to have any previous knowledge of the tools that will be presented at the workshop.</i></td></tr>

<td><b>Where:</b></td>

<td>{{page.address}}.<br/>Get directions with <a href="http://www.openstreetmap.org/?mlat={{page.latlng | replace:',','&mlon='}}&zoom=16">OpenStreetMap</a> or <a href="http://maps.google.com/maps?q={{page.latlng}}).">Google Maps</a></td>

<tr><td valign="top"><b>Requirements:</b></td>

<td>All participants will need to set up a few specific software packages on their computer <a href="#setup">(listed below)</a>.
<ul><li>If you are PSRC staff, set up the software on your <b>primary work desktop/laptop</b> in advance of the workshop day.</li>
<li>If you are not currently working at PSRC, <b>you must bring your own laptop</b>, set up with the software below.</li>
<li>All participants are also required to abide by the Software Carpentry <a href="{{site.swc_site}}/conduct.html">Code of Conduct</a>.</li>
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
  <div class="col-md-6">
    <h3 id="syllabus-shell">Command-Line Ninja:<br/>The Unix Shell</h3>
    <ul>
      <li>Files and directories</li>
      <li>History and tab completion</li>
      <li>Pipes and redirection</li>
      <li>Looping over files</li>
      <li>Creating and running shell scripts</li>
      <li>Finding things</li>
      <li><a href="{{site.swc_githubio}}/shell-novice/reference.html">Reference...</a></li>
    </ul>
  </div>
  <div class="col-md-6">
    <h3 id="syllabus-git">Version Control with Git</h3>
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

</div>

<div class="row">
  <div class="col-md-6">
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
  <div class="col-md-6">
    <h3 id="syllabus-sql">Managing Data with SQL</h3>
    <ul>
      <li>Reading and sorting data</li>
      <li>Filtering with <code>where</code></li>
      <li>Calculating new values on the fly</li>
      <li>Handling missing values</li>
      <li>Combining values using aggregation</li>
      <li>Combining information from multiple tables using <code>join</code></li>
      <li>Creating, modifying, and deleting data</li>
      <li>Python and databases</li>
      <li><a href="{{site.swc_githubio}}/sql-novice-survey/reference.html">Reference...</a></li>
    </ul>
  </div>
</div>

<div class="row">
  <div class="col-md-6">
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

  <div class="col-md-6">
    <h3 id="syllabus-make">Automation with Make</h3>
    <ul>
      <li>Introduction</li>
      <li>Makefiles</li>
      <li>Automatic variables</li>
      <li>Dependencies on data and code</li>
      <li>Pattern rules</li>
      <li>Variables and Functions</li>
      <li><a href="{{site.swc_githubio}}/make-novice/reference.html">Reference...</a></li>
    </ul>
  </div>

</div>

<!--
  ETHERPAD

  At `_misc/etherpad.txt` you will find a template for the etherpad.

  Display the Etherpad for the workshop.  You can set this up in
  advance or on the first day; either way, make sure you push changes
  to GitHub after you have its URL.  To create an Etherpad, go to

      http://pad.software-carpentry.org/YYYY-MM-DD-site

  where 'YYYY-MM-DD-site' is the identifier for your workshop,
  e.g., '2015-06-10-esu'.
-->

{% if page.etherpad %}

#### Etherpad

We will use Etherpad for chatting, taking notes, and sharing URLs and bits of code.

**Etherpad:** [{{page.etherpad}}]({{page.etherpad}}).

{% endif %}

------

## Setup

To participate in a Software Carpentry workshop, you will need
access to the software described below. In addition, you will
need an up-to-date web browser.

**Be sure to set up all five software items below on your primary desktop computer ahead of time -- before the day of the course.**

At the workshop, you may be using a borrowed laptop to remote control your primary work computer: that way, all the software setup can happen ahead of time. Added bonus: all the software will be at your fingertips when you return to your desk afterwards, too.

We maintain a list of common issues that occur during installation as a reference for instructors that may be useful on the [Configuration Problems and Solutions wiki page](https://github.com/swcarpentry/workshop-template/wiki/Configuration-Problems-and-Solutions).


---

### Windows Instructions

#### A. Git and the Unix 'Bash' Shell

Git is a version control system that lets you track who made changes to what when and has options for easily updating a shared or public version of your code
on [github.com](https://github.com). You will need a [supported web browser](https://help.github.com/articles/supported-browsers) (current versions of Chrome, Firefox or Safari, or Internet Explorer version 9 or above).

Bash is a commonly-used shell that gives you the power to do simple tasks more quickly.

On Windows, the easiest way to get Bash is to use the copy that is included in the Git for Windows installer.

1. Download the [Git for Windows Installer](https://git-for-windows.github.io).
2. Run the installer and follow the steps below:
   1. Click on "Next".
   2. Click on "Next".
   3. Click on "Next".
   4. Click on "Next".
   5. Click on "Next".
   6. **Select "Use Git from the Windows Command Prompt" and click on "Next".** If you forget to do this, programs that you need for the workshop will not work properly. If this happens, rerun the installer and select the appropriate option.  Click "Next"
   7. Keep **"Checkout Windows-style, commit Unix-style line endings"** selected. Click "Next".
   8. Select **"Use Windows' default console window"** and click on "Next" and "Finish".
3. ConsoleZ is a much nicer "terminal" program that has a legible font, resizable window, and more. You'll use ConsoleZ to launch the Bash terminal window instead of using the "Git Bash" icon.
   * Download the [ConsoleZ Installer](/2015-12-scripting-workshop/setup/ConsoleZ-Installer.exe) and follow the default installer prompts.
   * If Chrome or Firefox warns you that the installer file is untrusted, just go along with it. I created the installer here at PSRC and it is safe to install.

#### B. Text Editor

When you're writing code, it's nice to have a text editor that is
optimized for writing code, with features like automatic
color-coding of key words.

The default text editor on Mac OS X and Linux is usually set to Vim, which is a bad choice for beginners. If you accidentally find yourself stuck in it, try typing the escape key, followed by <code>:q!</code> (colon, lower-case 'q',
exclamation mark), then hitting Return to return to the shell.

**nano** is a basic editor and the default that instructors use in the workshop.

* To install nano, download the [Software Carpentry Windows installer](https://github.com/swcarpentry/windows-installer/releases/latest) and double click on the file to run it. *This installer requires an active internet connection.*
* Even if you choose not to use nano, we recommend you run the Software Carpentry installer because it also sets sane defaults for some other tools such as SQLite and Make.
* **Others editors** that you may want to use are [Notepad++](http://notepad-plus-plus.org) or [Sublime Text](http://www.sublimetext.com). Be aware that you must add the editor's installation directory to your system path. Please ask your instructor to help you do this.

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


#### D. SQLite

***FOR DISCUSSION*** - SQLite is easiest way to fiddle with SQL on a desktop. But we could also set up access to our "real" MySQL databases right?

SQL is a specialized programming language used with databases. Here at PSRC, we have existing enterprise databases in MS-SQL and MySQL, but those are a bit complex to set up. For this course, we use a simple database manager called [SQLite](http://www.sqlite.org). The SQL language is essentially identical, so the skills will all transfer -- and having a simple desktop version of SQL has its own benefits.

* The [Software Carpentry Windows Installer](https://github.com/swcarpentry/windows-installer/releases/latest) installs SQLite for Windows. If you used the installer already to install the nano text editor, you don't need to run it again. Otherwise, run it now.

#### E. R-Project (Statistics Software)

[R](http://www.r-project.org) is a programming language that is especially powerful for data exploration, visualization, and statistical analysis. To interact with R, we use [RStudio](http://www.rstudio.com).

<div class="row">
    <div class="col-md-4">
      <h4 id="r-windows">Windows</h4>
      <p>
        Install R by downloading and running
        <a href="http://cran.r-project.org/bin/windows/base/release.htm">this .exe file</a>
        from <a href="http://cran.r-project.org/index.html">CRAN</a>.
        <br/>Also, please install the
        <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
    <div class="col-md-4">
      <h4 id="r-macosx">Mac OS X</h4>
      <p>
        Install R by downloading and running
        <a href="http://cran.r-project.org/bin/macosx/R-latest.pkg">this .pkg file</a>
        from <a href="http://cran.r-project.org/index.html">CRAN</a>.
        <br/>Also, please install the
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
        <code>sudo yum install R</code>).
        <br/>Also, please install the
        <a href="http://www.rstudio.com/ide/download/desktop">RStudio IDE</a>.
      </p>
    </div>
</div> <!-- End of 'R' section. -->

#### E. Check your setup

**To check you have the correct version of Python:**

* Download [swc-installation-test-1.py](/2015-12-scripting-workshop/setup/swc-installation-test-1.py)
* Open up a Bash shell - start "Git Bash" on Windows, or "Terminal" on Mac
* Change into the directory where you put the script by typing in the bash window:
   * <code>cd ~/Downloads</code>
* Run the script:
   * <code>python swc-installation-test-1.py</code>

**To check you have set up the other software requirements correctly:**

* Download [swc-installation-test-2.py](/2015-12-scripting-workshop/setup/swc-installation-test-2.py)
* Open up a Bash shell. Change into the directory where you put the script by typing in the bash window:
   * <code>cd ~/Downloads</code>
* Run the script:
   * <code>python swc-installation-test-2.py</code>

If anything is missing, the script output will specify what needs to be corrected.

---

### Mac OS X

* **Bash:** the default shell in all versions of Mac OS X is Bash, so no need to install anything.
  * You access Bash from the Terminal
        (found in <code>/Applications/Utilities</code>). You may want to keep Terminal in your dock for this workshop.
* **Git:**
  * For OS X 10.9 and higher, install Git for Mac by downloading and running the most recent "mavericks" installer from
        [this list](http://sourceforge.net/projects/git-osx-installer/files/). After installing Git, there will not be anything in your <code>/Applications</code> folder, as Git is a command line program.
  * For older versions of OS X (10.5-10.8), use the most recent available installer labelled "snow-leopard" [available here](http://sourceforge.net/projects/git-osx-installer/files).
* **Python:** We recommend the Continuum Ananconda Python all-in-one python installer, which installs a basic Python system as well as the scientific computing modules required for this course.
  * Open [http://continuum.io/downloads](http://continuum.io/downloads) with your web browser.
  * Download the Python 2.7 installer for OS X.  We are not using Python 3 yet.
  * Install Python 2.7 using all of the defaults for installation.
* **SQLite**. SQLite comes pre-installed on Mac OS X.

---

### Linux

Use your system's package manager to install python, sqlite, git, and nano.


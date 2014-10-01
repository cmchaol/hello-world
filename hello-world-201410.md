<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#sec-1">1. my git experience</a>
<ul>
<li><a href="#sec-1-1">1.1. repository download, edit, upload, by git</a></li>
<li><a href="#sec-1-2">1.2. Caching your GitHub password in Git</a></li>
</ul>
</li>
<li><a href="#sec-2">2. org mode</a>
<ul>
<li><a href="#sec-2-1">2.1. synonym</a></li>
<li><a href="#sec-2-2">2.2. org export backends</a></li>
<li><a href="#sec-2-3">2.3. org export Literal examples</a></li>
</ul>
</li>
<li><a href="#sec-3">3. R</a>
<ul>
<li><a href="#sec-3-1">3.1. installation in gentoo</a></li>
<li><a href="#sec-3-2">3.2. ESS</a></li>
</ul>
</li>
</ul>
</div>
</div>


# my git experience

## repository download, edit, upload, by git

### summary

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="left" />

<col  class="left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="left">the repsitory</th>
<th scope="col" class="left">the git command</th>
</tr>
</thead>

<tbody>
<tr>
<td class="left">download</td>
<td class="left">git clone</td>
</tr>


<tr>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="left">edit</td>
<td class="left">git add</td>
</tr>


<tr>
<td class="left">&#xa0;</td>
<td class="left">git commit</td>
</tr>


<tr>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="left">upload</td>
<td class="left">git push</td>
</tr>
</tbody>
</table>

### download THIS repository

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="right" />

<col  class="left" />

<col  class="left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="right">step</th>
<th scope="col" class="left">&#xa0;</th>
<th scope="col" class="left">the command</th>
</tr>
</thead>

<tbody>
<tr>
<td class="right">1</td>
<td class="left">open a terminal</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">2</td>
<td class="left">point inside the terminal</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">&#xa0;</td>
<td class="left">move to the desire directory</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">3</td>
<td class="left">download the respostory</td>
<td class="left">git clone <https://github.com/cmchaol/hello-world.git></td>
</tr>
</tbody>
</table>

### edit the local repository, git add, git commit

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="right" />

<col  class="left" />

<col  class="left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="right">step</th>
<th scope="col" class="left">&#xa0;</th>
<th scope="col" class="left">the command</th>
</tr>
</thead>

<tbody>
<tr>
<td class="right">1</td>
<td class="left">move inside the local repository</td>
<td class="left">cd hello-world</td>
</tr>


<tr>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">2</td>
<td class="left">edit the-specific-file</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">3</td>
<td class="left">git add the-specific-file</td>
<td class="left">git add the-specific-file</td>
</tr>


<tr>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">4</td>
<td class="left">commit the snapshot</td>
<td class="left">git commit -m "<message>"</td>
</tr>
</tbody>
</table>

git add

<https://www.atlassian.com/git/tutorials/saving-changes/git-add>

git commit 

<https://www.atlassian.com/git/tutorials/saving-changes/git-commit>

### upload the local snapshot to the remote github repository

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="right" />

<col  class="left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="right">step</th>
<th scope="col" class="left">&#xa0;</th>
</tr>
</thead>

<tbody>
<tr>
<td class="right">1</td>
<td class="left">inside the local repository</td>
</tr>


<tr>
<td class="right">&#xa0;</td>
<td class="left">&#xa0;</td>
</tr>


<tr>
<td class="right">2</td>
<td class="left">git push</td>
</tr>
</tbody>
</table>

git push 

<https://www.atlassian.com/git/tutorials/syncing/git-push>

### a typical script

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="left">A practicle cycle</th>
</tr>
</thead>

<tbody>
<tr>
<td class="left">git clone</td>
</tr>


<tr>
<td class="left">edit</td>
</tr>


<tr>
<td class="left">git add</td>
</tr>


<tr>
<td class="left">git commit</td>
</tr>


<tr>
<td class="left">git push</td>
</tr>
</tbody>
</table>

    git add hello-world-201410.org
    
    git commit -m "<another modification of hello-world-201410.org>"
    
    git push

## Caching your GitHub password in Git

<https://help.github.com/articles/caching-your-github-password-in-git>

    git config          credential.helper  cache
    
    git config --global credential.helper  cache
    
    git config --global credential.helper 'cache --timeout=3600'

# org mode

## synonym

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="left" />

<col  class="right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="left">&#xa0;</th>
<th scope="col" class="right">reference</th>
</tr>
</thead>

<tbody>
<tr>
<td class="left">orgmode</td>
<td class="right">1</td>
</tr>


<tr>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
</tr>


<tr>
<td class="left">org mode</td>
<td class="right">1</td>
</tr>


<tr>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
</tr>


<tr>
<td class="left">org-mode</td>
<td class="right">3</td>
</tr>


<tr>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
</tr>


<tr>
<td class="left">org</td>
<td class="right">2</td>
</tr>


<tr>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
</tr>


<tr>
<td class="left">&#xa0;</td>
<td class="right">&#xa0;</td>
</tr>
</tbody>
</table>

reference

1

<http://orgmode.org/>

2

<http://orgmode.org/manual/Summary.html#Summary>

3

<http://en.wikipedia.org/wiki/Org-mode>

## org export backends

c-h v org-export-backends

## org export Literal examples

<http://orgmode.org/manual/Literal-examples.html#Literal-examples>

    #+BEGIN_EXAMPLE
    Some example from a text file.
    #+END_EXAMPLE

For simplicity when using small examples, you can also start the example lines with a colon followed by a space. There may also be additional whitespace before the colon:

Here is an example

    Some example from a text file.

    Here is an example
       : Some example from a text file.

# R

## installation in gentoo

emerge -s %<sup>R</sup>$ 

These days, if you want a regex search, you have to prepend a "%" and the regex search is case sensitive. 

<http://forums.gentoo.org/viewtopic-t-129047.html>

man emerge

&#x2013;search (-s)
              Searches  for  matches of the supplied string in the portage tree.  By default emerge uses a case-insensitive simple search, but you can enable a regular expression search by prefixing the search string with %.  For example, emerge &#x2013;search "%<sup>kde</sup>" searches for any package whose name starts with "kde"; emerge &#x2013;search "%gcc$" searches for any package that ends with "gcc"; emerge &#x2013;search "office" searches for any package that contains the word "office".  If you want to include the category into the search string, prepend an @: emerge &#x2013;search "%@<sup>dev</sup>-java.\*jdk". If you  want  to  search the package descriptions as well, use the &#x2013;searchdesc action.

 emerge -s %<sup>R</sup>$ 
Searching&#x2026;    
[ Results for search key : ^R$ ]
[ Applications found : 1 ]

dev-lang/R
      Latest version available: 3.0.1
      Latest version installed: 3.0.1
      Size of files: 24,910 kB
      Homepage:      <http://www.r-project.org/>
      Description:   Language and environment for statistical computing and graphics
      License:       || ( GPL-2 GPL-3 ) LGPL-2.1

## ESS

emerge -s %<sup>ess</sup>$

[ Results for search key : ^ess$ ]
[ Applications found : 2 ]

app-emacs/ess
    Latest version available: 13.09
    Latest version installed: 13.09
    Size of files: 3,278 kB
    Homepage:      <http://ess.r-project.org/>
    Description:   Emacs Speaks Statistics
    License:       GPL-2+ GPL-3+ Texinfo-manual

app-xemacs/ess
    Latest version available: 1.03
    Latest version installed: [ Not Installed ]
    Size of files: 459 kB
    Homepage:      <http://xemacs.org/>
    Description:   ESS: Emacs Speaks Statistics
    License:       GPL-2

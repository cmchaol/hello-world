<http://git-scm.com/book/en/Git-on-the-Server-The-Protocols>

To clone a Git repository over SSH, you can specify ssh:// URL like this:

$ git clone ssh://user@server/project.git

Or you can use the shorter scp-like syntax for SSH protocol:

$ git clone user@server:project.git

git clone ssh://user@server/project.git

git clone user@server:project.git

> Everything should be made as simple as possible,
> but not any simpler &#x2013; Albert Einstein

for hello-world

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="left" />

<col  class="left" />
</colgroup>
<tbody>
<tr>
<td class="left">git clone ssh://cmchaol@github.com/hello-world.git</td>
<td class="left">failed</td>
</tr>


<tr>
<td class="left">git clone ssh://git@github.com/cmchaol/hello-world.git</td>
<td class="left">succeed</td>
</tr>


<tr>
<td class="left">git clone git@github.com:cmchaol/hello-world.git</td>
<td class="left">succeed</td>
</tr>
</tbody>
</table>

git clone ssh://cmchaol@github.com/hello-world.git
Cloning into 'hello-world'&#x2026;
Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

git clone ssh://git@github.com/cmchaol/hello-world.git

git clone git@github.com:cmchaol/hello-world.git

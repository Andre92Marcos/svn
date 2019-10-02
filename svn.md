**svn checkout**

svn checkout URL[@REV]... [PATH]
svn co URL[@REV]... [PATH]

	URL[@REV] : URL to the indentity that you want to download
	[PATH] : Path to the directory that you want to receive the files. Doesn’t need to exist



Examples:
	 svn co https://svn.ingg.com/svn/dev2/com/ingg/ikernel/level3/plugin/uc/ikernel-plugin-uc-egm-lbo-impl/trunk ./trunk/


**svn copy**

svn copy [PATH1] [PATH2]

	Copies PATH1 to PATH2.

	-m “message” ”: Commit message


**svn diff**

svn diff (di)

Display the differences between two paths. You can use svn diff in the following ways:

Use just svn diff to display local modifications in a working copy.


svn diff -r revOlder:revNewer svnPath

**svn merge**

	svn merge -r UPREV:LOWREV . undo range

	svn merge -c -REV . undo single revision


**svn revert**

This will not delete new files:
	svn revert -R .


**svn add**



Schedule files, directories, or symbolic links in your working copy for addition to the repository. They will be uploaded and added to the repository on your next commit. If you add something and change your mind before committing, you can unschedule the addition using svn revert.

**svn authentication**

Use 
--username myUsername --password myPassword


**svn commit**

svn commit -m “[MESSAGE]” [OPTIONAL PATH TO FILE]

**svn mkdir**

Create a new directory under version control.

    svn mkdir PATH...
    svn mkdir URL...

**svn resolve**

Resolve conflict with my edits:

    svn resolve --accept mine-full PATH/TO/FILE

Resolve conflict with their edits:

    svn resolve --accept theirs-full PATH/TO/FILE

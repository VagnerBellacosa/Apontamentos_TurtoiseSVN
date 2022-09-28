# How to Use TortoiseSVN for Beginners

[![Jessica Thornsby](https://secure.gravatar.com/avatar/5ed4eb479e5608b97eb523acc4699f7d?s=96&d=mm&r=g)](https://www.developer.com/author/jessica-thornsby/)

By[Jessica Thornsby](https://www.developer.com/author/jessica-thornsby/)

March 14, 2012

TortoiseSVN is a popular Apache Subversion client for Windows, implemented as a Microsoft Windows shell extension. As it isn’t integrated into a specific IDE it can be used with a range of development tools; for example, it can be integrated into Microsoft Visual Studio using a third-party plugin such as VisualSVN. The key benefits of using [TortoiseSVN](http://tortoisesvn.net/) include:

1. Icon overlays, which allow you to see the status of every versioned file and folder at a glance.
2. Easy access to all Subversion commands though a TortoiseSVN sub-menu that’s automatically added to the Windows context menu.
3. Windows integration, which allows you to work with tools you’re already familiar with.
4. Context-aware sub-menu — available commands are filtered based on the selected file or folder. You will not see any commands you cannot use within the current context.
5. Powerful commit dialog — with integrated spellchecker, auto completion capabilities, and the ability to double-click on a modified file to open the diff program.

TortoiseSVN also comes with some useful tools for version control:

- **TortoiseMerge** — a diff / merge tool that displays the changes made to particular files.
- **TortoiseBlame** — displays who is responsible for a particular change, and the log message for the corresponding commit.
- **TortoiseIDiff** — displays the changes made to image files, as it’s not possible to use a standard file diff tool for images. TortoiseIDiff can display two images side-by-side, and display images blended over one another.

## Getting Started with TortoiseSVN

TortoiseSVN is GNU General Public License software that you can download for free from [wandisco.com](http://www.wandisco.com/subversion/download#tortoise). It is available in both 32-bit and 64-bit flavors. To download TortoiseSVN, simply double click the installer file and follow the onscreen instructions. When prompted, click *Install*.

The first step when using TortoiseSVN, is to download a local working copy of your repository. Start by creating a directory where you will store the working copy. Right-click on the folder and the Explorer context menu will appear, along with some new TortoiseSVN commands. Select *SVN Checkout…’*

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_1.png)

This will open the checkout dialog:

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_2.png)

From here you can set the following properties:

- URL of Repository

   

  — the URL of the repository you wish to check out. (If you’re using

   

  uberSVN

  , you can copy/paste the repository URL from the repository screen.)

  ![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_3.png)

- **Checkout directory** — the location on your local file system where the checkout will occur. By default, it will be the location you right-clicked, but you can change this manually.

- **Checkout depth** — an option to limit what you check out. This is useful if you’re changing one directory of a very large repository.

- **Revision** — get the latest version of the repository. You can also select a specific revision, which is useful if you need to roll back to a version before particular changes were made.

When you’ve finished with these options, you’re ready to perform the checkout. Click *Ok*. You’ll now see the progress of the checkout. All the files and the folders that are included in the checkout will be logged.

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_4.png)

## Making and Committing Your Changes with TortoiseSVN

Now you have a working copy on your computer; you are free to work on your own, local version of the project. When you have finished making your changes, the modified files/directories will be shown with the red exclamation mark overlay to indicate that they have been modified since they were last checked out or updated.

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_5.png)

Before you commit any changes, it’s a good practice to ensure your working copy is up to date with the repository. To update your working copy, select the desired files or directories, right-click them and select *Update* from the TortoiseSVN sub-menu. A new screen will open displaying the update’s progress. Changes performed by other team members will be merged into your files, but any changes you may have performed on the same files will be maintained.

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_6.png)

Now that you’ve ensured your working copy is up to date, it’s time to add your changes to the repository. Select the desired files or directories and hit the *SVN Commit…* command.

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_7.png)

*SVN Commit…* will open the commit dialog. From here, you can perform a number of actions:

- Launch the external diff tool, which displays every change made to the file, by double clicking on any modified file.

  ![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_8.png)

- Add a log message from the commit dialog. It’s a good practice to leave a log message, as they can be useful if problems arise later.

  ![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_9.png)

- Keep a particular file from being committed by unchecking that file. Hit *Ok* to commit your changes to the repository.

## Hidden TortoiseSVN Features

You are now familiar with TortoiseSVN’s context menu, but did you know that if you hold down the shift key, you can access an extended context menu? This menu has some additional options:

### Diff with URL

A big part of project development is pinpointing what has changed. TortoiseSVN has a trick for uncovering exactly what has changed on the trunk for users working on a branch and what has changed on a specific branch for users working on the trunk. When you hold down the *Shift* button and select *TortoiseSVN*, you will notice a new *Diff with URL* option has appeared.

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_10.png)

Select *Diff with URL*. In the following dialog, specify the URL in the repository you wish to compare with your local file. This will bring up the TortoiseMerge box, allowing you to see the changes.

### Delete Unversioned Items

Another new option that appears when you hold down *Shift* is *Delete unversioned items*. It’s possible to set the TortoiseSVN ignore list to exclude all unversioned items, but if you wish to purge all these ignored items and produce a clean build, this command comes in handy. Selecting *Delete unversioned items* launches a dialog listing all the unversioned files in the working copy, where you can select which files to delete. Note that this command only moves files to the recycle bin, so they can be recovered if you make a mistake.

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_11.png)

### Break Lock

Although Subversion was designed to use copying and merging rather than locking, there are some scenarios where locking is advisable (e.g. whenever “unmergeable” files such as images are involved.) Locking with TortoiseSVN is a matter of clicking the file that requires locking, and selecting *Get Lock…* from the TortoiseSVN sub-menu. It’s also a good practice to leave a comment explaining why you have decided to lock that file.

If you can add locks, at some point you will need to release them. To release a lock manually with TortoiseSVN, select the locked file, press *Shift* and then select the new *Break Lock* option from the TortoiseSVN sub-menu. TortoiseSVN will then contact the repository and release the lock. You can also use this command on a folder to release all the locks recursively.

![Getting Started with TortoiseSVN](https://devcomprd.wpengine.com/wp-content/uploads/2021/03/TortoiseSVN_12.png)

## Further Reading

You now know the basic TortoiseSVN workcycle, and some additional “hidden” commands! If you want to learn more about TortoiseSVN, the [official docs](http://tortoisesvn.net/docs/release/TortoiseSVN_en/index.html) are a great source of information.
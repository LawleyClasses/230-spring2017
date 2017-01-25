# Week 1 Thursday Exercise (26 Jan 2017)

## Overview & Goals

In today's exercise, we will be taking a text document, marking it up as an HTML document, adding basic CSS formatting, and uploading it to your RIT web space. 

We will also be adding a configuration file to your RIT web space to override some of the server's (problematic) default behavior.

## Setting Up Your Folders and Files

On your computer (or on a USB drive) create a folder called banjo. Inside of the banjo folder, put a folder called www . Inside of the www folder, put a folder called 230. And inside of the 230 folder, put folder called week1. The www folder represents your www directory on banjo.rit.edu. The 230 folder is where all of your exercises and projects for this class will be stored. And the week1 folder is for today's exercise. 

I've put a file called [cremebrulee.txt](./weekly_materials/week1/cremebrulee.txt) in the week1 folder on Github. When you view that file on Github, you'll see that it's a plain text file with the content from the [Wikipedia entry for "Crème brûlée"](https://en.wikipedia.org/wiki/Cr%C3%A8me_br%C3%BBl%C3%A9e). 

To download that text file to your computer for editing, right-click on the button in the top right corner of the file that says "Raw," choose "Save link as...", and select the week1 folder that you created in the previous step as the download destination.

You're also going to the two images in the week1 folder. Go up one level in the repo to the week1 folder, and click on the first image (2014_0531_Crème_brûlée_Doi_Mae_Salong.jpg). When it loads, there will be a Download button in the top right corner. Right-click that button, choose "Save link as...", and download it to your local week1 folder. Then epeat that process with the second image, 225px-Crema_Catalana_El_Glop.jpg. 

## Marking Up a Text File

Launch Visual Studio Code, and choose "Open Folder..." from the file menu. Find the your week1 folder, and select it. You should now see the three files that you downloaded in the left sidebar. (If you don't, click on the documents icon in the top left corner of the window.)

Click on the cremebrulee.txt file, and it should display in the editor. It currently has no HTML markup at all--you're going to turn it into a proper HTML document, and add some simple CSS rules to make it look a bit more like the original Wikipedia entry. 

Start by creating a new file (File->New File, or Ctrl-N). Save the file (File->Save or Ctrl-S), name it cremebrulee.html, and make sure it's in your week1 folder. 

Add the basic structure for an HTML document. You can do this by hand, or you can use the Emmet abbreviation I showed at the end of Tuesday's class; type an !, then hit tab. 

Now copy all of the content from the .txt document, and paste it into the body of the .html document. (You can close the .txt file now if you want; we're done with it.) 

There are a lot of accented and foreign characters in this document, which browsers won't interpret properly. You need to turn those into HTML entities. Happily, there's an easy way to do this. If you don't already have the Hasher extension installed, go to the extensions pane (bottom icon in the far left sidebar, or choose View->Extensions) and install it (type Hasher in the search box, and then click the install button when it appears). Once it's installed, you can highlight a word or phrase that has special characters (e.g. ), press the F1 key, and type "Hasher HTML". You'll see two options appear-- Hasher: HTML Entity Decode, and Hasher: HTML Entity Encode. Select the Encode option, and it will replace the accented characters with the appropriate HTML entity codes. Repeat this for all the words/phrases in the document using special characters. (You can actually select all the text you copied over and run the command on that--but make sure you don't include any html tags, or it will turn the tag brackets into entities!)

Now go through the file and mark it up with HTML. 

- Add an h1 heading for the page title, and h2 headings for all of the subsections.
- Add paragraph tags to the individual paragraphs of text. 
- Make the Contents and References sections into numbered ("ordered") lists, and the See Also, Bibliography, and External Links sections into bulleted ("unordered") lists. (In class I'll show you a nice trick for this using Emmet.)
- Add the two images where indicated in the file. Don't worry about positioning them for now; we'll deal with that when we add the CSS. 
- Use the `<sup>` tag to make each of the footnote references a superscript.
- Where appropriate, add tags to make text bold (`<strong>...</strong>`) and/or italicized (`<em>...</em>`).

Don't worry about adding links yet; we'll be doing that next week. 

When you're done, use Ctrl-O to open your html file in Chrome (or another browser). It should look a lot like this: [cremebrulee1.png](cremebrulee1.png)

## Uploading
 
Once you're satisfied with the html file, you're going to upload the files you've been working on to your RIT web space. 

Using the SFTP program of your choice (the recommended option in the IGM labs is Filezilla), connect to the banjo.rit.edu server, and copy your entire 230 folder to your www directory on banjo. (I'll demo this in class.)

Test it by going to `http://people.rit.edu/yourid/230/week1` -- you should see the .txt and .html files, and the two images. Click on the html file and make sure it displays properly. If you run into problems here, **ask for help**!

Once your page has displayed properly, type Ctrl-U to display the page source. You'll probably see a big block of completely unfamiliar code near the top of your page, where your first image is embedded. In the next section, I'll explain where that came from, and how we can make it go away. 

## Fixing Banjo

banjo.rit.edu implements several techniques to help pages load faster and more consistently, but these technique have the side effect of making pages on the server very hard for us to debug and to validate.

The solution? We need to add an .htaccess files to your www directory.

.htaccess files allow you to make web server configuration changes on a per-folder
basis. The period at the beginning of the file name is intentional; it indicates a hidden file in UNIX. However, that same period can make the file difficult to work with on a Windows or Mac computer, so we're going to start with a file that does not include the period at the beginning of the name. We will be working with .htaccess files in more depth later in the semester, but for now we just want to get this file uploaded so that the server behaves properly for you.

(Note: If you already have an .htaccess file in your banjo www directory, rather than creating a new file as described below, simply add a line with the directive (ModPagespeed off) to the end of the existing file.)

1) In the www directory that you created on your local computer or USB drive, create a new file called htaccess, without the period at the beginning of the file name. In that file, put a single line of text:
   ModPagespeed off

2) Using an SFTP client to upload the htaccess file to the www folder in your banjo.rit.edu account.

3) Once you've uploaded the file, on Banjo, change its filename from htaccess to .htaccess (just add a . to the front of the name). 

4) Make sure you set the permissions on this file to 644 (Read and Write for you, Read only for group and other).

To see if this worked, reload your cremebrulee.html page, and try viewing the source again. 

## Adding Basic CSS Formatting
Now we're going to use CSS to start to make this look a bit more like the original Wikipedia entry.

In the head of your document, add a link to an external stylesheet called cremebrulee.css. 

```
<link rel="stylesheet" type="text/css" href="cremebrulee.css" />
```

Use File->New or Ctrl-N to create a new file, and save it to the week1 folder with the name cremebrulee.css.

For today, since we've already done quite a bit, I'm going to give you the CSS to start with. Paste the following style rules into your cremebrulee.css file:

```
body {
    font-family: 'Helvetica Neue','Helvetica','Nimbus Sans L','Arial','Liberation Sans',sans-serif;
    line-height: 1.4;
    padding-left: 20px;
}

a { text-decoration: none; }

h1, h2 {
    font-family: 'Linux Libertine',Georgia,Times,serif;
    line-height: 1.3;
    margin-bottom: 0.25em;
    padding: 0;
    border-bottom: 1px solid #a2a9b1;
    font-weight: normal;
    }

h1 {
    font-size: xx-large;
}
```
Save your HTML and CSS files, and upload them to your week1 directory. Your cremebrulee.html file should now look more like this: [cremebrulee2.png](cremebrulee2.png)

You're done!

## Due Date
You must have this exercise complete by 11:59pm on Friday, January 27th. On Saturday, my grader will go to `http://people.rit.edu/~youruserid/230/week1`, check to make sure all the files are there, and load the html file to make sure it bears some resemblance to what I asked for. 

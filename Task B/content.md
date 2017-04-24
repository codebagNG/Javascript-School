# Writing JavaScript

JavaScript code is typically embedded in the HTML, to be interpreted and
run by the client's browser. Here are some tips to remember when writing


## JavaScript commands.
* JavaScript code is case sensitive
* White space between words and tabs are ignored
* Line breaks are ignored except within a statement
* JavaScript statements end with a semi- colon ;


## The SCRIPT Tag


The <SCRIPT> tag alerts a browser that JavaScript code follows. It is typically embedded in the HTML.
<SCRIPT language = "JavaScript">
statements

SCRIPT Example
* Open "script_tag.html" in a browser.
* View the Source
* Put the cursor after

```</SCRIPT>
<! – Enter code below 􀃆 and enter the following:
<SCRIPT language = "JavaScript">
alert("Welcome to the script tag test page.")
</SCRIPT>```

* Save the changes by choosing Save from the File menu.
* Then Refresh the browser by clicking the Refresh or Reload button.


## Implementing JavaScript

There are three ways to add JavaScript commands to your Web Pages.
* Embedding code
* Inline code
* External file

#### External File

You can use the SRC attribute of the <SCRIPT> tag to call JavaScript code
from an external text file. This is useful if you have a lot of code or you
want to run it from several pages, because any number of pages can call the
same external JavaScript file. The text file itself contains no HTML tags. It
is call by the following tag:
```<SCRIPT SRC="filename.js">   </SCRIPT>```

#### External Example
* Open "external.html" in a browser
* View the Source
* Put the cursor after <! – Enter code here 􀃆 and enter:
```<SCRIPT language = "JavaScript" SRC = "external.js"> </SCRIPT>```

#### Save the changes and Refresh the browser.

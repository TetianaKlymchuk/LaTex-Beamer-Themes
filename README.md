# LaTex-Beamer-Themes
As a PhD student I have to give some presentations. I think I tried once to use Powerpoint to give a presentation filled with mathematical equations before I decided that this was not going to work ;)

After some other packages, I finally found LaTeX-Beamer. For the majority of the presentations the default styles provided with LaTeX-Beamer were sufficient, but every now and then I wanted to have a bit more, do I dare to say it, powerpoint like theme :)

I used LaTeX Beamer Themes from https://latex.simon04.net. Most of them are in fact had bugs and unclear descriptions or did not compile properly. I modified them in order to have an working code thus to use the style, you must first download the source from my GitHub repository, copy it into the texmf directory and make sure that you have run the texhash command under linux or the windows equivalent such that pdflatex is able to find the style files.

1. The first example is default style provided with LaTeX-Beamer, called **Berlin**:
![screenshot_1](https://cloud.githubusercontent.com/assets/28005338/25578777/b2d86c58-2e7a-11e7-96cb-a0131ecac081.png)
![screenshot_2](https://cloud.githubusercontent.com/assets/28005338/25578779/b5b62500-2e7a-11e7-9489-d881fa762e3d.png)

You do not need any additional style for this package, it is only needed to add:
```
\documentclass[usenames,dvipsnames]{beamer}
\usetheme{berlin}
```
in the preamble of you file. Also I use in the example
```
\setbeamertemplate{navigation symbols}{}
```
which hides navigation symbols (who does still use them? :)) And
```
\includegraphics<1>[height=1.2cm]{configuracion_1.png}
```
in order to show how to add your own logo. For this reason it is needed to keep with your tex-file all the pictures that you've used in your presentation.

2. The second example is  called **Gelugor** style, which has been modified using style from https://latex.simon04.net.
![screenshot_3](https://cloud.githubusercontent.com/assets/28005338/25579023/d0e7d952-2e7c-11e7-8af7-afbee61095dc.png)
![screenshot_4](https://cloud.githubusercontent.com/assets/28005338/25579024/d36a1848-2e7c-11e7-9c75-4ddf9263bfa1.png)

It is needed to add beamerthemeGelugor.sty and the following command in the preamble (it also possible use an example tex-file and manually change these commands):
```
\title{Title}
\subtitle{Subtitle}
\author{Author}
\date{\today}
\institute{\url{aa@ua.edu}\\\url{http://www.aaa.edu/}}
```
I also add an additional title page without using automatic title page, but created manually. For this reason I keep all graphics together with file.tex and style.sty.
3. The third example is very nice and spring theme, called **Intridea**:
![screenshot_5](https://cloud.githubusercontent.com/assets/28005338/25579169/006cb228-2e7e-11e7-825f-e15f2871a342.png)
![screenshot_6](https://cloud.githubusercontent.com/assets/28005338/25579170/021d0258-2e7e-11e7-893b-a58dc3353a3b.png)

I also have added some logotypes, which are not in the style, but were added manually in case it is needed to change a logo.
For this reason all files together are required for a proper work of a Presentation.

4. The last example is dark theme, called **Kalgan**:
![screenshot_7](https://cloud.githubusercontent.com/assets/28005338/25579234/b678e6cc-2e7e-11e7-8596-c7d2ae529318.png)
![screenshot_9](https://cloud.githubusercontent.com/assets/28005338/25580327/d7597eec-2e88-11e7-803e-55aeb9db4b4e.png)

I have no idea who can use those theme for Presentation. Maybe, if one have a lot of white images which are needed to stand out.
Nevertheless, this theme looks cool and it worth to show it here.
```
\documentclass[usenames,dvipsnames]{beamer}
\usetheme{Kalgan}
\usefonttheme[onlylarge]{structurebold}
\setbeamerfont*{frametitle}{size=\normalsize,series=\bfseries}
\setbeamertemplate{navigation symbols}{}
```
and file beamerthemeKalgan.sty is needed.

I am open for any suggestions and contributions!

Dieses Paket beinhaltet ein interaktives R Problem Set, welches auf dem Paket RTutor basiert (https://github.com/skranz/RTutor). 

Das Problem Set beschäftigt sich mit dem Artikel "Texting Bans and Fatal Accidents on Roadways: Do They Work? Or Do Drivers Just React to Announcements of Bans?" von Abouk und Adams (2013). Ziel ist es, den Effekt von SMS-Verboten auf tödliche Verkehrsunfälle mithilfe des Difference-in-Differences-Ansatzes zu untersuchen. Dazu werden sowohl deskriptive Analysen als auch Regressionsanalysen durchgeführt und die Ergebnisse der Autoren repliziert. Den vollständigen Artikel finden Sie unter folgendem Link:
https://www.aeaweb.org/articles?id=10.1257/app.5.2.179.


## 1. Installation

RTutor und dieses Paket werden auf Github gehostet. Um alles zu installieren, führen Sie den folgenden Code in Ihrer R-Konsole aus.
```s
install.packages("RTutor",repos = c("https://skranz-repo.github.io/drat/",getOption("repos")))

if (!require(devtools))
  install.packages("devtools")

devtools::install_github("selenyagci/RTutorSMSVerbot")
```

## 2. Anzeigen und Bearbeiten des Problem Sets
Um mit dem Problem Set zu starten, erstellen Sie zunächst ein Arbeitsverzeichnis, in dem Dateien wie Datensätze und Ihre Lösung gespeichert werden. Passen Sie anschließend den folgenden Code an und führen ihn aus.
```s
library(RTutorSMSVerbot)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorSMSVerbot")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorSMSVerbot",
       auto.save.code=TRUE, clear.user=FALSE)
```
Wenn alles gut funktioniert, sollte sich ein Browserfenster öffnen. Sie können nun mit der Bearbeitung des Problem Sets starten.

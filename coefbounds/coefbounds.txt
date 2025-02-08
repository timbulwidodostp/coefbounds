# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Nonparametric Bounds for Regression with Interval-Censored Outcomes Use coefbounds With (In) R Software
install.packages("remotes")
remotes::install_github("brentonk/coefbounds")
library("coefbounds")
coefbounds = read.csv("https://raw.githubusercontent.com/timbulwidodostp/coefbounds/main/coefbounds/coefbounds.csv",sep = ";")
# Estimation Nonparametric Bounds for Regression with Interval-Censored Outcomes Use coefbounds With (In) R Software
Dependen_1 <- coefbounds$Dependen_1
Dependen_2 <- coefbounds$Dependen_2
Independen_1 <- coefbounds$Independen_1
Independen_2 <- coefbounds$Independen_2
coefbounds_1 <- coefbounds(Dependen_1 + Dependen_2 ~ 1, boot = 0)
coefbounds_1
coefbounds_2 <- coefbounds(Dependen_1 + Dependen_2 ~ Independen_1 + Independen_2, boot = 10)
coefbounds_2
# Nonparametric Bounds for Regression with Interval-Censored Outcomes Use coefbounds With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
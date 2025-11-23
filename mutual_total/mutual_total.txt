# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Calculates the Mutual Information Index M and Theil's Entropy Index H use mutual_total (segregation) With (In) R Software
install.packages("segregation")
library("segregation")
mutual_total = read.csv("https://raw.githubusercontent.com/timbulwidodostp/mutual_total/main/mutual_total/mutual_total.csv",sep = ";")
# Estimation Calculates the Mutual Information Index M and Theil's Entropy Index H use mutual_total (segregation) With (In) R Software
mutual_total(mutual_total, "school", "race", weight = "n")
mutual_total(mutual_total, "race", "school", weight = "n")
mutual_total(mutual_total, "race", c("district", "school"), weight = "n")
mutual_total(mutual_total, "race", "school", weight = "n", se = TRUE, n_bootstrap = 1000)
mutual_total(mutual_total, "race", "school", within = "district", weight = "n") 
mutual_total(mutual_total, "race", "district", weight = "n")
# Calculates the Mutual Information Index M and Theil's Entropy Index H use mutual_total (segregation) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
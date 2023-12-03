# Example of README.md
dat=mtcars
pmatrix=scale(dat)
d=dist(pmatrix)
c=hclust(d,method = "ward.D2")
plot(c)
rect.hclust(c,k=2)
groups<-cutree(c,k=2)
table(mtcars$carb,groups)

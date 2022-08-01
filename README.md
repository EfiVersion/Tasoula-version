# Example of README.md
##R script for mtcars Hierarchical Cluster
?mtcars
dat = mtcars
pmatrix = scale(dat)
d = dist(pmatrix)
c = hclust(d, method = "ward.D2")
plot(c)
rect.hclust(c, k=4)

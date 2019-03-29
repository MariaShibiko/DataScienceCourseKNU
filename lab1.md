В лабораторній роботі необхідно виконати наступні дії:
  1. Створити змінні базових (atomic) типів. Базові типи: character, numeric,
integer, complex, logical.


```{r}
compl <- 78+7i
print(compl)
[1] 78+7i

charac<- "ddoof"
print(charac)
[1] "ddoof"
numer<-728.728
print(numer)
[1] 728.728
integ<-8746L
print(integ)
[1] 8746
logic<-8
logic
[1] 8
```
2. Створити вектори, які: містить послідовність з 5 до 75; містить числа 3.14,
2.71, 0, 13; 100 значень TRUE.
```{r}
logic<-FALSE
logic
[1] FALSE
vect<-c(5:75)
vect
[1]  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47 48 49
[46] 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71 72 73 74 75
vect_2<-c(3.14, 2.71, 0,13)
vect_2
[1]  3.14  2.71  0.00 13.00
logical<-TRUE
vect<-vector("logical",lenth=100)

```
Створити наступну матрицю за допомогою matrix, та за допомогою cbind
або rbind
0.5 1.3 3.5
3.9 131 2.8
0 2.2 4.6
2 7 5.1
```{r}
a<-c(0.5, 1.3, 3.5)
b<-c(3.9, 131, 2.8)
d<-c(0, 2.2, 4.6)
e<-c(2, 7, 5.1)
cbind(a,b,d,e)
a     b   d   e
[1,] 0.5   3.9 0.0 2.0
[2,] 1.3 131.0 2.2 7.0
[3,] 3.5   2.8 4.6 5.1
rbind(a,b,d,e)
[,1]  [,2] [,3]
a  0.5   1.3  3.5
b  3.9 131.0  2.8
d  0.0   2.2  4.6
e  2.0   7.0  5.1
```
4. Створити довільний список (list), в який включити всі базові типи
```{r}
listnew <- list(charac, numer, integ, compl, logic)
listnew
[[1]]
[1] "ddoof"
a
[[2]]
[1] 728.728

[[3]]
[1] 8746

[[4]]
[1] 78+7i

[[5]]
[1] 8
```
5. Створити фактор з трьома рівнями «baby», «child», «adult»

```{r}
fact <- c(0,2,2,0,1,0,2,2)
fact <- factor(fact, levels=c(0,1,2))
levels(fact) <-c("baby", "child", "adult")
fact
[1] baby  adult adult baby  child baby  adult adult
Levels: baby child adult
```

# Matrix-multiplication
X = [[8, 5, 1],
     [9, 3, 2],
     [4, 6, 3]]
Y = [[8, 5, 3],
     [9, 5, 7],
     [9, 4, 1]]
result = [[0 for _ in range(len(Y[0]))] for _ in range(len(X))]
for i in range(len(X)):
    for j in range(len(Y[0])):
        for k in range(len(Y)):
            result[i][j] += X[i][k] * Y[k][j]
print("Result of matrix multiplication:")
for row in result:
    print(row)

OUTPUT:
Result of matrix multiplication:
[107, 70, 52]
[111, 74, 50]
[102, 58, 49]

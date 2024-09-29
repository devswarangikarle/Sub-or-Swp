# Sub-or-Swp

You are given two positive integers X and Y. Repeat the following operation until X is not 0:
If X > Y, swap X and Y;
Otherwise, set X = (Y − X) and Y = X.
Output the final value of Y after all operations.

import sys
import math

input = sys.stdin.read
data = input().splitlines()

T = int(data[0])
results = []

for i in range(1, T + 1):

    X, Y = map(int, data[i].split())
    results.append(math.gcd(X, Y))

sys.stdout.write("\n".join(map(str, results)) + "\n")

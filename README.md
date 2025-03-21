# Largest-Exponential
import math
v = [tuple(map(int, input().split())) for _ in range(int(input()))]
v = [(e * math.log(b), b, e) for b, e in v]

K = int(input())
_, b, e = sorted(v)[K-1]
print(b, e)	

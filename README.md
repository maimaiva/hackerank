# hackerank

### Company Logo
Count number of characters in the words, print top 3 

'''
import math
import os
import random
import re
import sys
import collections

s = sorted(input().strip())
s_counter = collections.Counter(s).most_common()
#print(s_counter)
s_counter = sorted(s_counter, key=lambda x: (x[1] * -1, x[0]))

for i in range(0, 3):
    print(s_counter[i][0], s_counter[i][1])

'''

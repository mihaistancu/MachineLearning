# MachineLearning
# Nuralnetwork

# MY CODE HERE:

In [1]:
X = [['Sunny','Warm','Normal','Strong','Warm','Same','+'],
 ['Sunny','Warm','High','Strong','Warm','Same','+'],
 ['Rainy','Cold','High','Strong','Warm','Change','-'],
 ['Sunny','Warm','High','Strong','Cool','Change','+']]
In [2]:
h = ['0','0','0','0','0','0']
In [3]:
def positiveInstances():
    return [x for x in X if x[-1]=='+']
In [8]:
for x in positiveInstances():
    for i in range(len(h)):
        if h[i]!=x[i]:
            if h[i]=='0':
                h[i]=x[i]
            else:
                h[i]='!'
In [9]:
h
Out[9]:
['Sunny', 'Warm', '!', 'Strong', '!', '!']
Implement List-Then-Eliminate and Candidate Elimination below

In [ ]:

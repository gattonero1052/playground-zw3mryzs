# List
Using Sample List: 3,1,5,4,1,-2

## Create
destructuring(unpack)
```python runnable
# destructuring
[a,b,c,d] = [[3],1,5,4]
print([a,b,c,d])
```

## Slice
```python runnable
# slice from 1 to 3
ls = [3,1,5,4,1,-2]
print(ls[1:3])

# slice from 1 to end
print(ls[1:])

# slice from start to 3
print(ls[:3])
```

## Max
```python runnable
ls = [3,1,5,4,1,-2]
print(max(ls))
```

## Distinct
```python runnable

# keep order
ls = [3,1,5,4,1,-2]
d = dict(zip(set(ls),[1]*len(ls)))
for x in ls:
    if d[x]==0:
        del ls[x]
    else:
        d[x]-=1
print(ls)
# throw order
ls = [3,1,5,4,1,-2]
print(list(set(ls)))
```

## Concat
```python runnable
ls = [3,1,5,4,1,-2]
print(ls + ls)
```

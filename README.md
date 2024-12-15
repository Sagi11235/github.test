# Online Python compiler (interpreter) to run Python online.
# Write Python 3 code in this online editor and run it.
def longest_substring(digits):
  n=[]
  for i in range (0,len(digits)-1):
    if int(digits[i])%2==int(digits[i+1])%2:
      n=[n,i]
  p=[]
  for i in range (0,len(n)):
      if i>0:
        p=[p,n(i)-n(i-1)]
      else:
          p=[p,n(i)]
  m=0
  for i in range (0, len(p)):
    if n(i)!=max(p):
      m+=p(i)
    else:
      break
  return digits[m:m+max(p)]
  
print(longest_substring("844929328912985315632725682153"))

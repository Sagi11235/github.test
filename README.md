# github.test
def longest_substring(digits):
  n=[]
  for i in range [0,len(digits)-1]:
    if digits(i)%2==digits(i+1)%2:
      n=[n,i]
  m=0;
  for i in range [0, len(n)]:
    if n(i)!=max(n):
      m+=n(i)
    else:
      break
  return digits[m:m+max(n)]

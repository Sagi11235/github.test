# github.test
def longest_substring(digits):
  n=[]
  for i=0:1:len(digits)-1
    if digits(i)%2==digits(i+1)%2
      n=[n,i]
  m=0;
  for i=0:1:len(n)
    if n(i)!=max(n)
      m+=n(i)
    else
      brake
  return digits[m:1:m+max(n)]

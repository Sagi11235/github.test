# Online Python compiler (interpreter) to run Python online.
# Write Python 3 code in this online editor and run it.
def longest_substring(digits):
  place1=0
  place2=0
  dp=0
  dp_max=0
  n=0
  for i in range (-1,len(digits)):
    if i==len(digits)-1 or int(digits[i])%2==int(digits[i+1])%2:
       place1=place2
       place2=i
       dp=place2-place1
       if dp_max<dp:
         n=place1
         dp_max=dp
  return digits[n+1:n+dp_max+1]
  
print(longest_substring("2846286484444288886666448822244466688822247"))

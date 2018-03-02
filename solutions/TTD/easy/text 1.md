## TEXT 1 
 For the beginning we are given easy crypto stuff : - 
 **CRYPTO** 
 	   `131017171A48221A1D170F` 
 	     and we are given an input field now by using that field  we can find that
 	     *a = 0c 
 	     b= 0d* 
 	     and so on ...
 	     so we find the      the whole character set  [*0-9 a-z A-Z - _ . , ; : ? ! [space]*] 
and we that to decode the *crypto*

def split(str, num):
    return [ str[start:start+num] for start in range(0, len(str), num) ]
a = "131017171A48221A1D170F"
b = split(a,2)
b2=("02030405060708090A0B0C0D0E0F101112131415161718191A1B1C1D1E1F202122232425"+
    "262728292A2B2C2D2E2F303132333435363738393A3B3C3D3E3F404142434445464748")
b2l = split(b2,2)
b3=("0123456789abcdefghijklmnopqrstuvwxyz"+
    "ABCDEFGHIJKLMNOPQRSTUVWXYZ-_.,;:?! ")
b3l=[]
for i in range(0,len(b3)):
    b3l.append(b3[i])
ans=''
for i in b:
    print i in b2l
    if(i in b2l):
        ans += b3l[b2l.index(i)]
    print "------->>>>",ans

    
     	     

 	      




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTI5ODE0Mzk3N119
-->

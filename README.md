# ipein
@author: atta hilali
"""
def creer_file():
    p=[]
    return p
def emfiler(p,x):
    p.append(x)
    return p
def defiler(p,x):
    p.remove(x)
    return p
def sommet(p):
    return p[0]
def intro(f2,f3,f5,k):
    if k==sommet(f2):
        defiler(f2,k)
    if k==sommet(f3):
        defiler(f3,k)
    if k==sommet(f5):
        defiler(f5,k)

#programme principale
n=30
f2=creer_file()
f3=creer_file()
f5=creer_file()
emfiler(f3,1)
emfiler(f2,1)
emfiler(f5,1)
while 1:
    k=min(sommet(f2),sommet(f3),sommet(f5))
    print(k)
    intro(f2,f3,f5,k)
    if k<n:
        emfiler(f3,3*k)
        emfiler(f2,2*k)
        emfiler(f5,5*k)
    else:
        break

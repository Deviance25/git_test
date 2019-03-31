# git_test

############# Использование метода ZipFile #############

from zipfile import ZipFile

src = 'E:\\Books\Python-dly-detey.pdf'
zFile = 'E:\\archive_Books.zip'
zf = ZipFile(zFile, 'w')
zf.write(src)
zf.close()



############# Задача по чтению файла #############


#d = []
#sm = 0
#t = {}
#with open ("test.txt", "r") as files:
#    for line in files:
#        d.append([line.strip()])
#print(d)

l = []
d = {}
with open("test.txt", 'r') as s:
    for i in s:
        l.extend([i.strip().split(';')])
#print(l)
for i in l:
    d[i[0]] = i[1:]
#print(d)


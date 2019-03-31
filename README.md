# git_test


d = []
sm = 0
t = {}
with open ("test.txt", "r") as files:
    for line in files:
        d.append([line.strip()])
print(d)

for i in d[1:]:
    t[]


############# Использование метода ZipFile #############

from zipfile import ZipFile

src = 'E:\\Books\Python-dly-detey.pdf'
zFile = 'E:\\archive_Books.zip'
zf = ZipFile(zFile, 'w')
zf.write(src)
zf.close()

######################################################

############# Задача по чтению файла #############
lst = []
sred = []
fst = []
scnd = []
thr = []
with open("test.txt", 'r') as s:
    for line in s:
        lst.extend([line.strip().split(';')])
for i in lst:
    sred.extend((int(i[1]))*2)
    fst.extend([int(i[1])])
    scnd.extend([int(i[2])])
    thr.extend([int(i[3])])
f = open("1.txt", "w+")
for i in sred:
    print (i, file = f)
print ((sum(fst)/len(fst)), (sum(scnd)/len(scnd)), (sum(thr)/len(thr)), file = f)


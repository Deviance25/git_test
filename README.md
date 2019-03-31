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

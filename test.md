## 制作过程
1. 将学号姓名放到name.txt
2. python LSBSteg.py encode -i lain.png -o half.png -f name.txt
3. 压缩half.png->half.zip
4. cat test1.png half.zip > test.png

## 解密过程
1. unzip test.png
2. python LSBSteg.py decode -i half.png -o result.txt



```css
   基本格式 （各种参数+多个文件～支持多线程）
   
   fastqc [-o output dir] [--(no)extract] [-f fastq|bam|sam] seqfile1 .. seqfileN
   
   -o --outdir FastQC生成的报告文件的储存路径
   --extract 使用这个参数是让程序不打包【默认会打包成一个压缩文件】
   -t --threads 选择程序运行的线程数，每个线程会占用250MB内存（一般与文件数量一致就好）
   -q --quiet 安静运行模式【不选这个选项，程序会实时报告运行的状况】
```
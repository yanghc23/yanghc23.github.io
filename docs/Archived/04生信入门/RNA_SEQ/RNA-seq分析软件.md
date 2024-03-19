TopHat    
cufflinks
HISAT
StringtTie
balldown
![[Pasted image 20230821135855.png]]



## RNA 原始数据质控

### 软件 FASTAP
![[Pasted image 20230821140042.png]]
![[Pasted image 20230821140144.png]]
  常用的是 fastqc


### 比对  ：  HISAT2

![[Pasted image 20230821140248.png]]

路径设置
![[Pasted image 20230821140340.png]]

### 基因表达定量： StringTie

![[Pasted image 20230821140812.png]]


![[Pasted image 20230821140900.png]]

### 质控  RSeQC

1. 首先可以对 bam 文件进行一个全面的统计  

![[Pasted image 20230821142543.png]]

2. 计算 FPKM
![[Pasted image 20230821142617.png]]

![[Pasted image 20230821142634.png]]

![[Pasted image 20230821142700.png]]

![[Pasted image 20230821142726.png]]


###  RPKM  FPKM
先处理深度，在处理长度
![[Pasted image 20230821142846.png]]

### TPM
先处理长度，后处理深度
![[Pasted image 20230821142940.png]]


### 差异表达分析  DESeq2

![[Pasted image 20230821170118.png]]

### 基因名称注释  DESseq
![[Pasted image 20230821170323.png]]

### 富集分析 Reactome

![[Pasted image 20230821170644.png]]


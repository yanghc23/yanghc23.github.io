PPT 文件在 /project/sw_R

## H3K4me3 
用来标记启动子的

## H3K4me1
增强子和超级增强子的活性标记

## H3K27ac （乙酰化）
增强子、超级增强子的标记，很常用

## chip-seq 的流程

![Pasted image 20230809153700.png](Pasted image 20230809153700.png)
### sra-tools
用于操作 SRA 数据的工具一般用于下载 SRA 文件，从 SRA 文件中提取 fastq 文件，查看 SRA 文件信息等

### Bowtie2
一个快速、省内存的将短序列比对至模板基因组的工具。尤其擅长于将 50~100 个核苷酸大小的短序列比对到基因组上

![Pasted image 20230809152657.png](Pasted image 20230809152657.png)

## samtools
用于 SAM 格式的后处理对其的各种实用程序，例如索引、变体调用方和对齐查看器，从而提供了用于处理读取对齐的通用工具。sam 格式是一种序列比对之后输出格式 

## Picard
此工具在 BAM 或 SAM 文件中查找并标记重复读取，起哄重复读取倍定义为源自单个 DNA 片段。Mark 重复工具的工作原理是比较 SAM/BAM 文件中读取和读取对的 5 个素数位置的序列。提供 BARCODE_tag 选项，便于使用分子条形码进行重复标记。收集重复读取后，该工具使用一种算法来区分主要读取和重复读取，该算法按其基本质量分数的综合对读取进行排名。

## Macs2
根据经验对 Chip-seq 标签的偏移大小进行建模，并使用它来提高预测结合位点的空间分辨率。MACS 还使用动态泊松分布来有效地捕获基因组中的局部偏差，从而实现更可靠的预测。

![Pasted image 20230809154744.png](Pasted image 20230809154744.png)

## deeptools
基于 Python 开发，适用于有效处理分析高通量测序数据，可用于 chip-seq、rna-seq、MNase-seq

## ROSE
通过 bam 文件以及 gff 文件寻找 enhancer 及其相关基因的工具，由 python 编写

首先识别增强子区域，然后对增强子进行合并，定义一个阈值，将距离小于该与之的增强子进行合并，最后比较合并后的增强子区域内的 reads 分布情况来识别超级增强子

## 单末端测序和双末端测序的区别

![Pasted image 20230809152657.png](Pasted image 20230809152657.png)

## 参考基因组的下载
[https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/hg19.fa.gz](https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/hg19.fa.gz)

![Pasted image 20230809153050.png](Pasted image 20230809153050.png)

# h23_project

Ссылка на [Google Colab](https://colab.research.google.com/drive/1BHbbg3IoSVPjDG3vO1MH5n7uapZGYDjq?usp=sharing)  
Тот же файл на [github](https://github.com/XeniaMishina/h23_project/blob/main/data/bioinf_project.ipynb)

## KDM6A

## Описание 
- product: H3K27
- f: деметилирует "Lys-27" гистона H3, тем самым играя центральную роль в гистоновом коде
- комплекс: CHD8, MLL2/3, MLL4/WBP7, COMPASS-like MLL3,4
- ткани: костный мозг, щитовидная железа, эндометрий, яичники и др.
- домены: JmjC, TPR 

![Expression](https://github.com/XeniaMishina/h23_project/blob/main/data/Expression.png)

### Статьи
- [Synergistic triad epistasis of epigenetic H3K27me modifier genes, EZH2, KDM6A, and KDM6B, in gastric cancer susceptibility](https://link.springer.com/article/10.1007/s10120-018-0888-9)
- [UTX/KDM6A Loss Enhances the Malignant Phenotype of Multiple Myeloma and Sensitizes Cells to EZH2 inhibition](https://www.sciencedirect.com/science/article/pii/S2211124717313839)
- [Loss of KDM6A/UTX Function Is a Common Event in a Mouse Model of Multiple Myeloma, Human Cell Lines and Patients.](https://www.sciencedirect.com/science/article/pii/S000649711953419X)
- [Uniprot](https://www.uniprot.org/uniprotkb/O15550/entry)
- [Wikipedia](https://en.m.wikipedia.org/wiki/UTX_(gene))

## Выравнивание гистонов

### H2A
![H2A](https://github.com/XeniaMishina/h23_project/blob/main/histones/H2A.png)

### H2B
![H2B](https://github.com/XeniaMishina/h23_project/blob/main/histones/H2B.png)

### H3
![H3](https://github.com/XeniaMishina/h23_project/blob/main/histones/H3.png)

### H4
![H4](https://github.com/XeniaMishina/h23_project/blob/main/histones/H4.png)

Практически все последовательности всех гистонов являются копиями друг друга или очень похожи (в пределах одного гистона), поэтому можем взять по одной последовательности в каждом гистоне.

## Blastp

Делаем blastp для всех гистонов и белка KDM6A для 11 организмов, получаем evalue.

Пример команды:  
`blastp -query my_histones/H2A.fasta -db proteomes/tuberculosis.faa  -out hblasts/tuberculosisH2A.blast -outfmt 7`

(В [Google Colab](https://colab.research.google.com/drive/1BHbbg3IoSVPjDG3vO1MH5n7uapZGYDjq?usp=sharing)   в начале есть код для перебора всех команд для ввода в терминал.)





this is some info of d3 array.
统计方法

搜索方法

转换方法（Transformations）

d3.cross(a,b[,reducer])
reducer函数指明数组a和数组b的元素组合方式

d3.merge(arrays)
和js原生的concat方法类似，但这个更方便

d3.pairs(array[,reducer])
对数组内相邻元素执行reducer函数，返回新形成的数组，默认是两两结合

d3.permute(array,indexes)
接受一个数组或者可以转成数组的对象，以及一个数组的索引或者对象的key值数组，返回对应索引或者value组成的数组

d3.shuffle(array[,lo[,hi]])
随机排序一个数组

d3.ticks(start,stop,count)
d3.tickIncrement(start,stop,count)
d3.tickStep(start,stop,count)

d3.range([start,]stop[,step])
返回一个范围数组，以start开始，默认是0，以step为间隔，默认是1

d3.transpose(matrix)
使用zip操作二维矩阵变换

d3.zip(arrays...)
返回arrays构成的矩阵的每一列组成的数组

柱状图方法（Histograms）

d3.histograms()
使用默认配置构造一个柱状图生成器

histogram(data)
histogram.value([value])
histogram.domain([domain])
histogram.thresholds([count])
histogram.thresholds([thresholds])

柱状图临界值方法（Histogram Thresholds）
d3.thresholdFreedmanDiaconis(values, min, max)
d3.thresholdScott(values, min, max)
d3.thresholdSturges(values)

d3-color

d3.color(specifier)
specifier可以是CSS3中的颜色名或者rgb值hsl值等等，返回一个rgb或者hsl颜色
color.opacity
颜色的不透明度
color.rgb()
返回rgb表示的颜色值
color.brighter([k])
返回颜色值的一个亮度的拷贝，如果k提供了，则控制返回的颜色值的亮度应该是多少，如果没提供，默认为1
color.darker([k])
类似color.brighter([k])
color.displayable()
当且仅当硬件可显示该颜色时返回true
color.toString()
根据CSS对象模型返回一个字符串，如果含有硬件无法显示该颜色，一个修正的颜色将被返回

d3.rgb(r,g,b[,opacity])
d3.rgb(specifier)
d3.rgb(color)

d3.hsl(h,s,l[.opacity])
d3.hsl(specifier)
d3.hsl(color)

d3.lab(l,a,b[,opacity])
d3.lab(specifier)
d3.lab(color)

d3.hcl(color)
……d3还支持一些其他颜色空间

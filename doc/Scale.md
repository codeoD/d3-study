Continuous Scales：

continuous(value)
从range中返回一个给定domain对应的值 \n
continuous.invert(value)
从domain中返回一个给定range对应的值,这个方法仅支持range是数值型的情况，否则返回NaN \n
continuous.domain([domain])
设置比例尺的域
continuous.range([range])
设置比例尺的范围
continuous.rangeRound([range])
等同于continuous.range(range).interpolate(d3.interpolateRound)
continuous.clamp(clamp)
使continuous(value)和continuous.invert(value)返回的值总在范围和域内
continuous.interpolate(interpolate)
continuous.ticks([count])
从域中返回大约count个数值，其具有相同间隔
continuous.tickFormat([count[, specifier]])
返回一个格式化函数
continuous.nice([count])
扩展domain，使开始和结束值具有合适边界 nice round
continuous.copy()
返回这个scale的一个copy，深拷贝，修改互不影响

linear scale

d3.linearScale()
Constructs a new continuous scale with the unit domain [0, 1], the unit range [0, 1], the default interpolator and clamping disabled

power scale

d3.scalePow()
Constructs a new continuous scale with the unit domain [0, 1], the unit range [0, 1], 
the exponent 1, the default interpolator and clamping disabled

log scale

d3.scaleLog()
Constructs a new continuous scale with the domain [1, 10], the unit range [0, 1], 
the base 10, the default interpolator and clamping disabled.

identity scale

d3.scaleIdentity()
Constructs a new identity scale with the unit domain [0, 1] and the unit range [0, 1].

time scale

d3.scaleTime()
Constructs a new time scale with the domain [2000-01-01, 2000-01-02], 
the unit range [0, 1], the default interpolator and clamping disabled.

Sequential Scales:

和continuous相似，但是输出的range是固定的，不可配置的，也米有暴露出 invert, range, rangeRound, interpolate这些方法 
d3.scaleSequential(interpolator)
用给定的interpolator函数构造一个新的scale
……
d3.interpolateViridis(t)
d3.interpolateInferno(t)
d3.interpolateMagma(t)
d3.interpolatePlasma(t)
d3.interpolateWarm(t)
d3.interpolateCool(t)
d3.interpolateRainbow(t)
d3.interpolateCubehelixDefault(t)

Quantize Scales：

和linear scale 相似，但是使用离散的range

quantize scale

d3.sacleQuantize()
Constructs a new quantize scale with the unit domain [0, 1] and the unit range [0, 1]. 
Thus, the default quantize scale is equivalent to the Math.round function.

quantize.invertExtent(value)
返回给定值对应的range

quantile scale

d3.scaleQuantile()
Constructs a new quantile scale with an empty domain and an empty range. 
The quantile scale is invalid until both a domain and range are specified.

threshold scale

d3.scaleThreshold()
Constructs a new threshold scale with the default domain [0.5] and the default range [0, 1]. 
Thus, the default threshold scale is equivalent to the Math.round function for numbers; 
for example threshold(0.49) returns 0, and threshold(0.51) returns 1.











dom
init(dom)
setOption({})

### title

1. text
2. textStyle
3. subtext
4. subtextStyle
5. show
6. left

### grid

1. top

### tooltip

1. trigger
2. backgroundColor
3. borderColor
4. borderWidth
5. textStyle

### legend

1. left
2. icon
3. top
4. itemHeight
5. textStyle

### xAxis

1. name
2. data
3. boundaryGap // 边界留白
4. axisLabel {margin, rotate}
5. axisTick
6. axisLine

### yAxis

1. name
2. splitNumber
3. interval
4. minInterval
5. maxInterval
6. data
7. axisLabel

### series

[]
{}

1. name
2. data
3. type
4. markPoint data { type } { coord: [x,y], value}
5. markLine data { type } [ {coord}, {coord} ]

### visualMap

1. min
2. max
3. inRange { color:[], colorLightness: [0,1] }

### radar

1. indicator '' [{min,max,color,value,name}]
2. shape
3. splitArea { areaStyle }
4. splitLine { lineStyle }
5. axisLine { lineStyle }

### geo

1. map 注册的地图名字
2. roam
3. zoom
4. itemStyle
5. emphasis

### 图表

1. 折线图

   - smooth
   - itemStyle
   - areaStyle
   - symbol  image:// path:// 
   - symbolSize

2. 饼图

   - roseType 玫瑰图 radius area
   - radius 百分比参考容器最短边大小 [内圆半径，外圆半径]
   - itemStyle { color }
   - label { position, lineHeight, fontWeight, fontSize, formatter }

3. 散点图

   - data [[x,y,r]]
   - symbolSize: ()=>{} | number
   - label: { formatter, fontWeight, fontSize, position, distance }

4. k 线图

   - data [[开盘值，收盘值，最低，最高]]
   - itemStyle { color, color0, borderColor, borderColor0 },
   - barWidth
   - borderWidth

5. 雷达图

   - data [{}]

6. 仪表盘

   - startAngle
   - endAngle
   - max
   - min

7. 地图

   - echarts.registerMap(name, data)
   - map
   - zoom
   - roam
   - itemStyle { areaColor, borderColor }
   - emphasis { itemStyle, label }
   - coordinateSystem mapname // 和例如散点图一起使用
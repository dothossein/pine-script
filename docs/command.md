# دستورات کاربردی

### گرفتن نام نماد چارت(symbol)

```pine
syminfo.tickerid

```

---

### گرفتن تایم فریم چارت(timeframe)

```pine 
timeframe.period
```

---

### if

```pine
if condition
    then
else if condition
    then
else
    then


condition ? if ture : false

```

---

### for

```pine
for i=0 to 10
    then
```

---

### while

```pine
while true
    then
    break
    continue
```

---

### input

```pine
strategy("My strategy", overlay=true)

var string name="hossein"
age=14
float tall=140.50

var string name2=input.string("hossein","Name: ",options = ["hossein","ali","hassan"])
var int age2=input.int(14,"age: ",minval=0,maxval=100,step=1)

float my_source=input.source(open,"source") // تمامی سورس ها بصورت آپشن نمایش داده میشوند

```

در Pine Script، کلمه کلیدی `var` برای تعریف متغیرهایی استفاده می‌شود که فقط یک بار مقداردهی اولیه می‌شوند و **مقدار آن‌ها در طول اجرای اسکریپت حفظ می‌شود**.

---

### color

```pine
color textColor = color.green   
color labelColor = #FF000080
c = color.rgb(0,255,0,0)
d=color.new(color, transp) → const color

```

---

### bgcolor

```pine
bgcolor(color.blue)

bgcolor(bar_index%2==0 ? color.new(color.blue,50): na)


color bg_color=na
if bar_index%2==0
    bg_color := color.blue
else
    bg_color :=color.red

bgcolor(color=bg_color)


```

---

### barcolor

```pine
barcolor(color.red)

```

---

### function

```pine
function(type a,type b) =>
    the code
```

---

###
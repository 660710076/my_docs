---
description: การหา Index ของ Element ใน array
---

# Finding the Index of an Element

การหาค่า Index ใน Element ของ array นั้นบ่อยครั้งที่เราต้องการหาตำเเหน่ง index ของ array เพื่อนำไปใช้งานต่อโดยเราสามารถหาตำเเหน่ง index ได้โดยคำสั่งต่อไปนี้

#### 1.)  การใช้ .index()

#### การใช้ .index()  นั้นเป็นการหาค่า index ใน array  ของ element ตัวเเรกที่เจอโดยการใส่ค่า element ลงไปใน () เพื่อตรวจสอบค่าใน array เเละทำการ return ออกมา

### ตัวอย่าง Array

```
month = ["Jan","Feb","Mar","April","May","May","June"]
```

หากเราต้องการหาค่า index ใน array สามารถทำได้ดังนี้

### ตัวอย่างภาษา Ruby

```
puts month.index("May")
# ค่าที่ได้ออกมาคือ 4
```

### ตัวอย่างภาษา Python

```
print(month.index("May"))
# ค่าที่ได้ออกมาคือ 4
```

### ตัวอย่างภาษา Java

```
import java.util.Arrays;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        String[] month = {"Jan", "Feb", "Mar", "April", "May", "May", "June"};
        List<String> monthList = Arrays.asList(month);

        System.out.print(monthList.indexOf("May"));
    }
}
# ค่าที่ได้ออกมาคือ 4
```

### ตัวอย่างภาษา C

```
    int size = sizeof(month) / sizeof(month[0]);

    for (int i = 0; i < size; i++) {
        if (strcmp(month[i], "May")==0) {
            printf("%d" , i);
            break;
      }
    }
    return 0;
# ค่าที่ได้ออกมาคือ 4
```

2.) การใช้ .rindex()

การใช้ .rindex() เป็นการหาค่า index ของelement ตัวสุดท้ายที่เจอใน array โดยทำการใส่ค่าลงใน () เเละทำการ return ออกมา

### ตัวอย่างภาษา Ruby

```
putsตัวอย่างby month.rindex("May")
# ค่าที่ได้ออกมาคือ 5
```

### ตัวอย่างภาษา Python

<pre><code>last_index = -1
for i in range(len(mon<a data-footnote-ref href="#user-content-fn-1">t</a>h)-1, -1, -1):
    if month[i] == "May":
        last_index = i
        print(last_index)
        break
        
# ค่าที่ได้ออกมาคือ 5    
</code></pre>

### ตัวอย่างภาษา Java

```
for(int i=month.length-1;i>-1;i--){
    if(month[i].equals("May")){
        System.out.print(i);
        break;
    }
}

# ค่าที่ได้ออกมาคือ 5
```

### ตัวอย่างภาษา C

```
int size = sizeof(month) / sizeof(month[0]);

for(int i=size-1;i>-1;i--){
    if(strcmp(month[i],"May")==0){
        printf("%d",i);
        break;
    }
}
return 0;

# ค่าที่ได้ออกมาคือ 5
```

## Reference

Techtopia - Understanding Ruby Arrays สืบค้นเมื่อ 4/9/2568 จาก [https://www.techotopia.com/index.php/Understanding\_Ruby\_Arrays](https://www.techotopia.com/index.php/Understanding_Ruby_Arrays)\
W3schools - Python Arrays สืบค้นเมื่อ 4/9/2568 จาก [https://www.w3schools.com/python/python\_arrays.asp](https://www.w3schools.com/python/python_arrays.asp)\
W3schools - C Arrays สืบค้นเมื่อ 4/9/2568 จาก [https://www.w3schools.com/c/c\_arrays\_size.php](https://www.w3schools.com/c/c_arrays_size.php)\
W3schools - Java Arrays สืบค้นเมื่อ 4/9/2568 จาก [https://www.w3schools.com/java/java\_arrays.asp](https://www.w3schools.com/java/java_arrays.asp)

[^1]: 

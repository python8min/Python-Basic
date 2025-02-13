# آموزش توابع در پایتون  

توابع یکی از مفاهیم کلیدی در زبان برنامه‌نویسی پایتون هستند که به شما امکان می‌دهند بلوک‌های کدی سازمان‌یافته، خوانا، و قابل استفاده مجدد ایجاد کنید. این فایل آموزشی به شما کمک می‌کند تا با ساختار و کاربرد توابع در پایتون آشنا شوید.

---

## **توابع چیستند؟**  
توابع در پایتون بلوک‌هایی از کد هستند که برای انجام یک وظیفه خاص تعریف می‌شوند. این بلوک‌ها می‌توانند **ورودی** بگیرند و **خروجی** تولید کنند. استفاده از توابع باعث:  
- کاهش تکرار کد  
- افزایش خوانایی  
- تسهیل اشکال‌زدایی  

---

## **ساختار کلی یک تابع**
ساختار یک تابع در پایتون به شکل زیر است:  
```python
def function_name(parameters):
    """
    توضیحات تابع (اختیاری)
    """
    # بدنه تابع
    return result  # (اختیاری)
```

### **مثال ساده**:  
تابعی که یک پیام خوش‌آمدگویی چاپ می‌کند:  
```python
def greet():
    print("سلام! به آموزش توابع خوش آمدید.")
greet()
```

---

## **پارامترها و آرگومان‌ها (Parameters & Arguments)**  
توابع می‌توانند ورودی بگیرند. این ورودی‌ها در قالب **پارامترها** تعریف می‌شوند و هنگام فراخوانی تابع، **آرگومان‌ها** مقدار آن‌ها را مشخص می‌کنند.

### **مثال با ورودی:**  
تابعی که نام شما را به عنوان ورودی دریافت می‌کند:  
```python
def greet_with_name(name):
    print(f"سلام {name}! خوش آمدی.")
greet_with_name("علی")
```

---

## **خروجی (Return Statement)**  
تابع می‌تواند مقداری را به عنوان خروجی برگرداند. برای این کار از دستور `return` استفاده می‌کنیم.

### **مثال با خروجی:**  
```python
def add_numbers(a, b):
    return a + b
result = add_numbers(5, 7)
print(result)  # خروجی: 12
```

---

## **آرگومان‌های پیش‌فرض (Default Arguments)**  
می‌توانید برای پارامترهای تابع مقدار پیش‌فرض تعریف کنید. اگر هنگام فراخوانی مقدار مشخص نشود، مقدار پیش‌فرض استفاده خواهد شد.

### **مثال با آرگومان پیش‌فرض:**  
```python
def greet_with_default(name="دوست عزیز"):
    print(f"سلام {name}!")
greet_with_default()  # خروجی: سلام دوست عزیز!
greet_with_default("مریم")  # خروجی: سلام مریم!
```

---

## **توابع ناشناس (Lambda Functions)**  
توابع کوتاه و ساده‌ای هستند که با کلمه کلیدی `lambda` تعریف می‌شوند. این توابع معمولاً برای عملیات‌های کوچک و سریع استفاده می‌شوند.

### **مثال:**  
```python
add = lambda x, y: x + y
print(add(3, 5))  # خروجی: 8
```

---

## **تفاوت `print` و `return`**  
- `print` مقداری را در کنسول نمایش می‌دهد ولی آن را برنمی‌گرداند.  
- `return` مقدار را برمی‌گرداند تا بتوانید در سایر قسمت‌های برنامه از آن استفاده کنید.

### **مثال:**  
```python
def add_numbers(a, b):
    print(a + b)  # فقط نمایش مقدار
    return a + b  # بازگشت مقدار

x = add_numbers(3, 5)  # مقدار برگشتی ذخیره می‌شود
```

---

## **تمرین‌ها برای یادگیری بیشتر**  
1. تابعی بنویسید که اعداد داخل یک لیست را جمع کند.  
2. تابعی بسازید که یک رشته را دریافت کرده و تعداد حروف آن را برگرداند.  
3. تابعی تعریف کنید که عددی را دریافت کرده و بررسی کند آیا عدد اول است یا خیر.  

---

## **منابع بیشتر**  
برای یادگیری بیشتر می‌توانید به مستندات رسمی پایتون یا وب‌سایت‌هایی مثل [W3Schools](https://www.w3schools.com/python/) یا [Real Python](https://realpython.com/) مراجعه کنید.  

**موفق باشید!**
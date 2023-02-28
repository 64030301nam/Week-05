# การทดลองสัปดาห์ที่ 5.2 #
## แสดงรายละเอียดของ predefined type ในภาษา C#  ##


### Learning Outcome ###
1. นักศึกษารู้จัก predefined type และบอกได้ว่ามีอะไรบ้าง
2. นักศึกษาสามารถเขียนโปรแกรมเพื่อรายงานค่าเฉพาะตัวของ predefined type ได้

## แบบฝึกหัด ##

แก้ไขโค้ดตัวอย่าง ให้รายงานรายละเอียดของ predefine type ได้ครบถ้วน

Type ใดที่ไม่มี properties ที่กำหนดให้แสดงก็ให้เว้นไว้ หรือใช้การขีด (`-`)
```cs
sbyte sb = new sbyte();  // create new object
byte bt = new byte();
short sh;                 
ushort ush;
int ii = new int();
uint ui;
long lo;
ulong ul;
float fl;
double db;
bool bl;
char ch;
decimal de;

object ob = new object();
string st = new string("");
dynamic dy;


Console.WriteLine($"Declaration\tType name\tType code\tMaximum Value\tMinimum Value");
Console.WriteLine($"----------------------------------------------------------------------------");
Console.WriteLine($"sbyte sb\t{sb.GetType()}\t{sb.GetTypeCode()}\t\t{sbyte.MaxValue}\t\t{sbyte.MinValue}");
Console.WriteLine($"byte bt\t\t{sb.GetType()}\t{bt.GetTypeCode()}\t\t{byte.MaxValue}\t\t{byte.MinValue}");
Console.WriteLine($"short sh");
Console.WriteLine($"ushort ush");
Console.WriteLine($"int ii\t\t{ii.GetType()}\t{ii.GetTypeCode()}\t\t{int.MaxValue}\t{int.MinValue} ");

Console.WriteLine($"object ob\t{ob.GetType()}");
Console.WriteLine($"string st\t{st.GetType()}\t{st.GetTypeCode()} ");

Console.WriteLine("============================================================================");
```

![image](https://user-images.githubusercontent.com/115066329/221769009-2f75955b-91ef-487e-88dc-d332213e4f9c.png)

```cs
sbyte sb = new sbyte();
byte bt = new byte();
short sh = new short();
ushort ush = new ushort();
int ii = new int();
uint ui = new uint(); 
long lo = new long();  
ulong ul = new ulong(); 
float fl = new float();
double db = new double();
bool bl = new bool();
char ch = new char();
decimal de = new decimal();

object ob = new object();
string st = new string("");
dynamic dy = new System.Dynamic.ExpandoObject();


Console.WriteLine($"Declaration\tType name\tType code\tMaximum Value\t\tMinimum Value");
Console.WriteLine($"------------------------------------------------------------------------------------------------------------------");
Console.WriteLine($"sbyte sb\t{sb.GetType()}\t{sb.GetTypeCode()}\t\t{sbyte.MaxValue}\t\t\t{sbyte.MinValue}");
Console.WriteLine($"byte bt\t\t{sb.GetType()}\t{bt.GetTypeCode()}\t\t{byte.MaxValue}\t\t\t{byte.MinValue}");
Console.WriteLine($"short sh\t{sh.GetType()}\t{sh.GetTypeCode()}\t\t{short.MaxValue}\t\t\t{short.MinValue}");
Console.WriteLine($"ushort ush\t{ush.GetType()}\t{ush.GetTypeCode()}\t\t{ushort.MaxValue}\t\t\t{ushort.MinValue}");
Console.WriteLine($"int ii\t\t{ii.GetType()}\t{ii.GetTypeCode()}\t\t{int.MaxValue}\t\t{int.MinValue} ");
Console.WriteLine($"uint ui\t\t{ui.GetType()}\t{ui.GetTypeCode()}\t\t{uint.MaxValue}\t\t{uint.MinValue}");
Console.WriteLine($"long lo\t\t{lo.GetType()}\t{lo.GetTypeCode()}\t\t{long.MaxValue}\t{long.MinValue}");
Console.WriteLine($"ulong ul\t{ul.GetType()}\t{ul.GetTypeCode()}\t\t{ulong.MaxValue}\t{ulong.MinValue}");
Console.WriteLine($"float fl\t{fl.GetType()}\t{fl.GetTypeCode()}\t\t{float.MaxValue}\t\t{float.MinValue}");
Console.WriteLine($"double db\t{db.GetType()}\t{db.GetTypeCode()}\t\t{double.MaxValue}\t{double.MinValue}");
Console.WriteLine($"bool bl\t{bl.GetType()}\t{bl.GetTypeCode()}\t\t\t{bool.TrueString}\t\t\t{bool.FalseString}");
Console.WriteLine($"char ch\t{ch.GetType()}\t{ch.GetTypeCode()}\t\t\t{char.MaxValue}\t\t{char.MinValue}");
Console.WriteLine($"decimal de\t{de.GetType()}\t{de.GetTypeCode()}\t\t{decimal.MaxValue}\t{decimal.MinValue}");
Console.WriteLine();
Console.WriteLine($"object ob\t{ob.GetType()}\t-----\t\t----------\t\t----------");
Console.WriteLine($"string st\t{st.GetType()}\t{st.GetTypeCode()}\t\t----------\t\t----------");
Console.WriteLine($"dynamic dy\t{dy.GetType()}\t----------\t\t----------");

Console.WriteLine("==================================================================================================================");
```
![image](https://user-images.githubusercontent.com/115066329/221770906-14b5be1e-64a2-45a4-bf7a-0ee72afc93df.png)


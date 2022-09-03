# UC-GameDev-CW-4

# <p dir="rtl">
<strong>الشرح: </strong></p>
<p dir="rtl">
هذه دالة تكشف حركة الفأرة

</p>

```
void OnMouseDrag(){}
```

و لتحويل نقطة من مساحة الشاشة إلى مساحة اللعبة
    
```
Camera.main.ScreenToWorldPoint(mousePos);

```


باستخدام هذه الدالة ، يمكنك تحريك GameObject باستخدام الفأرة


```
 void OnMouseDrag()
{
        Vector2 mousePos = new Vector2(Input.mousePosition.x, Input.mousePosition.y);
        Vector2 playerPos = Camera.main.ScreenToWorldPoint(mousePos);
        transform.position = playerPos;
}
```


<p dir="rtl">
<strong>خطوات الواجب: </strong></p>




* باستخدام هذه الدالة ، قم ببناء أي لعبة ترغب فيها

Sample Output : 



* في هذه اللعبة, تستخدم الفأرة لحماية الرجل الموجود في منتصف الشاشة

<p align = "center">
<img alt="" src="https://user-images.githubusercontent.com/61245162/173615897-8b5e1fc6-ea41-43e0-b264-1224f2071b5e.gif">
  </p>

* مثال آخر هو المتاهة, حيث يستخدم اللاعب الماوس للتنقل عبر متاهة والوصول إلى النهاية
<p align = "center">
<img alt="" src="https://user-images.githubusercontent.com/61245162/173616596-eee1367d-2662-4747-93c8-e8fe3e114c3c.gif">
  </p>


### الخطوة الأولى: الوصول إلى بيئة التطوير وملفات الموقع

للبدء في كتابة الكود، يجب عليك الدخول إلى مدير الملفات (File Manager) الخاص بالاستضافة التي تستخدمها. من هناك، قم بالبحث عن ملف الواجهة الرئيسية والذي يُسمى غالباً index.html. قم بالنقر بزر الماوس الأيمن على الملف واختر "تعديل" (Edit) لفتح محرر الأكواد.

### Step 1: Accessing the Development Environment

To start coding, you need to access the File Manager of your web hosting service. From there, locate your main interface file, usually named index.html. Right-click on the file and select "Edit" to open the code editor.

![img alt](https://github.com/taleensami001-lgtm/How-to-Add-Voice-Control-to-a-Web-Based-Robot-Interface/blob/0d0456dbbffbcc8f7c46df9956ace65c9c20ed3c/IMG_1939.png)
### الخطوة الثانية: بناء واجهة المستخدم وتنسيقها
داخل ملف index.html، نقوم ببناء الهيكل الأساسي للواجهة. تتكون الواجهة من شبكة أزرار للاتجاهات (أمام، خلف، يمين، يسار، توقف) بالإضافة إلى زر خاص لتفعيل الميكروفون، ونص في الأسفل لعرض حالة الاتصال. باستخدام CSS، نقوم بتنسيق الأزرار وترتيبها في شبكة (Grid) لتكون واضحة وسهلة الاستخدام، مع إعطاء زر الصوت لوناً مميزاً (مثل الأخضر).

### Step 2: Building and Styling the User Interface
Inside the index.html file, we build the basic structure of the interface. The layout consists of a grid of directional buttons (forward, backward, right, left, stop), a dedicated button to activate the microphone, and a status text element at the bottom. Using CSS, we style and arrange the buttons using a Grid layout to make them clear and user-friendly, giving the voice button a distinct color (like green).


### الخطوة الثالثة: برمجة دالة إرسال الأوامر للسيرفر
الآن نأتي إلى الجانب البرمجي باستخدام JavaScript. الخطوة الأهم هي إنشاء دالة sendCommand المسؤولة عن أخذ الأمر (مثل الحرف 'f' للتقدم للأمام) وإرساله إلى ملف PHP موجود على الخادم (وهو update_command.php). نستخدم تقنية fetch لإرسال هذه البيانات في الخلفية دون الحاجة لتحديث الصفحة، مع تحديث نص الحالة في أسفل الشاشة لإخبار المستخدم بنجاح الإرسال.

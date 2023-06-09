# العمل مع الريبو عن بُعد

تحدثنا سابقا علي أن Github يقوم بتوفير بيئة عمل مرنة يمكن للمطورين  استخدامها للتحكم في إدارة مشاريعهم، ومشاركة الأعمال والتعاون مع الآخرين  في المشاريع المشتركة، وإدارة الإصدارات والتعديلات على الكود المصدري،  وإدارة الأخطاء والعيوب وتتبع الأعمال.

الكود الذي تقوم بكتابته يكون محلي (Local) لا أحد يمكنه رؤيته غيرك  ولكن أحيانا تريد مشاركته مع الاخرين وهنا يأتي دور Github الذي يجعلك تقوم بإنشاء مستودع (repository) عليه وتحميل الكود المحلي إليه، ويمكنك مشاركة المستودع (repository) مع الآخرين عن طريق إرسال رابط المستودع  (repository) لهم. وبمجرد أن يتمتع أي شخص بصلاحيات الوصول إلى المستودع،  يمكنه القيام بعمليات التحرير والتعديل والتحديثات على الكود المصدري  وإرسالها مرة أخرى للمستودع (repository).

## اتبع الخطوات التالية لرفع مشروعك علي Github.

`git init`

`git add README.md`

`git commit -m "first commit"`

`git branch -M main`

`git remote add origin https://github.com/userName/repoName.git`

`git push -u origin main`

### **git init**

هذا الأمر يبدأ مشروع Git جديد. ينشئ Git مجلداً جديداً بإسم "git."  والذي يحتوي على جميع الأدوات التي يحتاجها Git لتتبع التغيرات في المشروع.



### **git add README.md**

هذا الأمر يقوم بإضافة ملف README.md.



### **"git commit -m "first commit**

يُستخدم هذا الأمر لتأكيد التغييرات في مشروع Git. يتم تضمين الملفات  التي تم إضافتها إلى منطقة الانتظار في عملية التأكيد (commit)، ويتم وصف  التغييرات في رسالة التأكيد.



### **git branch -M main**

يقوم هذا الأمر بإعادة تسمية الفرع الافتراضي الخاص بالمستودع من "master" الى "main".



### **`git remote add origin https://github.com/userName/repoName.git`**

يُستخدم هذا الأمر لإضافة اسم الخادم البعيد (remote repository)الذي تم ربط المشروع به إلى Git. يتم استخدام "origin" كاسم الخادم البعيد (remote repository) في هذا المثال.



### **git push -u origin main**

يقوم هذا الأمر بإرسال التغييرات المؤكدة إلى الخادم البعيد (remote repository).



## Fetch & Pull

Git Fetch و Git Pull كلاهما يُستخدمان لجلب تحديثات من مستودع Git  البعيد (remote repository) إلى مستودع Git المحلي (local repository)،  ولكن هناك اختلافات بينهما.

## **Git Fetch**

يُستخدم لجلب التحديثات الجديدة من المستودع البعيد (remote repository) إلى المستودع المحلي (local repository)، لكنه لا يقوم بدمج هذه التحديثات مع النسخة المحلية، ولذالك يجب أن تقوم بتنفيذ الأمر git merge.

## **Git Pull**

يُستخدم لجلب التحديثات الجديدة من المستودع البعيد (remote repository) و دمجها مع النسخة المحلية. يقوم Git Pull بالقيام بنفس العمل الذي يقوم  به Git Fetch ، ولكن يضيف خطوة إضافية وهي تنفيذ الأمر git merge لدمج  التحديثات الجديدة مع النسخة المحلية بشكل تلقائي.

يمكن استخدام Git Fetch عندما تريد فقط الحصول على تحديثات جديدة دون  دمجها مع النسخة المحلية، بينما يمكن استخدام Git Pull عندما تريد جلب  التحديثات الجديدة ودمجها مع النسخة المحلية.





## **Fork**

يعني إنشاء نسخة من مستودع Git الحالي وتخزينه في حساب Git آخر. عادةً  ما يتم استخدام هذا الأمر عند الرغبة في إضافة تحسينات أو تعديلات لمشروع  Git موجود على الإنترنت، حيث يتم إنشاء نسخة من المستودع الأصلي وتعديلها  دون التأثير على المستودع الأصلي. يمكن لأي شخص إنشاء نسخة من المستودع  وإجراء التعديلات التي يريدها وإرسالها إلى المستودع الأصلي للمشروع من  خلال إرسال طلب دمج Pull Request.

## **Clone**

يعني إنشاء نسخة من مستودع Git الحالي وتخزينها على جهاز الكمبيوتر  الخاص بك. يتم استخدام هذا الأمر عادةً عند الرغبة في الحصول على نسخة من  مستودع Git موجود على الإنترنت على جهاز الكمبيوتر الخاص بك لتتمكن من  العمل عليها بشكل محلي. يمكن استخدام الأمر clone عندما ترغب في الحصول على إصدار محدث من المستودع بعد إجراء تغييرات من قبل فريق التطوير.

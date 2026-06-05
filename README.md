# 📊 Social Media Data Analysis & Outlier Detection

مرحباً بك في هذا المشروع! هنا نقوم بعمل **Data Cleaning** و **Exploratory Data Analysis (EDA)** على مجموعة بيانات تخص منصات التواصل الاجتماعي (Social Media Dataset)، مع التركيز بشكل خاص على اكتشاف القيم الشاذة (**Outliers Detection**).

---

## 🚀 Project Overview (نظرة عامة على المشروع)

الهدف من هذا الـ Notebook هو فهم سلوك البيانات وتنظيفها وتجهيزها للتحليل. يحتوي المشروع على:
*   **Data Exploration**: استكشاف حجم البيانات ونوعها (`shape`, `dtypes`, `describe`).
*   **Handling Missing Values**: التعامل مع القيم المفقودة في البيانات باستخدام طرق الـ Imputation.
*   **Outliers Detection**: بناء دالات (Functions) مخصصة لاكتشاف القيم الشاذة باستخدام طريقتين مختلفتين:
    1.  **Z-Score Method**.
    2.  **IQR (Interquartile Range) Method**.
*   **Data Visualization**: رسم بياني لاستكشاف توزيع البيانات والتفاعل على المنصات المختلفة.

---

## 🛠️ Tech Stack & Libraries (التقنيات المستخدمة)

تم بناء هذا المشروع باستخدام **Python** والاعتماد على المكتبات التالية:
*   `pandas`: لملء، تنظيف، وتحليل البيانات المستطيلة.
*   `numpy`: للعمليات الحسابية وحساب الـ Z-Score.
*   `matplotlib` & `seaborn`: لعمل الـ Data Visualization ورسم الـ Boxplots والـ Countplots.

---

## 🔍 Key Steps in the Notebook (الخطوات الرئيسية)

### 1. Data Loading & Inspection (تحميل ومعاينة البيانات)
قراءة ملف الـ CSV واستعراض العينات والتأكد من أنواع البيانات الأساسية مثل التاريخ (`date`) وأرقام التفاعل (`likes`, `shares`, `comments`, `views`).

### 2. Outliers Detection Functions (دوال اكتشاف القيم الشاذة)
قمت بكتابة كود مخصص (Custom Functions) لتحديد الـ Outliers:
*   دالة `detect_outliers`: تعتمد على **Z-Score** (أكثر من 3 انحرافات معيارية من المتوسط).
*   دالة `detect_outliers_iqr`: تعتمد على **IQR** لتحديد الحدود العليا والدنيا للبيانات الرقمية في أعمدة معينة وتفادي الأعمدة النصية بشكل ذكي.

### 3. Handling Missing Values (معالجة البيانات المفقودة)
وجدنا بعض القيم المفقودة في أعمدة التفاعل، وتم التعامل معها بنجاح باستخدام طريقة الـ Forward Fill (`fillna(method='ffill')`) للتأكد من عدم وجود قيم فارغة (`nulls`).

### 4. Data Visualization (التمثيل البياني)
*   استخدام الـ **Boxplot** لمعاينة التوزيع والـ Outliers بصرياً.
*   عمل **Countplot** مخصص لمقارنة المنصات المختلفة (`platform`) وربطها بنسب التفاعل والتعليقات والـ Likes.

---

## 📈 Results (النتائج)
بعد تشغيل دوال اكتشاف القيم الشاذة (IQR & Z-Score) على بيانات الـ views والـ shares والـ comments، تبيّن أن البيانات **نظيفة وخالية من الأخطاء أو القيم الشاذة المؤثرة** (Empty DataFrame للـ Outliers)، مما يجعلها جاهزة تماماً للخطوات القادمة في التحليل أو بناء النماذج.


[social.pdf](https://github.com/user-attachments/files/16042246/social.pdf)


[social.pptx](https://github.com/user-attachments/files/16042245/social.pptx)

![Screenshot 2024-06-30 004249](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/aa2882de-db91-4e65-bba1-f9648e335bf6)
![Screenshot 2024-06-30 004254](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/5d39bfb5-0463-4ccf-9cd5-a5f62187216c)
![Screenshot 2024-06-30 004210](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/2ca6975f-5976-4cc0-a783-85704ad2df51)
![Screenshot 2024-06-30 004224](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/03a90d6b-0c07-40b9-aaf2-d758ab6cec2a)
![Screenshot 2024-06-30 004233](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/7c2d787b-a6aa-490d-8019-f41cdb775a3a)
![Screenshot 2024-06-30 004240](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/cc3e73b6-ab2e-4a8b-bd03-da420e0270e9)
![Screenshot 2024-06-30 001730](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/48efc79e-494f-494d-8754-0b9a80a0cc39)
![Screenshot 2024-06-30 001916](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/8873235d-b3c7-4475-9fc4-a4ea099cc7c0)
![Screenshot 2024-06-29 234904](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/45396ede-a5e2-422c-ab70-a968dc83a5f1)
![Screenshot 2024-06-29 234926](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/8a86e2ba-3a22-4e95-84cd-4ce96454871c)
![Screenshot 2024-06-29 234938](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/7e3cf34f-4352-4429-9260-7da60e3abe5f)
![Screenshot 2024-06-29 235002](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/44d28f35-e39c-42b3-b1d8-178f35a852cc)
![Screenshot 2024-06-29 235016](https://github.com/AbdulrahmanAhmed123/social_media/assets/95978956/f75b8596-edc4-4b61-a4d2-50c8a5a63f98)

# task-3-

بداية قمت بإنشاء حساب شخصي على موقع ibm Watson  لكي أتمكن من إنشاء assistant وذلك بمعنى chatbot  . 
ثم بعد ذلك قمت بالخطوات التالية :
1-	قمت بانشاء assistant  وقمت بتسميته Roaa  . 
2-	ثم قمت بإضافة مهارة skill له اسميتها " تحدث " وباللغة العربية . 
3-	ثم قمت بانشاء intent تحت اسم " ترحيب " لإنشاء خيارات متعددة يمكن الترحيب بها مثال " اهلا " .
4-	ثم ذهبت لخانة dialog  لتخصيص المهارة بشكل اكبر وقمت باضافة node واضافة الترحيب الذي قمت بإنشاءه ومن ثم اضافة نص رد لـ assistant respond مثال : "ياهلا " او " مرحبا " . 
5-	ثم قمت بانشاء entity واسميته " امراض " كمثال على chatbot  خاص بالمستشفيات وقمت باضافة value تحت اسم " سرطان " والمرادف الاخر " كانسر " ، ثم قمت بالذهاب الى system entities  لاختيار يوم و ساعة محددة يمكن للروبوت الرد على الاستفسار من خلالها ثم قمت بالعودة وانشاء intent جديد تحت اسم " حجوزات " ، بعد ذلك قمت باضافة مثال يمكن للمستخدم سؤاله وهو " هل يوجد لديكم حجوزات ؟ " ثم قمت باضافة node الذي تحت اسم حجوزات ومن ثم قمت باستخدام slots  لتحديد وقت و يوم وهي " يوم الجمعة " و " الساعة الثالثة عصرا " واضافتها .
6-	ثم قمت بتحميل skill  الذي انشئتها و قمت بارفاقها . 
7-	ثم بعد ذلك قمت بعد ذلك بتخصيص الواجهة كإسم الروبوت و لون الواجهة الظاهرة للمستخدم . 
8-	بعد ذلك لدمجه مع الموقع قمت بنسخ الكود الظاهر لدي و وضعه في برنامج studio visual code  ليظهر لي  على المتصفح . والكود كان كلتالي : 
9-	 <script>
10-	        window.watsonAssistantChatOptions = {
11-	            integrationID: "311b07f1-df2e-4699-8608-62ab8c9d75f5", // The ID of this integration.
12-	            region: "eu-de", // The region your integration is hosted in.
13-	            serviceInstanceID: "2206e209-a93d-4ccd-8ae4-538075813676", // The ID of your service instance.
14-	            onLoad: function(instance) { instance.render(); }
15-	          };
16-	        setTimeout(function(){
17-	          const t=document.createElement('script');
18-	          t.src="https://web-chat.global.assistant.watson.appdomain.cloud/loadWatsonAssistantChat.js";
19-	          document.head.appendChild(t);
20-	        });
21-	      </script>
22-	      </div>

وبعد ذلك عند فتحه على المتصفح تظهر لي واجهة الـ chatbot . وهذا الرابط : http://127.0.0.1:5500/front1.html



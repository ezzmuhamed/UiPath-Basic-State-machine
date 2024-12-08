# UiPath-Basic-State-machine
🎯 يعني إيه State Machine في UiPath؟

🌀 الـ State Machine ببساطة نوع من الأتمتة بيعتمد على شوية حالات (States) بنتنقل بينهم بناءً على شروط أو أحداث معينة.

مكوناتها الأساسية:

1️⃣ الحالات (States):

بنخش في حالة لما يحصل تريجر معين.

بنخرج منها لما الشرط المطلوب يتحقق.

في نوعين من الحالات:

State العادية:

Entry: الحاجات اللي بتحصل أول ما تدخل الحالة.

Exit: الحاجات اللي بتحصل أول ما تخرج منها.

Transitions: دي الانتقالات بين الحالات.

Final State: الحالة الأخيرة اللي بتنهي الأتمتة، ودي ليها بس Entry.

2️⃣ الانتقالات (Transitions):

بتوصل الحالات ببعضها، وبتحصل لما شروط معينة تتحقق.

كل Transition ليه:

Trigger: الحاجة اللي بتشغل الانتقال.

Condition: الشرط اللي لازم يتحقق عشان يحصل الانتقال.

Action: الحاجات اللي بتحصل أثناء الانتقال.

مثال بسيط: لعبة تخمين رقم 🎮

📌 هنعمل لعبة تخمين رقم من 1 لـ 100:

1️⃣ أول حالة:

بتولد رقم عشوائي باستخدام Assign، وبنخزن الرقم ده في متغير اسمه RandomNumber.

2️⃣ تاني حالة:

بتطلب من المستخدم يدخل رقم باستخدام Input Dialog.

الرقم اللي المستخدم هيكتبه بيتخزن في متغير اسمه InitialGuess.

3️⃣ الانتقالات:

لو الرقم اللي كتبه المستخدم أكبر من الرقم العشوائي، تظهر رسالة: "الرقم اللي اخترته كبير".

لو الرقم اللي كتبه أصغر، تظهر رسالة: "الرقم اللي اخترته صغير".

لو الرقم صح، بننتقل للحالة النهائية.

4️⃣ الحالة النهائية:

رسالة تهنئة بتقول: "مبروك! الرقم الصح هو " + الرقم العشوائي.

💡 ليه تستخدم الـ State Machine؟

بتسهل التعامل مع حالات معقدة وتسلسلات منطقية.

مرنة وسهلة التخصيص لأي عملية.

بتنظم الشغل لما الحالات كتير ومترتبة على بعضها.

🔔 ملاحظة مهمة:

الـ State Machine في UiPath لازم يكون ليها حالة بداية واحدة بس (Initial State)، يعني البداية لازم تكون من نقطة واضحة.

لكن بالنسبة للنهاية، ممكن يكون فيه أكتر من Final State عشان تقدر تغطي كل السيناريوهات اللي ممكن تنهي بيها العملية.

🎯 وكمان مهم تعرف إن الـ ReFramework اللي في UiPath مبني على State Machine، وده معناه إنك تقدر تعمل الـ Framework الخاص بيك أو بشركتك بكل سهولة باستخدام نفس المفهوم ده.

✨ الطريقة دي بتخلي شغلك منظم أكتر ومرن حسب احتياجاتك أو احتياجات الفريق بتاعك.

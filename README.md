<div align="center">
  <h1>Codex Ignis 📜 مخطوطة النار</h1>
    <img src="cover.png" alt="Codex Ignis Logo" width="350"/>
  <p><strong>حيثُ لا تُنسى المعرفة، وتُحفظ أصداء الحكمة في لهيب الأرشيف.</strong></p>
  <p>
    <a href="https://seif4d.github.io/Codex-Ignis/"><strong>🚀 جرب الصفحة الرئيسية</strong></a>
       |   
    <a href="https://seif4d.github.io/Codex-Ignis/app.html"><strong>🔥 افتح التطبيق مباشرة</strong></a>
  </p>

  <p>
    <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" alt="Status">
    <img src="https://img.shields.io/github/license/seif4d/Codex-Ignis?style=for-the-badge" alt="License">
    <img src="https://img.shields.io/badge/Built%20with-HTML%2FCSS%2FJS-orange?style=for-the-badge" alt="Built with">
    <img src="https://img.shields.io/badge/PRs-Welcome-brightgreen?style=for-the-badge" alt="PRs Welcome">
  </p>
</div>

> **Codex Ignis** هو ليس مجرد عارض ملفات، بل هو نظام أرشفة ذكي ومتكامل لإدارة المعرفة الشخصية المستخرجة من محادثات الذكاء الاصطناعي. استدعِ، استكشف، وحلل أرشيف محادثاتك في واجهة واحدة، قوية، وساحرة تعمل بالكامل في متصفحك.

![Codex Ignis Screenshot](screenshot.png)

---

## 🐉 قوة التنين بين يديك: المميزات الرئيسية

*   ✨ **استدعاء شامل:** قم باستيراد محادثاتك بسهولة من **ChatGPT**، **DeepSeek**، وملفات **AI Studio** مباشرةً. كل ذكرياتك في مكان واحد.
*   🧠 **تنظيم ذكي:** صنّف محادثاتك، رتبها أبجديًا أو حسب الحجم والتاريخ، وابحث في العناوين والمحتوى للعثور على أي معلومة في ثوانٍ.
*   ✏️ **تحكم كامل:** عدّل عناوين المحادثات وتصنيفاتها بسهولة. أرشيفك يتشكل حسب رؤيتك، لتصنع مكتبتك المعرفية الخاصة.
*   📊 **رؤى تحليلية:** اكتشف "الكلمات الأكثر اشتعالاً" في محادثاتك واحصائيات مفيدة لفهم أعمق لأفكارك وتفاعلاتك.
*   🚀 **يعمل بالكامل في المتصفح:** لا حاجة للتثبيت أو رفع ملفاتك لأي خادم. كل شيء يحدث محلياً على جهازك.
*   🔒 **الخصوصية أولاً:** ملفاتك تبقى ملكك. لا يتم إرسال أي بيانات لأي مكان. أنت تمتلك أرشيفك بالكامل.
*   🎨 **تصميم ساحر:** واجهة مستخدم جميلة مستوحاة من "النار والظل"، مع وضع ليلي ونهاري وتجربة استخدام سلسة.

---

## 🚀 البدء والاستخدام (في أقل من دقيقة)

استخدام **Codex Ignis** بسيط للغاية:

1.  **افتح التطبيق:** اذهب مباشرة إلى [**صفحة التطبيق**](https://seif4d.github.io/Codex-Ignis/app.html) التي تعمل عبر GitHub Pages.
2.  **(اختياري) احتفظ بنسخة:** يمكنك تحميل ملف `app.html` بالضغط على `Ctrl + S` للاحتفاظ بنسخة تعمل بدون انترنت على جهازك.
3.  **استدعِ الذكريات:** من داخل التطبيق، اضغط على زر "ملف" أو "مجلد" لتحميل محادثاتك.
4.  **أطلق العنان للاستكشاف!** تصفح، ابحث، حلل، وعدّل أرشيفك.

---

## 📜 الصيغ المدعومة حالياً

التطبيق مصمم للتعرف تلقائيًا على بنية الملفات من المصادر التالية:

-   ملف `conversations.json` (الصيغة الحديثة والمباشرة) من **ChatGPT**.
-   ملف `chat_log.json` من **DeepSeek**.
-   مجلد يحتوي على ملفات JSON من **Google AI Studio**.
-   ملف `Codex_Ignis_Export.json` الذي تم تصديره من التطبيق نفسه.

---

## 🪄 أدوات المخطوطة: تحويل السجلات القديمة

هل لديك ملفات بتنسيقات قديمة من ChatGPT؟ لا تقلق، المخطوطة تقدم لك أدوات التحويل اللازمة.

<details>
<summary><strong>الطريقة 1: التحويل من <code>chat.html</code></strong></summary>
<br>

إذا كان ملف التصدير الخاص بك قديمًا ويحتوي على `chat.html`، اتبع هذه الخطوات السحرية لتحويله:

**1. افتح الملف:** افتح ملف `chat.html` في متصفح ويب (مثل Google Chrome).

**2. افتح الكونسول:** اضغط على `F12` لفتح "أدوات المطور"، ثم انتقل إلى تبويب **Console**.

**3. نفّذ الكود:** **انسخ الكود التالي بالكامل**، ثم الصقه في الـ Console واضغط `Enter`.

```javascript

function extractConversationsToJson() {
    // 1. تحديد جميع عناصر المحادثات
    const conversationElements = document.querySelectorAll('div.conversation');

    // 2. تهيئة مصفوفة لتخزين بيانات المحادثات
    const allConversationsData = [];

    // 3. المرور على كل عنصر محادثة لاستخراج بياناته
    conversationElements.forEach(convoDiv => {
        const conversationData = {
            title: null, // سيتم تحديثه إذا وجد عنوان
            messages: []
        };

        // 3.1 محاولة استخراج العنوان (العنصر h4 داخل المحادثة)
        const titleElement = convoDiv.querySelector('h4');
        if (titleElement) {
            conversationData.title = titleElement.textContent.trim();
        }

        // 3.2 تحديد جميع عناصر الرسائل داخل المحادثة الحالية
        const messageElements = convoDiv.querySelectorAll('pre.message');

        // 3.3 المرور على كل عنصر رسالة لاستخراج المؤلف والمحتوى
        messageElements.forEach(messagePre => {
            const authorElement = messagePre.querySelector('div.author');
            // نفترض أن محتوى الرسالة هو العنصر div التالي مباشرة لعنصر المؤلف
            // أو يمكن استخدام selector أكثر تحديدًا إذا تغير الهيكل
            const contentElement = authorElement ? authorElement.nextElementSibling : messagePre.querySelector('div:not(.author)'); // طريقة بديلة لإيجاد المحتوى

            if (authorElement && contentElement) {
                const messageData = {
                    author: authorElement.textContent.trim(),
                    content: contentElement.textContent.trim()
                };
                conversationData.messages.push(messageData);
            } else {
                console.warn("Could not find author or content for a message in conversation:", conversationData.title || 'Untitled', messagePre);
            }
        });

        // 3.4 إضافة بيانات المحادثة المكتملة إلى المصفوفة الرئيسية
        if (conversationData.messages.length > 0) {
             allConversationsData.push(conversationData);
        } else if (conversationData.title) {
             // يمكن إضافة محادثات فارغة إذا كان لها عنوان فقط (اختياري)
             // allConversationsData.push(conversationData);
             console.warn("Conversation found with title but no messages:", conversationData.title);
        }
    });

    // 4. التأكد من وجود بيانات لاستخراجها
    if (allConversationsData.length === 0) {
        console.log("لم يتم العثور على أي محادثات بالصنف 'conversation'.");
        alert("لم يتم العثور على أي محادثات بالصنف 'conversation'.");
        return;
    }

    // 5. تحويل مصفوفة البيانات إلى نص JSON منسق
    const jsonString = JSON.stringify(allConversationsData, null, 2); // null, 2 للتنسيق الجميل

    // 6. إنشاء وتحميل ملف JSON
    const blob = new Blob([jsonString], { type: 'application/json' });
    const url = URL.createObjectURL(blob);
    const a = document.createElement('a');
    a.href = url;
    a.download = 'conversations.json'; // اسم الملف الذي سيتم تحميله
    document.body.appendChild(a); // الإضافة ضرورية لبعض المتصفحات مثل Firefox
    a.click();
    document.body.removeChild(a); // التنظيف بعد التحميل
    URL.revokeObjectURL(url); // تحرير الذاكرة

    console.log(`تم استخراج ${allConversationsData.length} محادثة وحفظها في ملف conversations.json`);
    alert(`تم استخراج ${allConversationsData.length} محادثة بنجاح! تحقق من مجلد التنزيلات لملف conversations.json.`);
}

// --- كيفية الاستخدام ---
// 1. افتح صفحة HTML التي تحتوي على المحادثات في جوجل كروم.
// 2. اضغط F12 لفتح أدوات المطور (Developer Tools).
// 3. اذهب إلى تبويب "Console".
// 4. الصق الكود أعلاه بالكامل في الـ Console واضغط Enter.
// 5. سيقوم الكود بتشغيل الدالة extractConversationsToJson() تلقائيًا.

// تشغيل الدالة مباشرة بعد لصق الكود
extractConversationsToJson();
```

**4. النتيجة:** سيقوم الكود بإنشاء وتحميل ملف `conversations.json` صالح للاستخدام في Codex Ignis.

</details>

<details>
<summary><strong>الطريقة 2: التحويل من <code>conversations.json</code></strong></summary>
<br>

إذا كان ملف `conversations.json` الخاص بك معقدًا وغير قابل للقراءة مباشرة، استخدم هذا السكربت لتحويله:

**1. احفظ السكربت:** تأكد أن لديك Python 3 مثبت. احفظ الكود التالي في ملف باسم `converter.py`.

**2. ضع الملفات معًا:** ضع ملف `converter.py` في نفس المجلد مع ملف `conversations.json` المعقد.

**3. نفّذ الأمر:** افتح الطرفية (Terminal) في هذا المجلد وشغّل الأمر التالي:
   ```bash
   python converter.py
   ```

**4. احصل على الملف الجديد:** سيقوم السكربت بإنشاء ملف جديد باسم `conversations_formatted.json`. هذا هو الملف الذي يمكنك استخدامه في Codex Ignis.

```python
import json
from datetime import datetime

def convert_chat_format_v2(input_filename="conversations.json", output_filename="conversations_formatted.json"):
    """
    يقوم هذا الكود المحسّن بقراءة ملف JSON من تصدير ChatGPT وتحويله
    إلى تنسيق مبسط ومنظم، مع ضمان تتبع المسار الصحيح والكامل للمحادثة.
    """
    print(f"🚀 جاري البدء بالإصدار الجديد... سأقرأ الملف: {input_filename}")

    try:
        with open(input_filename, 'r', encoding='utf-8') as f:
            all_conversations_data = json.load(f)
    except FileNotFoundError:
        print(f"❌ خطأ: لم أتمكن من العثور على الملف '{input_filename}'. تأكد من أنه في نفس المجلد.")
        return
    except json.JSONDecodeError:
        print(f"❌ خطأ: الملف '{input_filename}' لا يحتوي على بيانات JSON صالحة.")
        return

    formatted_conversations = []
    print(f"🔍 وجدت {len(all_conversations_data)} محادثة. جاري المعالجة بالطريقة الذكية...")

    for conversation_data in all_conversations_data:
        title = conversation_data.get("title", "محادثة بدون عنوان")
        mapping = conversation_data.get("mapping", {})
        
        # 1. البحث عن آخر رسالة في المحادثة (نقطة النهاية)
        # الطريقة الأكثر دقة هي استخدام "current_node" الذي يحدده الملف
        leaf_node_id = conversation_data.get("current_node")

        # إذا لم نجد "current_node"، سنبحث عن الرسالة الأحدث كخطة بديلة
        if not leaf_node_id:
            latest_time = 0
            for node_id, node in mapping.items():
                if not node.get("children"):  # هذه هي "أوراق" الشجرة (نهايات الفروع)
                    message = node.get("message")
                    if message and message.get("create_time"):
                        if message["create_time"] > latest_time:
                            latest_time = message["create_time"]
                            leaf_node_id = node_id
        
        if not leaf_node_id or not mapping:
            print(f"⚠️ تم تخطي محادثة '{title}' لعدم وجود رسائل واضحة.")
            continue

        # 2. تتبع المحادثة للخلف من النهاية إلى البداية
        messages = []
        current_id = leaf_node_id
        while current_id:
            node = mapping.get(current_id)
            if not node:
                break  # نتوقف إذا لم نجد العقدة

            message_data = node.get("message")
            if message_data and message_data.get("author"):
                author_role = message_data["author"].get("role")
                content_parts = message_data.get("content", {}).get("parts")
                
                # نتجاهل رسائل "النظام" ونجمع محتوى الرسالة
                if author_role != "system" and content_parts:
                    full_content = "".join(part for part in content_parts if isinstance(part, str)).strip()
                    
                    if full_content:  # نتأكد أن المحتوى ليس فارغًا
                        messages.insert(0, {  # نستخدم insert(0, ..) لإضافة الرسالة في البداية (لأننا نرجع للخلف)
                            "author": author_role,
                            "content": full_content
                        })
            
            # ننتقل إلى الرسالة "الأب" (الرسالة السابقة)
            current_id = node.get("parent")

        # 3. إضافة المحادثة المكتملة إلى قائمتنا النهائية
        if messages:
            formatted_conversations.append({
                "title": title,
                "messages": messages
            })
            print(f"✅ تمت معالجة محادثة: '{title}' بنجاح ({len(messages)} رسالة).")

    # 4. حفظ النتيجة النهائية في ملف JSON جديد ومنسق
    print(f"🎉 اكتملت المعالجة! جاري حفظ {len(formatted_conversations)} محادثة في الملف: {output_filename}")
    with open(output_filename, 'w', encoding='utf-8') as f:
        json.dump(formatted_conversations, f, indent=2, ensure_ascii=False)

    print("🎊 كل شيء تم بنجاح! الملف الجديد جاهز للاستخدام.")


# --- كيفية الاستخدام (نفس الطريقة السابقة) ---
if __name__ == "__main__":
    # اسم ملف الإدخال الذي يشبه التعويذة
    input_file = "conversations.json"
    
    # اسم الملف الذي تريد حفظ النتيجة فيه
    output_file = "conversations_formatted.json"
    
    convert_chat_format_v2(input_file, output_file)
```

</details>

---

## 🛠️ التقنيات المستخدمة

هذا المشروع هو دليل على قوة تقنيات الويب الحديثة، وهو مبني باستخدام:

-   **HTML5**
-   **CSS3** (مع استخدام متغيرات CSS لتصميم مرن)
-   **JavaScript (Vanilla)**: لا توجد مكتبات أو أطر عمل ضخمة!
-   **Marked.js:** لتحويل Markdown إلى HTML.
-   **DOMPurify:** لضمان الأمان عند عرض محتوى HTML.

---

## 🤝 للمساهمة

أهلاً بك يا رفيق الدرب في رحلة تطوير هذه المخطوطة! المساهمات مرحب بها جداً. سواء كانت لديك فكرة لميزة جديدة، أو وجدت خطأً، أو ترغب في تحسين الكود:

1.  قم بعمل **Fork** للمستودع.
2.  أنشئ فرعاً جديداً لميزتك (`git checkout -b feature/AmazingFeature`).
3.  قم بعمل **Commit** لتغييراتك (`git commit -m 'Add some AmazingFeature'`).
4.  قم بعمل **Push** للفرع (`git push origin feature/AmazingFeature`).
5.  افتح **Pull Request**.

يمكنك أيضاً فتح **Issue** لمناقشة فكرة أو الإبلاغ عن مشكلة.

---

## ⚖️ الترخيص

هذا المشروع مرخص تحت رخصة MIT. 

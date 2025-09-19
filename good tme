<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>موقع العبر والمواعظ</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Scheherazade+New:wght@400;700&display=swap');
        body {
            font-family: 'Scheherazade New', serif;
            background-color: #f3f4f6;
            direction: rtl;
        }
    </style>
</head>
<body class="bg-gray-100 min-h-screen flex items-center justify-center">

    <div class="container mx-auto p-4 md:p-8">
        <div class="text-center mb-8">
            <h1 class="text-4xl md:text-5xl font-bold text-gray-800 mb-2">عبر ومواعظ</h1>
            <p class="text-lg text-gray-600">من أجل حياة أكثر حكمة وإيجابية</p>
        </div>

        <div id="quotes-container" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
            <!-- سيتم إضافة العبر هنا بواسطة JavaScript -->
        </div>

    </div>

    <script>
        document.addEventListener("DOMContentLoaded", () => {
            const quotes = [
                { text: "أعظم الحكمة ألا تستعجل الأمور.", author: "حكمة قديمة" },
                { text: "لا يهم كم أنت بطيء، ما دمت لا تتوقف.", author: "كونفوشيوس" },
                { text: "التفاؤل هو الإيمان الذي يؤدي إلى الإنجاز.", author: "هيلين كيلر" },
                { text: "لا يمكن حل المشاكل بنفس العقلية التي خلقتها.", author: "ألبرت أينشتاين" },
                { text: "الحياة مليئة بالحجارة، فلا تتعثر بها بل اجمعها واصنع منها سلماً تصعد به للقمة.", author: "مجهول" },
                { text: "الصبر مفتاح الفرج.", author: "قول مأثور" },
                { text: "من تواضع لله رفعه.", author: "حديث شريف" },
                { text: "كن قوياً بما يكفي لمواجهة العالم، وكن ضعيفاً بما يكفي لمواجهة نفسك.", author: "بروس لي" },
                { text: "لا تندم على ما فات، فما فات قد مات، وما هو آت قد يأتي فكن مستعداً له.", author: "مجهول" },
                { text: "الحياة أقصر من أن تهدرها في مطاردة من لا يهتمون لأمرك.", author: "مارك توين" },
                { text: "أفضل طريقة للتنبؤ بالمستقبل هي أن تصنعه.", author: "بيتر دراكر" },
                { text: "لا تدع الفشل يوقفك عن الاستمرار.", author: "مجهول" },
                { text: "العقبات هي تلك الأشياء المخيفة التي تراها عندما ترفع عينيك عن هدفك.", author: "هنري فورد" },
                { text: "التغيير هو القانون الوحيد الثابت في الحياة.", author: "حكمة قديمة" },
                { text: "الأمل هو أن تحلق في السماء، وتغني أغنية السعادة.", author: "أبو القاسم الشابي" },
                { text: "النجاح ليس النهاية، والفشل ليس قاتلاً: الشجاعة هي مواصلة السير.", author: "ونستون تشرشل" },
                { text: "الناس ينسون ما قلت، لكنهم لن ينسوا أبداً ما جعلتهم يشعرون به.", author: "مايا أنجيلو" },
                { text: "الإيمان هو أن تؤمن بما لا ترى، ومكافأته أن ترى ما تؤمن به.", author: "سانت أوغسطين" },
                { text: "الابتسامة هي أفضل علاج مجاني.", author: "حكمة" },
                { text: "العلم نور والجهل ظلام.", author: "قول مأثور" },
                { text: "الكلمة الطيبة صدقة.", author: "حديث شريف" },
                { text: "كلما ارتفعت، كلما رأيت العالم بشكل أوسع.", author: "جلال الدين الرومي" },
                { text: "إن لم تكن في القمة، فأنت لست في القاع، بل أنت في الطريق إليها.", author: "مجهول" },
                { text: "الحياة ليست مشكلة تنتظر الحل، بل حقيقة يجب أن تجربها.", author: "سيرن كيركيغارد" },
                { text: "التفكير الإيجابي لا يعني أن كل شيء سيكون على ما يرام، بل يعني أنك ستكون بخير مهما حدث.", author: "مجهول" },
                { text: "الرحلة تبدأ بخطوة واحدة.", author: "لاوتسو" },
                { text: "لا تحكم على الكتاب من غلافه.", author: "قول مأثور" },
                { text: "إذا أردت أن تعيش سعيدًا، فاربط حياتك بهدف، وليس بأشخاص أو أشياء.", author: "ألبرت أينشتاين" },
                { text: "كن أنت التغيير الذي تريد أن تراه في العالم.", author: "غاندي" },
                { text: "النجاح هو مجموع الجهود الصغيرة التي تتكرر يوماً بعد يوم.", author: "روبرت كولير" },
                { text: "ما يهم ليس كم تعيش، بل كيف تعيش.", author: "سقراط" },
                { text: "القلب الذي لا يسكنه شيء، هو قلب حر.", author: "جبران خليل جبران" },
                { text: "لا تقلل من شأن أي عمل تقوم به، فكل عمل عظيم كان بدايته عملاً صغيراً.", author: "مجهول" },
                { text: "المال ليس كل شيء، لكنه يجعلك تشعر بالأمان.", author: "حكمة" },
                { text: "التسامح هو أن ترى الآخرين كما هم، وتتقبلهم كما هم.", author: "مجهول" },
                { text: "التعليم هو أقوى سلاح يمكنك استخدامه لتغيير العالم.", author: "نيلسون مانديلا" },
                { text: "الحياة ليست عن انتظار العاصفة لكي تمر، بل عن تعلم الرقص تحت المطر.", author: "فيفيان غرين" },
                { text: "إذا كان لديك هدف، فلا تستسلم حتى تحققه.", author: "مجهول" },
                { text: "الراحة تأتي بعد التعب.", author: "قول مأثور" },
                { text: "العمل عبادة.", author: "قول مأثور" },
                { text: "لا تحاول أن تكون شخصاً آخر، كن أنت فقط.", author: "حكمة" },
                { text: "المرونة هي القوة الحقيقية.", author: "مجهول" },
                { text: "كن لطيفاً، فالكل يعاني من شيء ما لا تعرفه.", author: "أفلاطون" },
                { text: "السعادة ليست في كم تمتلك، بل في كم تعطي.", author: "ليو تولستوي" },
                { text: "الفرح الحقيقي هو في أن تخدم الآخرين.", author: "الأم تيريزا" },
                { text: "لا أحد يستطيع أن يجعلك تشعر بالدونية بدون موافقتك.", author: "إليانور روزفلت" },
                { text: "الأماني العظيمة تصنع الرجال العظماء.", author: "جورج برنارد شو" },
                { text: "النجاح هو الانتقال من فشل إلى فشل دون فقدان الحماس.", author: "ونستون تشرشل" },
                { text: "العقل السليم في الجسم السليم.", author: "مثل عربي" },
                { text: "المرأة هي نصف المجتمع، بل هي التي تلد النصف الآخر.", author: "علي بن أبي طالب" },
                { text: "إن الإنجازات العظيمة تتطلب إصراراً ومثابرة.", author: "مجهول" },
                { text: "لا تحكم على مسار حياتك من زاوية واحدة.", author: "حكمة" },
                { text: "الوقت هو أثمن ما نملك، فلا تضيعه في الندم.", author: "حكمة قديمة" },
                { text: "القلب هو بوصلة الروح.", author: "مجهول" },
                { text: "المعرفة قوة، والعلم نور.", author: "مثل" },
                { text: "أفضل صديق هو من تجده بجانبك في الشدة.", author: "حكمة" },
                { text: "لا تخف من الفشل، بل اخش ألا تحاول أبداً.", author: "مثل" },
                { text: "الشمس لا تنتظر أحداً لتشرق.", author: "مثل ياباني" },
                { text: "الصمت لغة العظماء.", author: "حكمة" },
                { text: "التغيير الحقيقي يبدأ من الداخل.", author: "مجهول" },
                { text: "كل يوم هو فرصة جديدة لتعيش أفضل.", author: "مجهول" },
                { text: "لا تستسلم، فإن النجاح ينتظر المثابرين.", author: "حكمة" },
                { text: "الحياة ليست سباقاً، بل رحلة.", author: "حكمة" },
                { text: "لا تحاول أن تكون شخصاً كاملاً، كن فقط شخصاً حقيقياً.", author: "مجهول" },
                { text: "الإنسان يمكنه أن يفعل أي شيء إذا آمن بنفسه.", author: "حكمة" },
                { text: "العطاء لا يفقر أحداً.", author: "قول مأثور" },
                { text: "السعادة قرار وليست مصيراً.", author: "مجهول" },
                { text: "لا تترك ظلال الماضي تسيطر على مستقبلك.", author: "مجهول" },
                { text: "الإيجابية هي مفتاح كل باب مغلق.", author: "مجهول" },
                { text: "التعلم لا يتوقف أبداً.", author: "حكمة" },
                { text: "إن كنت تظن أنك لا تستطيع، فأنت على حق.", author: "هنري فورد" },
                { text: "لا يوجد فشل حقيقي سوى التوقف عن المحاولة.", author: "ستيفن كوفي" }
            ];

            const quotesContainer = document.getElementById("quotes-container");

            quotes.forEach(quote => {
                const quoteCard = document.createElement("div");
                quoteCard.className = "bg-white p-6 rounded-lg shadow-md transition-transform transform hover:scale-105";
                
                const quoteText = document.createElement("p");
                quoteText.className = "text-xl text-gray-800 mb-4 leading-relaxed italic text-right";
                quoteText.textContent = `“${quote.text}”`;
                
                const authorText = document.createElement("p");
                authorText.className = "text-md text-gray-500 font-bold text-left";
                authorText.textContent = `- ${quote.author}`;
                
                quoteCard.appendChild(quoteText);
                quoteCard.appendChild(authorText);
                quotesContainer.appendChild(quoteCard);
            });
        });
    </script>

</body>
</html>

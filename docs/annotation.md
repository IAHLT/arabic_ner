# Annotation Guideline

<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Frank+Ruhl+Libre|Scheherazade+New">
<style>
.person {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #0069B4; border-radius: 1px; font-family: "Scheherazade New";
}
.location {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #28A745; border-radius: 1px; font-family: "Scheherazade New";
}
.org {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #17A2B8; border-radius: 1px; font-family: "Scheherazade New";
}
.fac {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #721817; border-radius: 1px; font-family: "Scheherazade New";
}
.event {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #2B4162; border-radius: 1px; font-family: "Scheherazade New";
}
.gpe {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: black; background-color: #FFC107; border-radius: 1px; font-family: "Scheherazade New";
}
.product {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #FA9F42; border-radius: 1px; font-family: "Scheherazade New";
}
.woa {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #0B6E4F; border-radius: 1px; font-family: "Scheherazade New";
}
.ttl {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #FA8B1B; border-radius: 1px; font-family: "Scheherazade New";
}
.language {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #437F97; border-radius: 1px; font-family: "Scheherazade New";
}
.timex {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: white; background-color: #849324; border-radius: 1px; font-family: "Scheherazade New";
}
.misc {
    padding: .2em .2em; font-size: 80%; font-weight: 700; display:inline; margin-right: 1px; color: black; background-color: #e7d2e4; border-radius: 1px; font-family: "Scheherazade New";
}
</style>


<body><p><strong>IAHLT Guidelines for Named Entity Annotation – Arabic</strong></p>
<p><strong>Introduction</strong></p>
<p>This document aims to serve as a draft proposal for entity classification، based on two schemas:</p>
<p><a href="https://github.com/OnlpLab/NEMO-Corpus/blob/main/guidelines/nemo_guidelines_v4.pdf">Hebrew Named Entity
    Annotation Guidelines</a> / Dan Bareket, Dafna Amit, Zef Segal, Reut Tsarfaty</p>
<p><a href="https://github.com/nickyringland/nested_named_entities/blob/master/entity_annotation_guildlines.pdf">Entity
    Annotation Guidelines</a> / Nicky Ringland</p>
<p>In addition, this proposal includes guidelines and explanations from Nemo Guidelines.</p>
<p>We suggest using the following categories for the IAHLT annotation of Named Entities:</p>
<p><strong>Abbreviation</strong> <strong> Meaning</strong></p>
<table>
    <tbody>
    <tr>
        <td><p>person</p></td>
        <td><p>PER</p></td>
    </tr>
    <tr>
        <td><p>organization</p></td>
        <td><p>ORG</p></td>
    </tr>
    <tr>
        <td><p>location</p></td>
        <td><p>LOC</p></td>
    </tr>
    <tr>
        <td><p>geo-political entity</p></td>
        <td><p>GPE</p></td>
    </tr>
    <tr>
        <td><p>facility</p></td>
        <td><p>FAC</p></td>
    </tr>
    <tr>
        <td><p>event</p></td>
        <td><p>EVE</p></td>
    </tr>
    <tr>
        <td><p>product</p></td>
        <td><p>DUC</p></td>
    </tr>
    <tr>
        <td><p>work of art</p></td>
        <td><p>WOA</p></td>
    </tr>
    <tr>
        <td><p>language</p></td>
        <td><p>ANG</p></td>
    </tr>
    <tr>
        <td><p>time expression</p></td>
        <td><p>TIMEX</p></td>
    </tr>
    <tr>
        <td><p>miscellaneous</p></td>
        <td><p>MISC</p></td>
    </tr>
    <tr>
        <td><p>title</p></td>
        <td><p>TTL</p></td>
    </tr>
    </tbody>
</table>
<p>The examples used in this document were taken from Arabic Wikipedia, Davar newspaper, and Kul Al-Arab newspaper.</p>
<h1><strong>Categories</strong></h1>
<p><strong>PER</strong></p>
<p>Pertains to names of individual people, whether fictional or real-life.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li> ولد <strong class="person">[إبراهيم طوقان]<sup>PER</sup></strong> في بيئة ثقافية وفكرية جيدة.</li>
    <li>ذلك دفع <strong class="person">[فدوى طوقان]<sup>PER</sup></strong> إلى المشاركة في الحياة السياسية خلال [الخمسينيات من القرن
        الماضي]<sup>TIMEX</sup>.
    </li>
    <li>من بين رؤساء السلطات الذين حضروا اللقاء كان: <strong class="person">[سمير محاميد]<sup>PER</sup></strong> من [أم
        الفحم]<sup>GPE</sup>، <strong class="person">[رائد دقة]<sup>PER</sup></strong> من [باقة الغربية]<sup>GPE</sup>، <strong class="person">[أحمد
            الأسد]<sup>PER</sup></strong class="gpe"> من [اللقية]<sup>GPE</sup>، <strong class="person">[علي سلام]<sup>PER</sup></strong> من
        [الناصرة]<sup>GPE</sup>، <strong class="person">[أيمن مرعي]<sup>PER</sup></strong class="gpe"> من [الفريديس]<sup>GPE</sup>، <strong class="person">[عمر
            أبو رقيق]<sup>PER</sup></strong class="gpe"> من [تل السبع]<sup>GPE</sup> و<strong class="person">[ابراهيم
            الهواشلة]<sup>PER</sup></strong> من [واحة الصحراء]<sup>GPE</sup>.​"
    </li>
</ol>
<p>NOTE: A <em>figure</em> in a work of art should be tagged PER, whereas the <em>name</em> of the art work should be
    tagged as WOA. For example:</p>
<ol style="direction: rtl;">
    <li><a id="_Hlk97041565"></a>ناقشت رواية [امرأة عند نقطة الصفر]<sup>WOA</sup> أشكال قهر الرجل للمرأة جسدياً ونفسياً،
        وذلك من خلال شخصية محورية وهي <strong class="person">[فردوس]<sup>PER</sup></strong>.
    </li>
    <li>شجرة شوح (شجرة العيد) مضاءة، ملابس <strong class="person">[بابا نويل]<sup>PER</sup></strong>، لحم على النار وكمامة على الأنف.
    </li>
</ol>
<p>In case of an ellipsis, where two first names are followed by a single surname – the first will be annotated by its
    own; and the second will be treated as one unit with the last name, forming a single entity:</p>
<ol style="direction: rtl;">
    <li>[جبران خليل جبران]<sup>PER</sup>، [إيليا أبو ماضى]<sup>PER</sup> ، [سعيد عقل]<sup>PER</sup> ، [نزار قباني]<sup>PER </sup>والأخوين
        <strong class="person">[إبراهيم]<sup>PER</sup> و[فدوى طوقان]<sup>PER</sup></strong>.
    </li>
</ol>
<p>Family names, when the reference is to the family as a whole and not to a person, should not be tagged:</p>
<ol style="direction: rtl;">
    <li>الحكم على قاتلي عائلة دوابشة هو عدالة جزئية للقتلى.</li>
</ol>
<p>Opposed to:</p>
<ol style="direction: rtl;">
    <li>كسب خطاب <strong class="person">[عرفات]<sup>PER</sup> </strong>التعاطف مع [القضية الفلسطينية]<sup>MISC</sup>على الساحة الدولية.
    </li>
</ol>
<p><strong>ORG</strong></p>
<p>Pertains to a group of people organized for a particular purpose, such as: educational institutions, government
    agencies, business companies, media outlets, security bodies, political parties, government offices,
    courts/tribunals, ensembles, sport teams, NPO’s, etc.</p>
<p>Generic names such as “the government” and “the ministry” should not be tagged as ORG.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>مُنحت <strong class="org">[السلطة الفلسطينية]<sup>ORG</sup></strong> بعض السلطات والمسئوليات المحدودة في المنطقة "أ" و "ب".
    </li>
    <li>أعلنت <strong class="org">[وزارة الشؤون الخارجية الإسرائيلية]<sup>ORG</sup></strong> أن الهدف الرئيسي من الاتفاقية
        الانتقالية توسيع الحكم الذاتي الفلسطيني.
    </li>
    <li>احتفلت <strong class="gpe">[جامعة [بيرزيت]<sup>GPE</sup>]<sup>ORG</sup></strong> [عام 1976]<sup>TIMEX</sup> بتخريج فوجها
        الأول.
    </li>
    <li>بدأت فكرة تأسيس [المتحف الفلسطيني]<sup>FAC</sup><strong> </strong>بمبادرة من أعضاء مجلس أمناء <strong class="org">[مؤسسة
        التعاون]<sup>ORG</sup></strong> في [عام 1997]<sup>TIMEX</sup> تخليداً للذكرى الخمسين ل[لنكبة]<sup>EVE</sup>.
    </li>
    <li>تم اعداده من قبل مؤسسة<strong class="org"> [أوكسفام]<sup>ORG</sup>،</strong> تمت كتابته وإنتاجه من خلال <strong class="org">[مؤسسة آرت
        لاب]<sup>ORG</sup></strong>، بتمويل من <strong class="org">[الاتحاد الأوروبي]<sup>ORG</sup></strong>.
    </li>
    <li>بعد الجلسة قام <strong class="ttl">[مكتب [رئيس الحكومة]<sup>TTL</sup>]<sup>ORG</sup></strong> بنشر بلاغ تفاؤلي بموجبه "تم
        الاتفاق على أن يقوم [مكتب <strong class="ttl">[رئيس الحكومة]<sup>TTL</sup>]<sup>ORG</sup></strong>، <strong class="org">[وزارة
            المالية]<sup>ORG</sup></strong> و<strong class="org">[وزارة التعاون الإقليمي]<sup>ORG</sup></strong> على الفور بوضع خطة
        خماسية لتطوير وتعزيز البلدات الدرزية والشركسية، والذي سيدرج تمويله في ميزانية الدولة.
    </li>
    <li>اليوم ينتظر المعهد مصادقة <strong class="org">[وزارة الصحة]<sup>ORG</sup></strong> للبدء في تجربة المرحلة الثالثة والأخيرة
        في التطوير.
    </li>
    <li>خلال الصيف الأخير استثمرت <strong class="org">[حكومة [الولايات المتحدة الأمريكية]<sup>GPE</sup>]<sup>ORG</sup></strong> أكثر
        من 2.48 مليار دولار في هبات الأبحاث وفي شراء مبكر لجرعات التطعيم من <strong class="org">[مودرنا]<sup>ORG</sup></strong>، و2
        مليار دولار في شراء مبكر لجرعات التطعيم من <<strong class="org">[فايزر]<sup>ORG</sup></strong>.
    </li>
    <li>وجدت دراسة أجرتها جمعية <strong class="org">'[نساء ضد العنف]<sup>ORG</sup>' </strong>عدم مساواة بين اليهود والعرب في معاملة
        الشرطة للعنف الأسري وسلوك <strong class="org">[مكتب [النائب العام]<sup>TTL</sup>]<sup>ORG</sup></strong> وحتى مدة عقوبة
        السجن للمُجرمين.
    </li>
    <li>كذلك شركة <strong class="org">[طيفع]<sup>ORG</sup></strong>، بعد أن لم تكن عمليا بملكية اسرائيلية، أعلنت في [عام 2017]<sup>TIMEX</sup>
        عن إغلاق مصانع في [إسرائيل]<sup>GPE</sup> وأقالت 1.700 عامل، في أعقاب تباطؤ في وتيرة ارتفاع أسهمها.
    </li>
    <li>بدأ هذا الإجراء في البرنامج الصباحي ل<strong class="org">[إذاعة الجيش الإسرائيلي]<sup>ORG </sup>([غالي تساهل]<sup>ORG</sup>).</strong>
    </li>
</ol>
<p>Religious institutions, higher education institutions, hospitals, hotels, museums and so on should be labeled ORG
    only when the reference is to the organization/management (otherwise, if the intention is for the building, they
    should be tagged FAC). </p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>استنكرت <strong class="org">[​نقابة الأطباء]<sup>ORG</sup></strong> في [بيروت]<sup>GPE </sup>الاعتداء على أطباء قسم الطوارئ
        في <strong class="fac">​[مستشفى المقاصد]<sup>FAC</sup></strong> ​بالضرب والتهديد والذم والقدح.
    </li>
</ol>
<p>Sports teams will be tagged ORG also when referred to by the GPE entity that they represent. Consider, for example,
    the two different uses of [طوباس] in this sentence:</p>
<ol style="direction: rtl;">
    <li>بعد الهدف الطوباسي مباشرة أتت صافرة الحكم لينتهي الشوط الأول بتقدم <strong class="org">[طوباس]<sup>ORG</sup></strong> بهدف
        نظيف.
    </li>
    <li>في ذلك الوقت، لعبت [حسين]<sup>PER</sup> في <strong class="org">[تسور شالوم]<sup>ORG</sup>.</strong> <strong>(القصد هنا لفريق
        تسور شالوم)</strong></li>
</ol>
<p> Compare with:</p>
<ol style="direction: rtl;">
    <li>قال الطالب [عدي عبد الجواد]<strong><sup>PER</sup></strong> الذي أصيب خلال فض وقفة لطلاب الثانوية العامة أمام
        [مديرية التربية والتعليم]<strong><sup>ORG</sup></strong> في <strong>[</strong><a id="_Hlk95185218"></a><strong>طوباس]<sup>GPE</sup>.</strong>
    </li>
</ol>
<p>This category also includes government agencies. Thus, in mentions of ministers heading a government office, the name
    of the office should be tagged as ORG:</p>
<ol style="direction: rtl;">
    <li>كما عمل اشتية [وزيرًا ل<strong class="org">[الأشغال العامة والإسكان]<sup>ORG</sup></strong>]<sup>TTL</sup><strong> </strong>و[وزيرًا
        ل<strong>[المجلس الاقتصادي الفلسطيني </strong><br><strong>للتنمية
            والإعمار]<sup>TTL</sup>[<sup>ORG</sup>.</strong></li>
    <li>صادق [مجلس أراضي [إسرائيل]<sup>GPE</sup>]<sup>ORG </sup>على خطة [وزير<strong> [البناء
        والإسكان]<sup>ORG</sup></strong>]<sup>TTL</sup><strong> </strong>[زئيف الكين]<sup>PER</sup> لتطوير خطة "سعر هدف"
        التي تتيح شراء شقة أولى للأزواج الشابة أو محسنات سكن بسعر أقل بنسبة 20 % من سعر السوق.
    </li>
</ol>
<p>Organizations which have a common shortened name will also be tagged as such:</p>
<ol style="direction: rtl;">
    <li>تقول [عنبال حرموني]<sup>PER</sup>، [رئيسة [نقابة العاملين الاجتماعيين]<sup>ORG</sup>]<sup>TTL</sup> في
        [الهستدروت]<sup>ORG</sup>، إن النقابة تطلب من<strong> </strong>[وزارة المالية]<sup>ORG</sup>
        <strong class="org">و[الرفاه]<sup>ORG</sup> </strong>أن تنشئ على الفور هيئة الأمن للعاملين الاجتماعيين في السلطات المحلية.
    </li>
    <li>يشير الإقتراح إلى أن استيعاب العمال الفلسطينيين يتيح تقديم استجابة سواء على ضائقة تشغيل هؤلاء العمال في <strong class="gpe">[السلطة]<sup>GPE</sup>،</strong>
        أو على صعوبات التجنيد في الشركات الإسرائيلية.
    </li>
    <li>ربما ستقوم [وزارة المالية]<sup>ORG</sup> بتقليصها من الوزارات الحكومية، <strong class="org">[التربية والتعليم]<sup>ORG</sup>
        و[الصحة]<sup>ORG</sup> و[الرعاية الاجتماعية]<sup>ORG</sup>.</strong></li>
    <li>في [عام 1988]<sup>TIMEX</sup> تبنت <strong>[منظمة التحرير]<sup>GPE</sup> </strong>رسميا خيار الدولتين في [فلسطين
        التاريخية]<sup>LOC</sup>.
    </li>
</ol>
<p>Some organizations are named after a public figure whose name may become the shortened name of the organization. The
    public figure’s name should be tagged as ORG in these instances:</p>
<ol style="direction: rtl;">
    <li>مثل جميع موظفي <strong>[بن غوريون]<sup>ORG</sup></strong> فإن أرمون ينهي المحادثة بقوله إن الأزمة ستؤثر على جميع
        الإسرائيليين.
    </li>
</ol>
<p>Sometimes organizations and geopolitical entities have the same name, such as the Palestinian Authority. It differs
    depending on the context whether the entity is referring to the organization itself or the area which it rules:</p>
<ol style="direction: rtl;">
    <li>الإغلاق الأول، وعلى وجه الخصوص إغلاق فرع البناء في [اسرائيل]<sup>GPE</sup>، أدى إلى ضربة اقتصادية صعبة في
        <strong class="gpe">[السلطة الفلسطينية]<sup>GPE</sup>.</strong></li>
</ol>
<p>Unofficial names of organizations will be tagged as ORG, such as “the Israeli Army” (instead of “the Israel Defense
    Forces”), or </p>
<ol style="direction: rtl;">
    <li><strong class="org">[الجيش الإسرائيلي]<sup>ORG</sup></strong> هو من درّب معظم المتطوعين الخاصين بي في [سوريا]<sup>GPE</sup>.
    </li>
</ol>
<p><strong>LOC</strong></p>
<p>Places that are lacking a defined political component, such as: celestial objects, continents, geographical regions,
    waterbodies, straits/isthmuses, nature reserves, mountains/hills, mountain ranges, etc.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>تم تأسيس موشاف [تسيبوري]<sup>GPE</sup> بجوار الموقع في [عام 1949]<sup>TIMEX</sup>. ويقع ضمن اختصاص المجلس
        الإقليمي <strong>[وادي [يزرعيل]<sup>GPE</sup>]<sup>LOC</sup>.</strong></li>
    <li>في [عام 1988]<strong><sup>TIMEX</sup></strong> تبنت [منظمة التحرير]<sup>GPE</sup> رسميا خيار الدولتين في
        <strong>[[فلسطين]<sup>GPE</sup> التاريخية]<sup>LOC</sup></strong>.
    </li>
    <li>نموذج واضح عن ذلك بشكل خاص، هي الفئة السكانية في القرى غير المعترف بها في <strong>[النقب]<sup>LOC</sup></strong>.
    </li>
    <li>"لدينا مدرسة للأطفال ذوي الإعاقة المتوسطة حتى الصعبة، والتي تخدم الطلاب من جميع أنحاء منطقة
        <strong class="location">[المثلث]<sup>LOC</sup></strong>".
    </li>
    <li>تقع [بيت لحم]<sup>GPE</sup> ضمن سلسلة <strong class="location">[جبال [القدس]<sup>GPE</sup>]<sup>LOC</sup>.</strong></li>
    <li>يطمع [الإسرائيليون]<sup>GPE</sup> ب<strong class="location">[هضبة الجولان]<sup>LOC</sup> </strong>لأنهم يرون أهمية كبيرة في
        السيطرة عليها لما تتمتع به من موقع استراتيجي.
    </li>
    <li>أقيم [نصب المقاتل البدوي]<sup>FAC</sup> بالقرب من <strong>[تقاطع الموفيل]<sup>LOC</sup> </strong>في الشمال
        بمبادرة من [سعدي]<sup>PER</sup> الابن.
    </li>
    <li>يمتد الجسر فوق <strong>[نهر الدانوب]<sup>LOC</sup></strong>.</li>
    <li>في قلب <strong class="location">[بحر البلطيق]<sup>LOC</sup></strong> توجد مجموعة من الجزر المعروفة باسم <strong>[أرخبيل
        ألاند]<sup>LOC</sup></strong>.
    </li>
</ol>
<p>In some cases, the name of a geographically-defined entity also contains the name of a larger geographical area in
    which it is being located. Example:</p>
<ol style="direction: rtl;">
    <li>وقعت [الهستدروت]<sup>ORG</sup> ب<strong class="location">[منطقة [الجليل]<sup>LOC</sup> الغربي]<sup>LOC</sup> </strong>وإدارة
        [مصنع زيكا للصناعات]<sup>ORG</sup> على اتفاقية عمل جماعية خاصة.
    </li>
    <li>[أعصم السلطي]<sup>PER</sup> الذي يبلغ من العمر 28 عاما من قرية [عيلوط]<sup>GPE</sup> في <strong class="location">[[الجليل]<sup>LOC</sup>
        الاسفل]<sup>LOC</sup> </strong>قُتل باطلاق نار في [يوم السبت]<sup>TIMEX</sup>.
    </li>
    <li>يُقام "سوق [الجمعة]<sup>TIMEX</sup>" في مدينة "[الكمار]<sup>GPE</sup>" في <strong>[شمال
        [هولندا]<sup>GPE</sup>]<sup>LOC</sup></strong>.
    </li>
</ol>
<p>Notice to exclude instances like “الشمال الغربي من أمستردام”, compared to “شمال غرب أمستردام”.</p>
<ol style="direction: rtl;">
    <li>أبدى [الباحث]<sup>TTL</sup> [فيليب شيرر]<sup>PER</sup> من [جامعة <strong class="location">[جنوب [غرب [تكساس]<sup>GPE</sup>]<sup>LOC</sup>]<sup>LOC</sup></strong>
        الطبية]<sup>ORG</sup>، دهشته إزاء قدرة [فيروس كورونا]<sup>MISC</sup> على إصابة الخلايا الدهنية في الجسم.
    </li>
    <li>تقع [توركو]<sup>GPE</sup> على طول <strong class="location">[ساحل [جنوب
        [فنلندا]<sup>GPE</sup>]<sup>LOC</sup>]<sup>LOC</sup></strong>.
    </li>
    <li>[نهر زمبيزي]<sup>LOC</sup> على الحدود بين [زامبيا]<sup>GPE</sup> و[زيمبابوي]<sup>GPE</sup>، في <strong>[جنوب
        [وسط [أفريقيا]<sup>LOC</sup>]<sup>LOC</sup>]<sup>LOC</sup></strong>.
    </li>
</ol>
<p><strong>GPE</strong></p>
<p>An entity who is defined by having a shared (1) ruling authority, (2) geographic location, and (3) population;
    including: nation states, counties, cities, towns, villages, regional councils, (cooperative) settlements,
    kibbutzim, neighborhoods, etc.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>سوف تغطي ولاية المجلس أرض <strong class="gpe">[الضفة الغربية]<sup>GPE</sup> و[قطاع غزة]<sup>GPE</sup></strong> باستثناء
        القضايا التي سيتم التفاوض عليها في مفاوضات الوضع الدائم.
    </li>
    <li>حدد نص الاتفاق <strong class="gpe">[المنطقة "أ"]<sup>GPE</sup></strong> بحدود محددة لبعض المدن، و<strong class="gpe">[المنطقة "ب"]<sup>GPE</sup></strong>
        بحدود محددة لمعظم القرى، وعرَّف <strong class="gpe">[المنطقة "ج"]<sup>GPE</sup> </strong>بأنها <strong class="gpe">[الضفة الغربية]<sup>GPE</sup>
        </strong>ما دون "أ" و"ب".
    </li>
    <li>بدأ انتشار الفدائيين الفلسطينيين يتركز في دول الطوق وخاصة <strong class="gpe">[الأردن]<sup>GPE</sup> و[لبنان]<sup>GPE</sup>
        و[سوريا]<sup>GPE</sup></strong>.
    </li>
    <li>هذا التأخير لم يتصدر عناوين نشرات الأخبار بسبب أن <strong class="gpe">[إسرائيل]<sup>GPE</sup></strong> نجحت في الحصول على
        التطعيمات من الشركات الأجنبية.
    </li>
</ol>
<p>Referring to a country using the name of its population will also be tagged here:</p>
<ol style="direction: rtl;">
    <li>يطمع <strong class="location">[الإسرائيليون]<sup>GPE</sup></strong> ب[هضبة الجولان]<strong class="location"><sup>LOC</sup></strong> لأنهم يرون
        أهمية كبيرة في السيطرة عليها لما تتمتع به من موقع استراتيجي.
    </li>
    <li>في سنوات الحروب بين <strong class="gpe">[الفرس]<sup>GPE</sup> و[الرومان]<sup>GPE</sup> </strong>تمكن
        [الإمبراطور]<sup>TTL</sup> " [هرقل]<sup>PER</sup> " من طرد <strong>[الفرس]<sup>GPE</sup> </strong>من
        ممتلكات<strong class="gpe"> [الدولة الرومانية]<sup>GPE</sup> </strong>[عام 629م]<sup>TIMEX</sup>.
    </li>
</ol>
<p>Sometimes GPE entities are separated using a comma, we tag them separately:</p>
<ol style="direction: rtl;">
    <li>توفي في [الولايات المتحدة الأمريكية]<strong class="gpe"><sup>GPE</sup></strong> بعد إجرائه لعملية القلب المفتوح في [مركز
        [تكساس]<sup>GPE</sup> الطبي]<sup>FAC</sup> في <strong class="gpe">[هيوستن]<sup>GPE</sup>، [تكساس]<sup>GPE</sup></strong>.
    </li>
</ol>
<p>Some geopolitical entities are named after a smaller geopolitical entity, like a municipality or a province being
    named after a city within them. Make sure to annotate the internal entity as well. For example:</p>
<ol style="direction: rtl;">
    <li>[ماربيلا]<sup>GPE</sup> تقع ضمن <strong class="gpe">[مقاطعة [مالقة]<sup>GPE</sup>]<sup>GPE</sup></strong>.</li>
</ol>
<p><strong>FAC</strong></p>
<p>(Wo)man-made constructions, roughly generalized as objects within the responsibility of civil architecture; such as:
    buildings, stadiums, towers, prisons, museums, parking lots, airports, docking ports, roads/highways, train/bus
    stations, bridges, tunnels, streets, etc. </p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>بنت السلطات البريطانية <strong class="fac">[المقاطعة]<sup>FAC</sup> </strong>وسجن<strong> </strong>على بعد 800 متر من
        <strong class="fac">[المنارة]<sup>FAC</sup></strong>، حيث لا يزال الاثنان قائمين.
    </li>
    <li>قال [بار ديفيد]<sup>PER</sup> انه تلقى نبأ تقاعد سلفه بالضبط في المؤتمر العام الماضي: "قبل عام، استقلت الطائرة
        في <strong class="fac">[مطار دوف]<sup>FAC</sup></strong>.
    </li>
    <li>قمنا بالتنظيم في <strong class="gpe">[ميناء [حيفا]<sup>GPE</sup>]<sup>FAC</sup></strong>، سنقوم بالتنظيم في <strong>[ميناء
        [أشدود]<sup>GPE</sup>]<sup>FAC</sup></strong>، أيضا لو كانت هناك تحديات.
    </li>
    <li>في [مكوروت]<sup>ORG</sup> عقدنا اتفاقية مرة في المائة سنة، وفي <strong class="gpe">[قطار
        [إسرائيل]<sup>GPE</sup>]<sup>FAC</sup></strong> سنقوم بذلك أيضا.
    </li>
    <li>قام قادة إحتجاج السلطات المحلية الدرزية والشركسية بالتظاهر [يوم الاثنين]<sup>TIMEX</sup> من هذا الأسبوع أمام
        <strong class="fac">[بيت [رئيس الحكومة]<sup>TTL</sup>]<sup>FAC</sup></strong> في [القدس]<sup>GPE</sup>.
    </li>
    <li>وكان من نصيب [غسان]<sup>PER</sup> الالتحاق <strong class="fac">ب[مدرسة الفرير]<sup>FAC</sup> </strong>ب[يافا]<sup>GPE </sup>وكان
        يحسد لأنه يدرس [اللغة الفرنسية]<sup>ANG</sup> زيادة عما يدرسه غيره.
    </li>
    <li>بحلول [عام 1905]<sup>TIMEX</sup>، مر طريق جديد يربط [نابلس]<sup>GPE</sup> ب[القدس]<sup>GPE</sup> عبر موقع ساحة
        <strong class="fac">[المنارة]<sup>FAC</sup></strong> ومبنى <strong class="fac">[سرايا]<sup>FAC</sup></strong> الذي يضم الإدارة العثمانية
        المحلية.
    </li>
    <li>يقع مجمع <strong class="fac">[مستشفى</strong> <strong class="gpe">هداسا [عين كارم]<sup>GPE</sup>]<sup>FAC </sup></strong>في الجنوب
        الغربي من [القدس]<sup>GPE</sup>.
    </li>
    <li>صادقت الحكومة على دخول 3.200 عامل فلسطيني إضافي من [يهودا والسامرة]<sup>GPE</sup> ([الضفة الغربية]<sup>GPE</sup>)
        إلى [إسرائيل]<sup>GPE</sup>، لغرض العمل في مجالي الصناعة والخدمات، وكذلك إضافة 800 تصريح عمل للعمال الفلسطينيين
        في <strong>[المنطقة الصناعية [عطروت]<sup>GPE</sup>]<sup>FAC</sup></strong>.
    </li>
    <li>ولعل بعض من أهم الأشياء التي يجب مشاهدتها في [توركو]<sup>GPE</sup> تشمل <strong>[قلعة
        [توركو]<sup>GPE</sup>]<sup>FAC</sup></strong>.
    </li>
</ol>
<p>An entity may be FAC or ORG, depending on the context if the reference is to the building rather than the
    organization/administration. Compare between the entities in the 2 sets of sentences in the 2 examples below:</p>
<ol style="direction: rtl;">
    <li>- توفي في [الولايات المتحدة الأمريكية]<sup>GPE</sup> بعد إجرائه لعملية القلب المفتوح في <strong class="fac">[مركز تكساس
        الطبي]<sup>FAC</sup></strong>.<br>- أعلن <strong class="org">[مستشفى النجاح الوطني الجامعي]<sup>ORG</sup> </strong>عن توقفه
        عن استقبال المزيد من مرضى الأورام.
    </li>
    <li>- [حكومة [إسرائيل]<sup>GPE</sup>]<sup>ORG </sup>استثمرت ايضا في تطوير لقاح من انتاج البلاد، ومولت تطوير وانتاج
        لقاح في <strong class="fac">[المعهد البيولوجي]<sup>FAC</sup></strong> في [نس تسيونا]<sup>GPE</sup>.
    </li>
</ol>
<p>- ومع ذلك، على ما يبدو فان الحكومة لم تتطرق بشكل جدي لامكانية ان يطور <strong class="org">[المعهد
    البيولوجي]<sup>ORG</sup></strong> لقاحا قبل الشركات الكبرى، ولم تمكّنهم من إجراء مراحل التجارب في المقابل، ما أعاق
    التطوير. </p>
<p>Note that neighborhoods are considered geopolitical entities, whereas streets should be treated as facilities. For
    example:</p>
<ol style="direction: rtl;">
    <li>عندما تزوج [غسان]<sup>PER</sup> كان يسكن في <strong class="fac">[شارع الحمراء]<sup>FAC</sup> </strong>ثم انتقل إلى <strong>[حي
        المزرعة]<sup>GPE</sup></strong>.
    </li>
</ol>
<p>Opposed to:</p>
<ol style="direction: rtl;">
    <li>وكان أبوه يعمل في تجارة الأقمشة في <strong class="gpe">[حي السكاكيني]<sup>GPE</sup></strong>.</li>
    <li>سمي ب<strong>[شارع الزهراء]<sup>FAC</sup></strong> نسبة لوجود <strong class="fac">[قصر الزهراء]<sup>FAC</sup></strong> فيه
        هو الاسم الذي أطلقه آل دقاق على بيتهم.
    </li>
    <li>تعتبر [البلدة القديمة]<sup>LOC </sup>في [بيت لحم]<sup>GPE </sup>أهم مناطقها على الإطلاق لوجود أهم المعالم
        الدينية المسيحية فيها، وهي تتوسط المدينة وشوارعها. من أهم تلك الشوارع: <strong>[طريق
            [الخليل]<sup>GPE</sup>]<sup>FAC</sup>، [الشارع الجديد]<sup>FAC</sup>، [شارع [بيت ساحور]<sup>GPE</sup>]<sup>FAC</sup>،
            [شارع [بولس السادس]<sup>PER</sup>]<sup>FAC</sup>، [شارع السينما]<sup>FAC</sup>، [شارع الفرير]<sup>FAC</sup>،
            [شارع [جمال عبد الناصر]<sup>PER</sup>]<sup>FAC</sup></strong>.
    </li>
    <li>توقيف 3 قاصرين من [كفر قاسم]<sup>GPE</sup> بشبهة إلقاء حجارة على سيارات في<strong class="fac"> [شارع رقم
        5]<sup>FAC</sup></strong>.
    </li>
</ol>
<p>In cases of facilities that are named after a person, a geopolitical entity, or a place it is necessary to also tag
    the nested entities. For example:</p>
<ol style="direction: rtl;">
    <li>لجنة التسميات في <strong class="gpe">[بلديّة [القدس]<sup>GPE</sup>]<sup>ORG </sup></strong>الإسرائيليّة قد أعلنت أنها تدرس
        طلبًا قُدِّم من أحد النوّاب الإسرائيليين المتطرفين في [الكنيست]<strong><sup>ORG</sup></strong> لتغيير اسم
        <strong class="person">[شارع [صلاح الدين]<sup>PER</sup>]<sup>FAC </sup></strong>إلى <strong>[شارع [دونالد ترامب]<sup>PER</sup>]<sup>FAC</sup></strong>.
    </li>
</ol>
<p>When both the Arabic and foreign names of an entity are provided, both should be tagged separately:</p>
<ol style="direction: rtl;">
    <li>مهرجان لوحات الطباشير في <strong class="fac">[متنزه السكة]<sup>FAC</sup> ([بارك همسيلاه]<sup>FAC</sup>).</strong> "الأصوات
        هامة، لكن الأهم منها هي وحدتها" (تصوير: [طال ألفي]<sup>PER</sup>)
    </li>
</ol>
<p>Streets that are named after people can be challenging, make sure to include in span the word “شارع” since it is
    crucial for understanding the specific entity’s name. A good way of determining: will the meaning stay the same if
    we remove the first noun?</p>
<ol style="direction: rtl;">
    <li>سقط عامل عن ارتفاع 8 أمتار في موقع بناء في <strong class="fac">[شارع [موشيه شريت]<sup>PER</sup>]<sup>FAC</sup> </strong>في
        [تل أبيب]<sup>GPE</sup>.
    </li>
</ol>
<p>In sentences where facilities that are named after geopolitical entities are listed, make sure to tag the listed
    items as FAC too.</p>
<ol style="direction: rtl;">
    <li>سيتم إنشاء ثمانية مجمعات لقاح للعاملين في [إسرائيل] في معابر <strong class="fac">[جلمة]<sup>FAC</sup>، [جبعة]<sup>FAC</sup>،
        [راخيل]<sup>FAC</sup></strong><br><strong class="fac"> ([300]<sup>FAC</sup>)، [ميتار]<sup>FAC</sup>، [طولكرم]<sup>FAC</sup>،
        [قلقيلية]<sup>FAC</sup>، [نعلين]<sup>FAC</sup> و[ترقوميا]<sup>FAC</sup>.</strong></li>
    <li>سيتم إنشاء أربع مجمعات إضافية، للعاملين في المستوطنات في المناطق الصناعية <strong class="fac">[اريئل]<sup>FAC</sup> ،
        [باركان]<sup>FAC</sup>، [معلية ادوميم]<sup>FAC</sup>، [إفرات]<sup>FAC</sup>.</strong></li>
</ol>
<p><strong>TTL </strong></p>
<p>Titles that should be annotated are those describing military ranks, religious roles (شيخ، رابي، إمام), academic
    titles (دكتور، مهندس، محامي), legislative and executive roles (مدير، مدير عام، مدير تنفيذي، رئيس، نائب، رئيس لجنة),
    aristocratic titles (سيد/ة), etc.; whether referring to a real-life human-being, or a made-up character. </p>
<p>For example: </p>
<ol style="direction: rtl;">
    <li>قال <strong class="ttl">[رئيس [الهستدروت]<sup>ORG</sup>]<sup>TTL</sup></strong> أنه "إذا تم تشكيل حكومة تمد يدها لعون
        العمال، فسوف يجدونا شركاء.
    </li>
    <li>قال <strong class="ttl">[رئيس [لجنة مفعّلي الرافعات البرجية]<sup>ORG</sup>]<sup>TTL</sup></strong>، [دان
        فرشبسكي]<sup>PER</sup>: "نرحب بالنية في تغيير الأنظمة القديمة منذ عام [1967]<sup>TIMEX</sup>"
    </li>
    <li>"في [رمضان]<sup>EVE</sup> هناك فرصة لفتح صفحة جديدة " يذكّر <strong class="ttl">[الشيخ]<sup>TTL</sup> </strong>[عامر]<sup>PER</sup>
        بأمل.
    </li>
    <li><strong class="ttl">[عضو [الكنيست]<sup>ORG</sup>]<sup>TTL</sup> </strong>[مفيد مرعي]<sup>PER </sup>([كحول
        لفان]<sup>ORG</sup>): "هذه شهاد فقر، يجب أن يكون في الخطة المستمرة مال ملون بميزانية الدولة"
    </li>
    <li>شارك <strong>[د.]<sup>TTL</sup></strong> [منصور عباس]<sup>PER</sup> <strong>[رئيس [القائمة العربية الموحدة]<sup>ORG</sup>]<sup>TTL</sup></strong>
        في الزيارة السنوية ل[مقام <strong>[النبي]<sup>TTL</sup> </strong>[شعيب]<sup>PER</sup>]<sup>FAC</sup>، وقدم
        التهنئة بالعيد لفضيلة <strong>[الشيخ]<sup>TTL</sup></strong> [موفق طريف]<sup>PER</sup>.
    </li>
    <li><strong>[الكابتن]<sup>TTL</sup></strong> [روبرت لويس]<sup>PER</sup> لم يكن وحشا.</li>
    <li>أجرى محققو [مكتب <strong>[مراقب الدولة]<sup>TTL</sup></strong>]<sup>ORG</sup> رقابة حول استعداد [إسرائيل]<sup>GPE</sup>
        لتفشي أوبئة واكتشفوا أن النظام الصحي بعيد من أن يكون مستعدا كما يجب.
    </li>
    <li>[مشهراوي]<sup>PER</sup> كان صديقا لوالدة [كريستينا]<sup>PER</sup>، [نادية حلو]<sup>PER</sup> رحمها الله، التي
        كانت <strong>[عضوة [الكنيست]<sup>ORG</sup>]<sup>TTL</sup> </strong>العربية المسيحية الأولى ([حزب
        العمل]<sup>ORG</sup>).
    </li>
    <li>كما كانت [حلو]<sup>PER</sup> أيضا <strong>[نائبا لرئيسة [نعمت]<sup>ORG</sup>]<sup>TTL</sup>،</strong> وكانت
        <strong>[رئيسة [وحدة النهوض بمكانة المرأة]<sup>ORG</sup>]<sup>TTL</sup> </strong>في [مركز السلطة المحلية]<sup>ORG</sup>.
    </li>
</ol>
<p>When an entity has two separate titles, each title is annoted separately:</p>
<ol style="direction: rtl;">
    <li><strong>[رئيس المعهد]<sup>TTL</sup>، [البروفيسور]<sup>TTL</sup> </strong>[شموئيل شابيرا]<sup>PER</sup>، قال في
        [الكنيست]<sup>ORG</sup> في [شهر تشرين الثاني]<sup>TIMEX</sup>/ [نوفمبر]<sup>TIMEX</sup> بأننا "كنا نستطيع أن
        نكون في الوقت الحالي بشكل عميق في داخل المرحلة الثالثة."
    </li>
    <li><strong>[رئيس [بلدية [بني براك]<sup>GPE</sup>]<sup>ORG</sup>]، [الحاخام]<sup>TTL</sup> </strong>[أفراهام
        روبنشتاين]<sup>PER</sup> استقبل رسالة دعم.
    </li>
    <li><strong>[رئيس [نادي عائلة البشارة
        للاتين]<sup>ORG</sup>]<sup>TTL </sup>[السيد]<sup>TTL</sup></strong><sup> </sup>[ريمون منصور]<sup>PER</sup>، شكر
        جميع من ساهم وعمل وتطوع في إنجاح هذه المبادرة.
    </li>
</ol>
<p>Titles should <strong>not </strong>be nested within other titles; annotations such as <sup>TTL</sup>[<sup>TTL</sup>نائبة
    [المديرة العامة]] are not allowed.</p>
<ol style="direction: rtl;">
    <li>[غال لوسكي]<sup>PER</sup> و<strong>[نائبة المديرة العامة ل[منظمة المساعدات الإسرائيلية المنقولة
        جوا]<sup>ORG</sup>]<sup>TTL</sup></strong> [مايا تسوكرمان]<sup>PER</sup> في مؤتمر في [دبي]<sup>GPE</sup>. "آنا
        آمل أن يؤسس هذا المؤتمر تحالفا في الدم بين المسلمين واليهود".
    </li>
    <li>قالت <strong>[القائمة بأعمال رئيس اللجنة]<sup>TTL</sup></strong>، <strong>[عضوة
        [الكنيست]<sup>ORG</sup>]<sup>TTL</sup></strong> [طالي بلوسكوف]<sup>PER</sup>: "يدور الحديث عن فترة مركبة.
    </li>
</ol>
<p>Adjectives (السابق، الإسرائيلي، الرائع، الشهير) adjacent to titles should be excluded:</p>
<ol style="direction: rtl;">
    <li>بنيت القلعة [سنة 1892]<sup>TIMEX</sup> من قبل <strong>[المهندس المعماري]<sup>TTL</sup> </strong><s>الهولندي</s>
        [بيترس جي. اتش. كويبرس]<sup>PER</sup>.
    </li>
    <li>أكد <strong>[رئيس الوزراء]<sup>TTL</sup></strong> <s>الإسرائيلي</s> [نفتالي بينيت]<sup>PER</sup> في تصريحات له
        اليوم [الأربعاء]<sup>TIMEX</sup>، سعيه لإعادة الجنود.
    </li>
</ol>
<p>Titles that gain their meaning only in the context of what appears after them will get a wider span, for example:</p>
<ol style="direction: rtl;">
    <li>[نزار حمودي]<sup>PER</sup> –<strong> [مدير مشاريع]<sup>TTL</sup></strong> في [بنك لئومي]<sup>ORG</sup> قال: "
        نحن سعداء باستمرار مشاريعنا ومساهماتنا المجتمعية."
    </li>
    <li>سيترأس القسم [المحاسب]<sup>TTL</sup> [زئيف تشاي]<sup>PER</sup>، الذي يشغل حاليًا منصب<strong> [رئيس المدققين
        الداخليين]<sup>TTL</sup> </strong>للبنك.
    </li>
</ol>
<p>Titles in dual and plural forms are tagged as well, as long as PER entities follow.</p>
<p><strong>EVE</strong></p>
<p>Events that are known by a common, widely-used and/or official name, such as: sporting events, festivals, peace
    treaties, <strong>holidays</strong>, national days, wars, battles, natural disasters and so on. </p>
<p>Please make sure to tag also the internal entities in cases of events whose names contain other (nested) names, such
    as the name of the month/year in which they took place; or the place where they occurred. </p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>فقد تأثرت [فدوى طوقان]<strong><sup>PER</sup></strong> باحتلال [فلسطين]<sup>GPE</sup> بعد <strong>[نكبة
        [1948]<sup>TIMEX</sup>]<sup>EVE</sup></strong> زاد تأثرها بعد احتلال مدينتها
        [نابلس]<strong><sup>GPE</sup></strong> خلال <strong>[حرب [1967]<sup>TIMEX</sup>]<sup>EVE</sup>.</strong></li>
    <li><strong>[ثورة [فلسطين]<sup>TIMEX</sup>[1936] <sup>GPE</sup>]<sup>EVE</sup></strong>، عرفت فيما بعد بأنها
        <strong>[الثورة الكبرى]<sup>EVE</sup></strong>، هي انتفاضة وطنية قام بها العرب الفلسطينيون في
        [[فلسطين]<sup>GPE </sup>الانتدابية]<sup>GPE</sup> ضد [الإدارة البريطانية]<sup>ORG</sup><strong>.</strong></li>
    <li>واستُدعي إلى [الجيش المصري]<sup>ORG</sup> في أثناء <strong>[العدوان الثلاثي على
        [مصر]<sup>GPE</sup>]<sup>EVE</sup>.</strong></li>
    <li>في <strong>[مؤتمر [إيلات]<sup>GPE</sup> للعمل]<sup>EVE</sup></strong>، قال [رئيس [الهستدروت]<sup>ORG</sup>]<sup>TTL</sup>
        أنه "إذا تم تشكيل حكومة تمد يدها لعون العمال، فسوف يجدونا شركاء. إذا تشكلت حكومة تسعى إلى إلحاق الضرر بالعمال –
        يجدونا في المقدمة.
    </li>
    <li>أنا أفعل ذلك لأنه برأيي هذه عبرة أهم من الإبادة الجماعية (<strong>[الهولوكوست]<sup>EVE</sup></strong>).</li>
    <li><strong>[هوريكان كاترينا]<sup>EVE</sup></strong> أدى في نفس السنة إلى فيضانات في [نيو اورليانز]<sup>GPE</sup>.
    </li>
    <li>في <strong>[الكورونا]<sup>EVE</sup></strong><sup> </sup>هؤلاء الشباب لم يكونوا في ال[زوم]<sup>DUC </sup>بسبب
        النقص في البنى التحتية.
    </li>
</ol>
<p>Holidays and anniversaries should be tagged as EVE as well:</p>
<ol style="direction: rtl;">
    <li>البنك مستمرّ في هذا التقليد، وفي إطار احتفالات <strong>[شهر المرأة]<sup>EVE</sup></strong> و<strong>[يوم
        الأم]<sup>EVE</sup></strong> الذي نحتفل به في [آذار]<sup>TIMEX</sup>.
    </li>
    <li>للمرة الأولى منذ تأسيسها، منعت المملكة، بأغلبية ساحقة، المسلمين من انحاء العالم الوصول الى [مكة]<sup>GPE</sup>
        في <strong>[عيد الأضحى]<sup>EVE</sup></strong>.
    </li>
    <li>تحت وقع هذه الأحداث استعد المسلمون لبداية <strong>[شهر رمضان]<sup>EVE</sup></strong>.</li>
    <li><strong>[يوم [القدس]<sup>GPE</sup>]<sup>EVE </sup></strong>تحوّل إلى رمز ل[لقدس]<sup>GPE</sup> العليا.</li>
</ol>
<p>Some entities may refer to time periods but should be tagged as EVE nevertheless:</p>
<ol style="direction: rtl;">
    <li>اشتهرت هذه المدينة الجامعية الشهيرة منذ <strong>[العصور الوسطى]<sup>EVE</sup></strong>.</li>
    <li>هو قصر من <strong>[عصر النهضة]<sup>EVE</sup></strong> على الطراز الإيطالي مع واجهة خارجية رائعة.</li>
</ol>
<p>Events may be nested:</p>
<ol style="direction: rtl;">
    <li>سيقام حدث فريد في<strong> [ذكرى يوم [المحرقة]<sup>EVE</sup>]<sup>EVE</sup></strong> في القطاع العربي من خلال
        [zoom]<sup>DUC</sup>.
    </li>
</ol>
<p><strong>DUC</strong></p>
<p>Any product that has a brand name, such as: electronic devices, vehicles, weapons, food products, medicines, etc.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>يشرف على تطوير تقنيات <strong>[USB]<sup>DUC</sup></strong> [منظمة منتدى منفذي ال<strong>[يو إس بي]<sup>DUC</sup>]</strong><sup>ORG</sup><strong>.</strong>
    </li>
    <li><strong>[آي بي إم دي بي 2]<sup>DUC</sup></strong>هي عائلة من قواعد البيانات تطورها شركة [آي بي إم]<sup>ORG</sup>،
        و كان الإصدار الأول لها في عام [1983]<strong><sup>TIMEX</sup>.</strong></li>
    <li>وافقت [إدارة الغذاء والدواء الأمريكية]<sup>ORG</sup> على دواء <strong>[ديسكوفي]<sup>DUC</sup></strong>[<strong>Descovy])<sup>
        DUC</sup></strong>) لاستعماله في الوقاية قبل التعرض، مع <strong>[تروفادا]<sup>DUC</sup></strong>، وذلك يمنح نفس
        القدر من الحماية.
    </li>
    <li>ووفقا لأقواله، "وصلت الفكرة من أحد الطلاب الجامعيين، الذي بدأ يعلّم 4 – 5 أطفال في غرفة صغيرة، بدون <strong>[زوم]<sup>DUC</sup></strong>
        وبدون انترنت. لأنه ليس لدينا بنية تحتية للانترنت."
    </li>
    <li>بعد مناقصة <strong class="product">[الجيل الخامس]<sup>DUC</sup></strong>، تدرس شركات الاتصالات خطوات إضافية.</li>
    <li>تتم إدارة الخدمات المصرفية اليوم من خلال الهاتف الذكي (<strong class="product">[الآيفون]<sup>DUC</sup></strong>).</li>
</ol>
<p>Social media networks are considered products:</p>
<ol style="direction: rtl;">
    <li>وبهدف تحقيق خطتهم، انشأوا مجموعة <strong class="product">[واتس اب]<sup>DUC</sup> </strong>نسقوا فيها تفاصيل خطة المساس.</li>
    <li>[نتنياهو]<sup>PER</sup> قرر الكتابة عن ذلك على منصة <strong class="product">[تويتر]<sup>DUC</sup>.</strong></li>
    <li>كتب [هورفيتس]<sup>PER</sup> في حسابه على <strong class="product">[تويتر]<sup>DUC</sup></strong>: "وعدت وأوفيت".</li>
</ol>
<p>Except for when the entity’s name is referring to the administration of said product:</p>
<ol style="direction: rtl;">
    <li>أعلن <strong class="org">[تويتر]<sup>ORG</sup> </strong>عن نيته حظر حساب [الرئيس الأمريكي]<sup>TTL</sup> [دونالد ترامب]<sup>PER</sup>.
    </li>
</ol>
<p><strong>WOA</strong></p>
<p>Artworks, such as: book titles, songs/poems, drawings/paintings, sculptures, movies, TV shows, scientific
    works/papers, theories, etc.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>ومن آثارها النثرية أيضاً: <strong class="woa">[أخي [إبراهيم]<sup>PER</sup>]<sup>WOA</sup></strong>، <strong>[رحلة جبلية رحلة
        صعبة]<sup>WOA</sup></strong> ، <strong class="woa">[الرحلة الأصعب]<sup>WOA</sup></strong>.
    </li>
    <li>ولعل نشيد "<strong class="woa">[موطني]<sup>WOA</sup></strong>"، الذي نسمعه صباح كل يوم في ساحات المدارس ومعاهد التعليم خير
        دليل على بقاء روحه وأدبه في الذاكرة.
    </li>
    <li>يعتقد البعض أن هناك تشابهاً بين مسلسل <strong>[التغريبة الفلسطينية]<sup>WOA</sup> و[الدرب الطويل]<sup>WOA</sup></strong>
        الذي صور في [الأردن]<strong class="gpe"><sup>GPE</sup></strong> وعُرِضَ عام [2000م]<strong><sup>TIMEX</sup></strong>.
    </li>
    <li>ناقشت رواية <strong class="woa">[امرأة عند نقطة الصفر]<sup>WOA</sup> </strong>أشكال قهر الرجل للمرأة جسدياً ونفسياً.</li>
</ol>
<p>Notice that when it is a specific issue/publication of a newspaper that is being referred to, it should be tagged as
    WOA (unlike editorial boards, or press teams, which should be tagged ORG). Same for news websites.</p>
<ol style="direction: rtl;">
    <li>وفقا لصحيفة <strong class="woa">[الصنارة]<sup>WOA</sup></strong>، خلال اللقاء عرض [نتنياهو]<sup>PER</sup> خطة المدراء
        العامين لمكافحة العنف والجريمة في المجتمع العربي.
    </li>
    <li>نشرت مصادر من [حماس]<sup>ORG</sup> هجوما اعلاميا على مساعي [مصر]<sup>GPE</sup> ووعود [السيسي]<sup>PER</sup> عبر
        جريدة <strong class="woa">[الأخبار]<sup>WOA</sup></strong> اللبنانية.
    </li>
    <li>جنبا إلى جنب مع جميع مشتركي تطبيقات صحيفة <strong class="woa">"[كلكليست]<sup>WOA</sup>"</strong>، تلقى موظفو "[سلكوم]<sup>ORG</sup>"
        إبلاغًا مساء [الاثنين]<sup>TIMEX</sup>، يشير إلى أنه من المحتمل أن يفقدوا وظائفهم في الأيام المقبلة.
    </li>
    <li>كما ارتبطت المشاركة في الأنشطة غير الدراسية بصحة عقلية أفضل حسب موقع <strong class="woa">[ساينس
        دايلي]<sup>WOA</sup></strong>.
    </li>
</ol>
<p>As opposed to:</p>
<ol style="direction: rtl;">
    <li>أفادت [وزارة التربية والتعليم]<sup>ORG</sup> في تعقيب لها على توجه "<strong class="org">[دفار]<sup>ORG</sup></strong>":
        "تنظر الوزارة بخطورة كبيرة إلى ظاهرة العنف تجاه الطلاب".
    </li>
</ol>
<p>The name of an artwork may also include internal entities.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>ويظهر أثر موت أخوها <strong class="person">[إبراهيم]<sup>PER</sup></strong> جلياً عندما نراها تهدي أغلب دواوينها إلى "روح أخي
        <strong class="person">[إبراهيم]<sup>PER</sup></strong>" ويظهر أيضا من خلال كتابها "<strong class="woa">[أخي [إبراهيم]<sup>PER</sup>]<sup>WOA</sup></strong>"
        والذي صدر سنة [1946]<a id="_Hlk97038832"></a><sup>TIMEX</sup>.
    </li>
    <li>"<strong class="woa">[عائد إلى [حيفا]<sup>GPE</sup>]<sup>WOA</sup></strong>" وصف فيها رحلة مواطني [حيفا]<sup>GPE</sup> في
        انتقالهم إلى [عكا]<sup>GPE</sup>.
    </li>
</ol>
<p>Note: Radio stations should be tagged as ORG, while radio programs should be tagged as WOA. For example:</p>
<ol style="direction: rtl;">
    <li>بحسب ما ورد في إذاعة "<strong class="org">[كادينا سير]<sup>ORG</sup></strong>" الاسبانية فإن هناك احتمالية غير ضئيلة ترجح
        رحيل [ميسي]<sup>PER</sup> عن الفريق.
    </li>
</ol>
<h1><strong>ANG</strong></h1>
<p>Pertains to language names.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>فلقد تمكن في أثناء رحلته الدراسية وطلب العلم من إتقان عدة لغات أجنبية،
        ك<strong class="language">[الإنجليزية]<sup>ANG</sup></strong> علاوة على لغات اخرى مثل <strong>[التركية]<sup>ANG</sup>
            و[الألمانية]<sup>ANG</sup> و[الإسبانية]<sup>ANG</sup>.</strong></li>
    <li>ستوزع منظمة "[حاخامات من أجل حقوق الانسان]<sup>ORG</sup>" كتيبات "[الحقوق]<sup>WOA</sup>" ب<strong class="language">[اللغة
        العبرية]<sup>ANG</sup></strong>، <strong class="language">[اللغة العربية]<sup>ANG</sup></strong> و<strong>[اللغة
        الروسية]<sup>ANG</sup>.</strong></li>
    <li>من المحتمل أن تسمع أشخاصًا يتحدثون <strong class="language">[اللغة السويدية]<sup>ANG</sup></strong> أكثر من
        <strong class="language">[الفنلندية]<sup>ANG</sup> </strong>ما بين تلك الجزر.
    </li>
</ol>
<p><strong>TIMEX</strong></p>
<p>Pertains to specific dates that have a name or a numeral representation, such as: the days of the week, months of the
    year, a certain day in a month (13 أغسطس), and seasons. </p>
<p>It is important to note that TIMEX expression tags do not get nested but rather include the full maximal span, such
    that words like شهر “the month of …” and سنة/عام “year” must be included in the tag as well.</p>
<p>Hours need not be tagged.</p>
<p>For example:</p>
<ol style="direction: rtl;">
    <li>يرجح أنه ولد <strong>[عام 1937]</strong><a id="_Hlk97039043"></a><strong><sup>TIMEX</sup></strong> في قرية
        [الشجرة]<sup>GPE</sup> الواقعة بين [طبريا]<sup>GPE</sup> و[الناصرة]<sup>GPE</sup>.
    </li>
    <li>نُشرت في [مجلة " الحرية "]<sup>ORG</sup> العدد 88 في <strong>[25 سبتمبر 1961م]<sup>TIMEX</sup></strong>.</li>
    <li>ظهر رسم [حنظلة]<strong><sup>PER</sup></strong> في [الكويت]<strong><sup>GPE</sup></strong> <strong>[عام
        1969م]<sup>TIMEX</sup></strong> في [جريدة السياسة الكويتية]<strong><sup>ORG</sup></strong>.
    </li>
    <li>وقد وري جثمانه الثرى في <strong>[13 أغسطس]</strong><a id="_Hlk97039918"></a><strong><sup>TIMEX</sup></strong> في
        مدينة [رام الله]<strong><sup>GPE</sup>.</strong></li>
    <li>تدّعي الشركة أنه خلال <strong>[شهر فبراير]<sup>TIMEX</sup></strong> أبلغتها شركة [هوت]<sup>ORG</sup> أنها قد
        تلقت تعليمات من [وزارة الاتصالات]<sup>ORG</sup> بقطع الخط.
    </li>
    <li>التقى [رئيس الحكومة]<sup>TTL</sup>، [بنيامين نتنياهو]<sup>PER</sup>، هذا المساء <strong>([الأحد]<sup>TIMEX</sup>)</strong>
        مع حوالي عشرين رئيسا لسلطات عربية.
    </li>
    <li>وفي <strong>[الخمسينيات]<sup>TIMEX</sup></strong> بدأ يستخدم اسم ياسر عرفات.</li>
    <li>وفي <strong>[5 يونيو 1967]<sup>TIMEX</sup></strong>، كانت بداية [حرب الأيام الستة]<sup>EVE</sup>.</li>
    <li>صادقت الحكومة في <strong>[يوم الأحد]<sup>TIMEX</sup>، ال[07/11]<sup>TIMEX</sup> </strong>على دخول 3200 عامل
        فلسطيني إضافي من [يهودا والسامرة]<sup>GPE</sup> ([الضفة الغربية]<sup>GPE</sup>) إلى [إسرائيل]<sup>GPE</sup>.
    </li>
    <li>الحدث التأسيسي الذي قاد إلى إنشاء المنتدى هو "[مسيرة الامهات]<sup>EVE</sup>" في <strong>[الصيف]<sup>TIMEX</sup>
    </strong>الماضي.
    </li>
</ol>
<p>Notice that when a sentence has a dual or a plural nominal modifier like “شهري”, it will not be tagged with the first
    expression as they are not compatible grammatically, like below:</p>
<ol style="direction: rtl;">
    <li>الآلية المقترحة ذات أثر رجعي حتى شهري <strong>[آذار]<sup>TIMEX</sup> و[نيسان]<sup>TIMEX</sup></strong>، وفي غياب
        وعد مستقبلي – لا تشجع العودة إلى العمل.
    </li>
    <li>ويضم المجمع منازل أودنس النموذجية من القرنين <strong>[السادس عشر]<sup>TIMEX</sup></strong> و<strong>[السابع عشر]<sup>TIMEX</sup></strong>.
    </li>
</ol>
<p>Time expressions can also be nested inside events:</p>
<ol style="direction: rtl;">
    <li>لكنه عاد وقبِل بقرار مجلس الأمن الدولي في أعقاب هزيمة [يونيو 1967]<sup>TIMEX</sup><strong>.</strong></li>
    <li><a id="_Hlk97040918"></a>ومن تلك المفاوضات <strong>[مؤتمر
        [مدريد]<sup>TIMEX</sup>[1991]<sup>GPE</sup>]<sup>EVE</sup></strong>، و[اتفاقية
        أوسلو]<sup>MISC</sup><strong>.</strong></li>
</ol>
<p>In cases where time expressions include both Arabic and foreign names of months, we tag each expression
    separately:</p>
<ol style="direction: rtl;">
    <li>قال في [الكنيست]<sup>ORG</sup> في <strong>[شهر تشرين الثاني]<sup>TIMEX</sup></strong>/ <strong>[نوفمبر]<sup>TIMEX</sup>
    </strong>بأننا "كنا نستطيع أن نكون في الوقت الحالي بشكل عميق في داخل المرحلة الثالثة."
    </li>
</ol>
<p>In cases where time expressions include a day and a date, we tag each separately:</p>
<ol style="direction: rtl;">
    <li><strong class="timex">[يوم الجمعة]<sup>TIMEX</sup> ([24.4]<sup>TIMEX</sup>)</strong class="org">، اتخذت [وزارة المالية]<sup>ORG</sup> خطوة
        مهمة وقدمت خطة تعويضات للمصالح التجارية المتضررة من [أزمة [كورونا]<sup>MISC</sup>]<sup>EVE</sup>، لكنها لم تخلق
        حافزًا لإعادتهم إلى العمل.
    </li>
</ol>
<p>When time expressions are put in construct states, we tag each noun separately:</p>
<ol style="direction: rtl;">
    <li>تم إيقاف هذا المشروع المذهل في <strong class="timex">[صيف]<sup>TIMEX</sup> [عام 2018]<sup>TIMEX</sup></strong>، بعد تعرفت
        [بوبال]<sup>PER</sup> على حالات المضايقة والاعتداء الجنسي التي ارتكبها أعضاء [الإتحاد الأفغاني]<sup>ORG</sup>.
    </li>
</ol>
<p>When the time expression is a range, make sure to tag the first date separately:</p>
<ol style="direction: rtl;">
    <li>أحداث العنف في الأسبوع<strong class="timex"> [12]<sup>TIMEX</sup>[18/12]-<sup>TIMEX</sup></strong>.</li>
</ol>
<p><strong>MISC</strong></p>
<p>Any type of entity that cannot be classified into any of the existing categories.</p>
<p>For example:</p>
<p>Diseases: not to be mistaken with <strong>symptoms </strong>of diseases which are not to be tagged.</p>
<ol style="direction: rtl;">
    <li>مرض [ياسر عرفات]<sup>PER</sup> بعد سنتين من حصار ل[لجيش الإسرائيلي]<sup>ORG</sup> له داخل مقره في [رام
        الله]<sup>GPE</sup>، ودخل في <strong>[غيبوبة]<sup>MISC</sup>.</strong></li>
    <li>لا يعرف سبب الوفاة على التحديد، وقد قال الأطباء أن سبب الوفاة هو <strong class="misc">[تليف الكبد]<sup>MISC</sup>.</strong>
    </li>
    <li>وقد توفيت والدته [زهوة أبو السعود]<sup>PER</sup> عندما كان في الرابعة من عمره بسبب <strong>[قصور
        كلوي]<sup>MISC</sup>.</strong></li>
    <li>لا شك أن نجاح [فايزر]<sup>ORG</sup> و[مودرنا]<sup>ORG</sup> في تطوير وفي انتاج لقاحات ناجعة وآمنة ضد <strong>[فيروس
        الكورونا]<sup>MISC</sup> </strong>هو انجاز مثير للإعجاب ويثير الالهام.
    </li>
</ol>
<p>Initiatives:</p>
<ol style="direction: rtl;">
    <li>بالنسبة لنا هذا يوم لكل المقدسيين الذين يعيشون هنا"، تقول لـ "[دفار]<sup>ORG</sup>" [طال ألفي]<sup>PER</sup>، من
        منظمات مبادرة <strong class="misc">"[يوم مقدسي – يوم الآخر]<sup>MISC</sup>"</strong>.
    </li>
</ol>
<p>Awards:</p>
<ol style="direction: rtl;">
  <li> وفي <strong class="timex"> [عام 1994]<sup>TIMEX</sup></strong> مُنحت <strong class="misc">[جائزة نوبل للسلام]<sup>MISC</sup> </strong>ل[ياسر
        عرفات]<strong><sup>PER</sup></strong>.
    </li>
    <li>هو الجسر الوحيد في [أوروبا]<sup>LOC</sup> الذي يتم ترشيحه ل<strong class="misc">[جائزة أوبال]<sup>MISC</sup></strong>.</li>
</ol>
<p>Game names:</p>
<p>Names of rules/laws/projects/political agreements/political entities:</p>
<ol style="direction: rtl;">
    <li>"نحن جزء من أقلية وطنية يتم التمييز ضدها في تشريعات مثل <strong class="misc">[قانون القومية]<sup>MISC</sup> و[قانون
        الجنسية]<sup>MISC</sup></strong>، النساء تعاني من ذلك".
    </li>
    <li>ومن تلك المفاوضات [مؤتمر [مدريد]<sup>GPE</sup>[1991]<sup>TIMEX</sup>]<sup>EVE</sup>، و<strong class="misc">[اتفاقية
        أوسلو]<sup>MISC</sup>.</strong></li>
    <li>كسب خطاب [عرفات]<strong><sup>PER</sup></strong> التعاطف مع <strong class="misc">[القضية الفلسطينية]<sup>MISC</sup></strong>على
        الساحة الدولية.
    </li>
    <li>"أنا أريد أن أتعاون مع منظمات في العالم الإسلامي، بعيدا عن ساحة <strong class="misc">[الصراع الإسرائيلي –
        الفلسطيني]<sup>MISC</sup></strong>". تقول [لوسكي]<sup>PER</sup>.
    </li>
    <li>قائد النضال في<strong class="misc"> [قانون المواطنة]<sup>MISC</sup></strong><sup> </sup>أعرب عن رضاه من إلغائه في
        [الكنيست]<sup>ORG</sup>.
    </li>
    <li>بدلا من <strong class="misc">[الخط الأخضر]<sup>MISC </sup></strong>نحن نجلب الشارة الخضراء.</li>
</ol>
<p>If both the Arabic and the foreign names are provided, both should be tagged separately:</p>
<ol style="direction: rtl;">
    <li>وبسبب رفض الدولة الاعتراف بهذه القرى، فان سكانها لا يتبعون لسلطة بلدية اي كانت، وبالتالي فانهم لا يدفعون
        <strong class="misc">[ضريبة الأملاك]<sup>MISC</sup> ([الارنونا]<sup>MISC</sup>)</strong>.
    </li>
</ol>
<p>Scientific names of animal/plant species:</p>
<ol style="direction: rtl;">
    <li>الأطعمة الغنية ب<strong class="misc">[حمض الأكساليك]<sup>MISC</sup></strong>، كالبقدونس، والفول السوداني.</li>
    <li>الأطعمة الغنية ب<strong class="misc">[حمض الفيتيك]<sup>MISC</sup></strong>، كالأرز البني.</li>
    <li>يعتبر الحمص والحليب مصدرًا لل<strong class="misc">[تربتوفان]<sup>MISC</sup>.</strong></li>
    <li>نبهوا إلى اهمية تناول الموز الذي يحتوي على ال<strong class="misc">[بوتاسيوم]<sup>MISC</sup></strong>
        وال<strong class="misc">[مغنيزيوم]<sup>MISC</sup></strong> وهما ضروريان لمحاربة أعراض [الاكتئاب]<sup>MISC</sup>.
    </li>
    <li>في [عام 2007]<sup>TIMEX</sup> لم تتردد شركة [فايزر]<sup>ORG</sup> في إغلاق مختبر فيه 3000 عامل في [ميشيغان]<sup>GPE</sup>،
        في أعقاب فشل في تجربة دواء ضد ال<strong class="misc">[كولسترول]<sup>MISC</sup></strong> الذي قامت بتطويره.
    </li>
</ol>
<p>Zodiac signs:</p>
<ol style="direction: rtl;">
    <li>הקנטאורים היו קשתים מעולים، ולכן דמותם מסמלת את מזל <strong class="misc">[קשת]<sup>MISC</sup></strong> בגלגל המזלות.</li>
</ol>
<p>Art movements and genres:</p>
<p>Ethnic groups:</p>
<ol style="direction: rtl;">
    <li>شعب <strong class="misc">[التاميل]<sup>MISC</sup></strong> هم أقلية عرقية في [سري لانكا]<sup>GPE</sup>، التي تعيش في أكثر
        منطقة تضررت من [التسونامي]<sup>MISC</sup>.
    </li>
</ol>
</body>

<!-- Assalomu alaykum. Bu file'limizda Vue_JS dan tushishi mumkin bo'lgan ayrim savollar va javoblar toplami mavjud.  -->

<!-- 1-savol: '<template></template>' tagiga v-for loop ishlatilganda key attribute'ni shu template tagining o'ziga bersa bo'ladimi? agar yo'q bo'lsa nima uchun? -->
<!-- Javob:  yo'q berib bo'lmaydi, chunki bu tag DOM'da haqiqiy element sifatida inobatga olinmaydi key attribute esa haqiqiy html elementga berilishi kerak, template ichida haqiqiy element ishlatilsa shunga beriladi -->
<!-- Misol: 
    <template v-for="(element, index) in topFilterData">
        <span
            v-if="element?.type === 'number'"
            :key="index"
            class="flex flex-col items-start"
        >
            <span class="text-[13px]">{{ element?.name }}</span>
            <generic-input
                :value="`${element?.defVal}`"
                type="number"
                width="250"
            />
        </span>
    </template> -->

<!-- ================================================================= -->

<!-- 2-savol: v-if va (v-show, v-hide). Bularning optimal ishlatilish case'larini aytib bering? -->
<!-- Javob: asosan elementni DOM dan butkul o'chirib yuborish kerak bo'lsa v-if dan foydalangan ma'qul,
 lekin element DOM dan o'chishi kerak emas shunchaki ko'rinish va ko'rinmasligini ta'minlash uchun v-show va v-hide dan foydalansa bo'ladi.
 v-show, v-hide ishlash tezligi v-if dan ko'ra tezroq hisoblanadi. -->

<!-- ================================================================= -->

<!-- 3-savol: ref(), reactive(), shallowRef() ning bir biridan farqi nimada? -->
<!-- Javob: Bular asosan Vue3'ning composition api'sida ishlatiladi, ref() bu state'da primative data type'li o'zgaruvchi yaratib uni reactivniy o'zgarishi uchun ishlatiladi.
 reactive() esa non-primative data type'li o'zgaruvchilarni reactivny qilish uchun hattoki ichma-ich joylashgan objectlarni ham reactivny o'zgaradigan qilib beradi.
 shallowRef() esa non-primative data type'li o'zgaruvchilarni, ya'ni objectlar ichma-ich joylashgan bo'lsa ham faqat parent objectni reactivny o'zgartiradi, ichidagi child objectlarga ta'sir o'tkazmaydi. -->

<!-- ================================================================= -->

<!-- Assalomu alaykum. Bu file'limizda Vue_JS dan tushishi mumkin bo'lgan ayrim savollar va javoblar toplami mavjud.  -->

<!-- 1-savol: '<template></template>' tagiga v-for loop ishlatilganda key attribute'ni shu template tagining o'ziga bersa bo'ladimi? agar yo'q bo'lsa nima uchun? -->
<!-- Javob:  yo'q berib bo'lmaydi, chunki bu tag DOM'da haqiqiy element sifatida inobatga olinmaydi key attribute esa haqiqiy html elementga berilishi kerak, template ichida haqiqiy element ishlatilsa shunga veriladi -->
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

<!-- 2-savol -->

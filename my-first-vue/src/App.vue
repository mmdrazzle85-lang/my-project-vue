<!-- <template> -->
  <!-- <h1>سلام {{name}}</h1>
  <p>سن من {{ age }}سال است</p>
  <h2>{{ number +number2 }}</h2>
    <h1>{{ count }}</h1> -->

  <!-- <button @click="count++">
    اضافه کردن
  </button>
  <button @click="count--">
    کم کردن
  </button> -->
  <!-- <input v-model="name2" placeholder="نام خود را وارد کنید" type="text"> -->
  <!-- <h2> سلام{{ name2 }}</h2> -->
     <!-- <input v-model="username" placeholder="نام کاربری"> -->

  <!-- <input v-model="age" placeholder="سن"> -->
   <!-- <input  placeholder="نام خود را وارد کنید " v-model="username" type="text"> -->
   <!-- <input placeholder="شهر خود را وارد کنید" v-model="country" type="text"> -->
  <!-- <h1 v-if="isLogin">
    خوش آمدی
  </h1>
  <h2 v-else>
    وارد حساب شوید 
  </h2>
    <button @click="isLogin = !isLogin">
    تغییر وضعیت
  </button> -->
  <!-- <h2>نام: {{ username }}</h2> -->

  <!-- <p>شهر : {{ country }}</p> -->
<!-- </template>
<script setup>
import { ref } from 'vue' -->
<!-- // const name = ref("Ali")
// const age =ref (20)
// const count = ref(0)
// const number=10
// const number2=20
// const name2=ref("")
// const username = ref('')
// const age = ref('')
// const username=ref("")
// const country=ref("") -->
<!-- const isLogin = ref(false) -->
<!-- </script> -->
































<!-- <template>
  <h1>وضعیت </h1>
    <p v-for="product in products">
    {{ product }}
  </p>
  
</template>
<script setup>
const products = [
  "Nike",
  "Adidas",
  "Puma",
  "Reebok",
  "Asics"
]
</script> -->


<!-- <script setup>
import { ref } from 'vue'

const isDisabled = ref(false)
</script>

<template>

  <button :disabled="isDisabled">
    دکمه
  </button>

  <button @click="isDisabled = !isDisabled">
    تغییر وضعیت
  </button>

</template> -->










<!-- <script setup>
const imageUrl = "https://picsum.photos/300/200"
const link = "https://google.com"
</script>

<template>

  <h1>محصول من</h1>

  <img :src="imageUrl">

  <br><br>

  <a :href="link">
    رفتن به گوگل
  </a>

</template> -->






<!-- 

<style>
.red {
  color: red;
}

.green {
  color: green;
}
</style>
<script setup>
import { ref } from 'vue'
const isActive =ref (false)
</script>

<template>
  <h1 :class="{ green: isActive }">
    سلام Vue
  </h1>
  <button @click="isActive=!isActive">clic</button>
</template> -->






<!-- <script setup>
import { ref } from 'vue'

const isVisible = ref(true)
</script>

<template>

  <button @click="isVisible = !isVisible">
    نمایش / مخفی
  </button>

  <h1 v-show="isVisible">
    سلام Vue
  </h1>

</template> -->


<!-- <script setup>
import { ref } from 'vue';
const isVisible=ref(true)
</script>
<template>
  <button @click="isVisible=!isVisible">
    نمایش /مخفی

  </button>
  <h1 v-show="isVisible">v</h1>
</template> -->










<!-- <script setup>
import { ref } from 'vue'

const city = ref('')
</script>

<template>

  <select v-model="city">
    <option value="">انتخاب شهر</option>
    <option value="tehran">تهران</option>
    <option value="mashhad">مشهد</option>
    <option value="kerman">کرمان</option>
  </select>

  <p>شهر انتخاب شده: {{ city }}</p>

</template> -->





<!-- <script setup>
import { ref } from 'vue'

const count = ref(0)

function increase() {
  count.value++
}
</script>

<template>

  <h1>{{ count }}</h1>

  <button @click="increase">
    اضافه کردن
  </button>

</template> -->








<!-- 
<script setup>
import { ref } from 'vue'

const count = ref(0)

function add(number) {
  count.value += number
}
</script>

<template>

  <h1>{{ count }}</h1>

  <button @click="add(1)">
    +1
  </button>

  <button @click="add(5)">
    +5
  </button>

  <button @click="add(10)">
    +10
  </button>

</template> -->









<!-- <script setup>
import { ref, computed } from 'vue'

const price = ref(100000)

const finalPrice = computed(() => {
  return price.value + 10000
})
</script>

<template>

  <p>قیمت اصلی: {{ price }}</p>

  <p>قیمت نهایی: {{ finalPrice }}</p>

</template> -->










<script setup>
import { ref, computed } from 'vue'

const price = ref(50000)
const count = ref(2)

const total = computed(() => {
  return price.value * count.value
})
</script>

<template>

  <p>قیمت: {{ price }}</p>

  <p>تعداد: {{ count }}</p>
  <p>heloo</p>

  <!-- <p>مبلغ کل: {{ total }}</p> -->

  <button @click="count++">
    اضافه کردن محصول
  </button>

</template>
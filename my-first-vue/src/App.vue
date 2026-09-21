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










<!-- <script setup>
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
<!-- 
  <button @click="count++">
    اضافه کردن محصول
  </button> -->

<!-- </template> --> -->




<!-- <script setup>
import { ref, computed } from 'vue'

const price = ref(100000)
const count = ref(2)

const total = computed(() => {
  return price.value * count.value
})
</script>

<template>
  <h2>قیمت محصول: {{ price }}</h2>

  <h2>تعداد: {{ count }}</h2>

  <h2>مبلغ کل: {{ total }}</h2>

  <button @click="count++">
    اضافه کردن
  </button>

  <button @click="count--">
    کم کردن
  </button>
</template> -->
 














<!-- 
<script setup>
import { ref, watch } from 'vue'

const name = ref('')

watch(name, () => {
  console.log('نام تغییر کرد')
})
</script>

<template>
  <h1>نام: {{ name }}</h1>

  <input v-model="name" placeholder="نام خود را وارد کنید">
</template> -->















<!-- <script setup>
import { ref, watch } from 'vue'

const age = ref(15)

watch(age, (newAge, oldAge) => {
  console.log('سن جدید:', newAge)
  console.log('سن قبلی:', oldAge)
})
</script>

<template>

  <h1>سن: {{ age }}</h1>

  <button @click="age++">
    افزایش سن
  </button>


</template> -->


<!-- 



<script setup>
import { ref, watch } from 'vue'

const price = ref(100000)

watch(price, (newPrice, oldPrice) => {
  console.log('قیمت قبلی:', oldPrice)
  console.log('قیمت جدید:', newPrice)
})
</script>

<template>

  <h2>قیمت: {{ price }}</h2>

  <button @click="price += 10000">
    افزایش قیمت
  </button>

</template> -->














<!-- <script setup>
import ProductCard from './components/ProductCard.vue'
</script>

<template>

  <ProductCard
    name="Nike"

    price="2000000"
  />

  <ProductCard
    name="Adidas"
    price="1800000"
  />

</template> -->













<!-- <script setup>
import ProductCard from './components/ProductCard.vue'

const products = [
  { name: 'Nike', price: 2000000 },
  { name: 'Adidas', price: 1800000 },
  { name: 'Puma', price: 1500000 }
]
</script>

<template>

  <ProductCard
    v-for="product in products"
    :key="product.name"
    :name="product.name"
    :price="product.price"
  />

</template> -->














<!-- 

<script setup>
import ProductCard from './components/ProductCard.vue'

const products = [
  {
    name: 'Nike Air',
    price: 2000000,
    category: 'کفش'
  },
  {
    name: 'Adidas Run',
    price: 1800000,
    category: 'کفش'
  },
  {
    name: 'Puma Sport',
    price: 1500000,
    category: 'لباس'
  }
]
</script>

<template>

  <ProductCard
    v-for="product in products"
    :key="product.name"
    :product="product"
  />

</template> -->









<!-- <script setup>
import ProductCard from './components/ProductCard.vue'

function addToCart() {
  console.log('محصول به سبد اضافه شد')
}
</script>

<template>
  <ProductCard @addToCart="addToCart" />
</template> -->











<!-- <script setup>
import ProductCard from './components/ProductCard.vue'

function addToCart(productName) {
  console.log(productName)
}
</script>

<template>
  <ProductCard @addToCart="addToCart" />
</template> -->








<!-- 
<script setup>
import { ref } from 'vue'
import ProductCard from './components/ProductCard.vue'

const cartCount = ref(0)

const products = [
  {
    name: 'Nike Air',
    price: 2000000
  },
  {
    name: 'Adidas',
    price: 1800000
  },
  {
    name: 'Puma',
    price: 1500000
  }
]

function addToCart(product) {
  cartCount.value++

  alert(product.name + ' به سبد اضافه شد')
}
</script>

<template>
  <h1>فروشگاه</h1>

  <h2>تعداد محصولات سبد: {{ cartCount }}</h2>

  <ProductCard
    v-for="product in products"
    :key="product.name"
    :product="product"
    @addToCart="addToCart"
  />
</template> -->
















<!-- 
<script setup>
import Card from './components/Card.vue'
</script>

<template>

  <Card>
    <h2>کفش Nike</h2>
    <p>قیمت: 2 میلیون تومان</p>
  </Card>

</template> -->










<!-- 

<script setup>
import Card from './components/Card.vue'
</script>

<template>

  <Card>

    <template #header>
      <h2>کفش Nike</h2>
    </template>

    <template #body>
      <p>قیمت: 2 میلیون تومان</p>
      <p>رنگ: مشکی</p>
    </template>

    <template #footer>
      <button>خرید</button>
    </template>

  </Card>

</template> -->














<!-- 
<script setup>
import { ref } from 'vue'

const input = ref(null)

function focusInput() {
  input.value.focus()
}
</script>

<template>
  <input ref="input" placeholder="نام خود را وارد کنید">

  <button @click="focusInput">
    رفتن روی Input
  </button>
</template> -->















<!-- <script setup>
import { ref, onMounted } from 'vue'

const input = ref(null)

onMounted(() => {
  input.value.focus()
})
</script>

<template>
  <input ref="input">
</template> -->





















<!-- <script setup>
import { ref, onMounted } from 'vue'

const input = ref(null)

onMounted(() => {
  input.value.focus()
})
</script>

<template>
  <h1>ثبت نام</h1>

  <input
    ref="input"
    placeholder="نام خود را وارد کنید"
  >
</template> -->






















<!-- 
<script setup>
import { ref } from 'vue'
import search from './components/SearchBox.vue'



const show = ref(true)
</script>

<template>
  <button @click="show = !show">
    نمایش / مخفی
  </button>

  <h1 v-if="show">
    سلام Vue
  </h1>
  <searchBox></searchBox>
</template> -->






















<!-- 
<script setup>
import { ref } from 'vue'
import SearchBox from './components/SearchBox.vue' -->

<!-- // const searchText = ref('')

// function search(value) {
//   searchText.value = value
// } -->
<!-- // </script> -->

<!-- // <template>
//   <h1>فروشگاه</h1>

//   <SearchBox @search="search" />

//   <h2>جستجوی شما:</h2>

//   <p>{{ searchText }}</p>
// </template> -->





<script setup>
import { ref } from 'vue'

const name = ref('')

function submitForm() {
  console.log(name.value)
}
</script>

<template>
  <input
    v-model="name"
    placeholder="نام خود   "
  >

  <button @click="submitForm">
    ثبت
  </button>
</template>
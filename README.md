# vas-ui
VasUI - Vue3 Template for Vue-Reactive UI Components

VasUI is not a library or framework. There is no npm installation control for the UI components.

Just clone the files to your project folder and use.

### It is a somehow Vue Community Project.
* Please use disucssion to express
* Please make the better components using Pull Requests

## Why VasUI
* I do not want to use any framework CLI (Quasar Framework)
* I want different component styles (Vuesax, PrimeVue, Vertify, Quasar, ElementUI, ...)
* I want FULL customizability - Just edit the VasUI files
* [Vue 3](https://v3.vuejs.org/) based - fast, typescript supported, for both small and large scale application development
* All Coding with `.vue` and `<script setup>` (`<script setup lang="ts">`)
* Under [MIT License](https://raw.githubusercontent.com/cyfung1031/vas-ui/main/LICENSE) - free to edit and distribute for both commerical and open source projects

## VasUI Highlights
* You can use them in any Vue Projects

## VasUI Concept

### no web component 
* just make your component with [TailwindCSS](https://tailwindcss.com/) / [WindiCSS](https://windicss.org/)
### no `v-model` for Vue Component
* For non DOM Component, `v-model` is the worst design ever in Vue. 
* You are wasting time to create codes in different components (calling emits and defining emits)
* `v-model` is only useful for DOM Element (like `<input>`, `<textarea>`)
### no need to struggle with `reactive()` / `ref()`
* `ref()` - within the same component
* `vas` - across different components
### Introduction of `refDom()`
* A non-reactive stuff for Vue Component's DOM Element Management
* assign in `<template>` - `:ref="vas.myDOM.setRef"`
* read in `<script>` - `vas.myDOM.refVal`


## Coding Example


[SFC Playground - Example 1](https://sfc.vuejs.org/#eyJBcHAudnVlIjoiPHNjcmlwdCBzZXR1cD5cbiAgaW1wb3J0IHsgcmVmLCByZWFjdGl2ZSB9IGZyb20gJ3Z1ZSdcbiAgaW1wb3J0IENvbXAxIGZyb20gJy4vQ29tcDEudnVlJ1xuICBpbXBvcnQgQ29tcDIgZnJvbSAnLi9Db21wMi52dWUnXG5cbiAgY29uc3QgaW5wdXRWYWx1ZSA9IHJlZignSGVsbG8gV29ybGQhJylcbiAgY29uc3QgY29sb3IgPSByZWYoMClcbiAgY29uc3QgdmFzID0gcmVhY3RpdmUoe1xuICAgIGlucHV0VmFsdWUsXG4gICAgY29sb3JcbiAgfSlcblxuPC9zY3JpcHQ+XG5cbjx0ZW1wbGF0ZT5cbiAgPENvbXAxIDp2YXM9XCJ2YXNcIj48L0NvbXAxPlxuICA8Q29tcDIgOnZhcz1cInZhc1wiPjwvQ29tcDI+XG48L3RlbXBsYXRlPiIsImltcG9ydC1tYXAuanNvbiI6IntcbiAgXCJpbXBvcnRzXCI6IHtcbiAgICBcInZ1ZVwiOiBcImh0dHBzOi8vc2ZjLnZ1ZWpzLm9yZy92dWUucnVudGltZS5lc20tYnJvd3Nlci5qc1wiXG4gIH1cbn0iLCJDb21wMS52dWUiOiI8dGVtcGxhdGU+XG5cdDxpbnB1dCBcbiAgICAgICAgIHYtbW9kZWw9XCJ2YXMuaW5wdXRWYWx1ZVwiXG4gICAgICAgICA6Y2xhc3M9XCJ7J3JlZCc6IHZhcy5jb2xvcj09MCwgJ2JsdWUnOiB2YXMuY29sb3I9PTF9XCJcbiAgICAgICAvPlxuPC90ZW1wbGF0ZT5cbjxzY3JpcHQgc2V0dXA+XG4gIGltcG9ydCB7IHJlZiwgcmVhY3RpdmUsIGRlZmluZVByb3BzIH0gZnJvbSAndnVlJ1xuICBjb25zdCBwcm9wcyA9IGRlZmluZVByb3BzKHtcbiAgICB2YXM6IHtcbiAgICAgIHJlcXVpcmVkOnRydWVcbiAgICB9XG4gIH0pXG4gIGNvbnN0IHZhcyA9IHByb3BzLnZhc1xuPC9zY3JpcHQ+XG48c3R5bGU+XG4gIC5yZWQge1xuICAgIGNvbG9yOiByZWRcbiAgfVxuICAuYmx1ZSB7XG4gICAgY29sb3I6IGJsdWVcbiAgfVxuPC9zdHlsZT4iLCJDb21wMi52dWUiOiI8dGVtcGxhdGU+XG4gIDxkaXY+bGFzdE1lc3NhZ2U6IHt7IGxhc3RNZXNzYWdlIH19PC9kaXY+XG4gIDxkaXY+bmV3TWVzc2FnZToge3sgbmV3TWVzc2FnZSB9fTwvZGl2PlxuICA8YnV0dG9uIEBjbGljaz1cInZhcy5jb2xvciA9ICh2YXMuY29sb3IgKyAxKSUyXCI+XG4gICAgQ2hhbmdlIENvbG9yXG4gIDwvYnV0dG9uPlxuPC90ZW1wbGF0ZT5cbjxzY3JpcHQgc2V0dXA+XG4gIGltcG9ydCB7IHJlZiwgcmVhY3RpdmUsIGRlZmluZVByb3BzLCB3YXRjaCB9IGZyb20gJ3Z1ZSdcbiAgY29uc3QgcHJvcHMgPSBkZWZpbmVQcm9wcyh7XG4gICAgdmFzOiB7XG4gICAgICByZXF1aXJlZDp0cnVlXG4gICAgfVxuICB9KVxuICBjb25zdCB2YXMgPSBwcm9wcy52YXNcbiAgY29uc3QgbGFzdE1lc3NhZ2UgPSByZWYobnVsbClcbiAgY29uc3QgbmV3TWVzc2FnZSA9IHJlZihudWxsKVxuICB3YXRjaCgoKT0+dmFzLmlucHV0VmFsdWUsIChjU3RhdGUsIHBTdGF0ZSk9PntcbiAgICBsYXN0TWVzc2FnZS52YWx1ZSA9IHBTdGF0ZVxuICAgIG5ld01lc3NhZ2UudmFsdWUgPSBjU3RhdGVcbiAgfSlcbjwvc2NyaXB0PiJ9)

* App.vue
```vue
<script setup>
  import { ref, reactive } from 'vue'
  import Comp1 from './Comp1.vue'
  import Comp2 from './Comp2.vue'

  const inputValue = ref('Hello World!')
  const color = ref(0)
  const vas = reactive({
    inputValue,
    color
  })

</script>

<template>
  <Comp1 :vas="vas"></Comp1>
  <Comp2 :vas="vas"></Comp2>
</template>
```

* Comp1.vue
```vue
<template>
	<input 
         v-model="vas.inputValue"
         :class="{'red': vas.color==0, 'blue': vas.color==1}"
       />
</template>
<script setup>
  import { ref, reactive, defineProps } from 'vue'
  const props = defineProps({
    vas: {
      required:true
    }
  })
  const vas = props.vas
</script>
<style>
  .red {
    color: red
  }
  .blue {
    color: blue
  }
</style>
```

* Comp2.vue
```vue
<template>
  <div>lastMessage: {{ lastMessage }}</div>
  <div>newMessage: {{ newMessage }}</div>
  <button @click="vas.color = (vas.color + 1)%2">
    Change Color
  </button>
</template>
<script setup>
  import { ref, reactive, defineProps, watch } from 'vue'
  const props = defineProps({
    vas: {
      required:true
    }
  })
  const vas = props.vas
  const lastMessage = ref(null)
  const newMessage = ref(null)
  watch(()=>vas.inputValue, (cState, pState)=>{
    lastMessage.value = pState
    newMessage.value = cState
  })
</script>
```

### Vue 例子

```javascript
<template>
    <div v-if="initCells <= 0">{{initCells}}</div>
    <div v-else>{{initCells}}<Cells :initCells="initCells - 1" /></div>
</template>

<script>
export default {
    name: 'Cells',
    props: ['initCells']
}
</script>
```
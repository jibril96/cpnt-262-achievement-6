<template>
<div class="Tickets"
    v-for= "(Tickets, index) in Tickets" :key=" 'tic' +index">
    <div class=”title”>{{Tickets.title}}</div>
    <div class=”price”>{{Tickets.price}}</div>
</div>

</template>

<script>
export default {
Data: () => {
return {
Tickets: [ 
{ title: 'one month trip', price:  1000},
{ title: 'two month trip', price: 1500},
{title: 'three month trip', price: 2000},
]
}
}
}
</script>

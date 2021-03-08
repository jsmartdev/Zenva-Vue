let firstVue = new Vue({
    el: '#firstDiv',
    data: {
        number: 1,
        numbers: [1, 2, 3],
    }
})    
let secondVue = new Vue({
    el: '#secondDiv',
    data: {
        isDoorOpen: false
    },
    methods: {
        openCloseDoor: function() {
            this.isDoorOpen = !this.isDoorOpen
        }
    }
})

Vue.component('grocery-item', {
    props: ['groceryitem'],
    template: '<li>{{ groceryitem.name }} {{ groceryitem.quantity}}</li>'
})

let thirdVue = new Vue({
    el:'#thirdDiv',
    data: {
        groceryItems: [
            {name: 'Bread', quantity: 2},
            {name: 'Cheese', quantity: 3},
            {name: 'Wine', quantity: 4}
        ]
    } 
})
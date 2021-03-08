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
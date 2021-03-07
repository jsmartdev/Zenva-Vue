let firstVue = new Vue ({
    el: '#firstDiv',
    data: {
        number: 1
    }
})

firstVue.number = 5

firstVue.$watch('number', function() {
    alert('number has changed')
})

firstVue.number = 10

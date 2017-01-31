<template>
    <table class="table table-hover product-table">
        <thead>
            <tr>
                <th>Name</th>
                <th>Description</th>
                <th>Price</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="product in products" track-by="id">
                <td>{{product.name}}</td>
                <td>{{product.description}}</td>
                <td>{{product.price}}</td>
            </tr>
        </tbody>
    </table>
</template>
<script>
export default {
    data() {
        return {
            products: [{
                    id: '24u2424lk22l42l42l4l4',
                    name: 'cobol 101 vintage',
                    description: 'Learn Cobol with this vintage programming book',
                    price: 399,
                },
                {
                    id: '32424lkj24u2424lk22l42l42l4l4',
                    name: 'Sharp C2719 curved TV',
                    description: 'Watch TV like never before iwht the brand new curved screen technology',
                    price: 1995,
                },
                {
                    id: '24u2l42l4l4',
                    name: 'Remmington X mechanical keyboard',
                    description: 'Excellent for gaming and typing, this Remmington X keyboard features tactile, clicky switches for speed and accuracy',
                    price: 595,
                }
            ]


        }
    }
}
</script>
<style>
.header {
    font-size: 4rem;
}
</style>

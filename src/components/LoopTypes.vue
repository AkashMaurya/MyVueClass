<template >
    <div>
        <h1>Loops</h1>
        <ul>
            <!-- <li " v-for=" items in technology" :key="items">{{ items }}</li> -->
        </ul>
        <table class="table table-dark table-hover">
            <thead>
                <tr>
                    <th scope="col">Sr. no</th>
                    <th scope="col">First</th>
                    <th scope="col">Last</th>
                    <th scope="col">Handle</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="items1 in Users" :key="items1">
                    <td>{{ items1.Sro }}</td>
                    <td>{{ items1.name }}</td>
                    <td>{{ items1.email }}</td>
                    <td>{{ items1.place }}</td>
                </tr>
            </tbody>
        </table>

    </div>
</template>
<script>
export default {
    name: "LoopsTypes",
    data() {
        return {
            // technology: ['java', 'C++', 'Android', 'Swift', 'Python'],
            Users: [{
                Sro: '1',
                name: 'akash',
                email: 'akash@gmail.com',
                place: 'Delhi'
            },
            {
                Sro: '2',
                name: 'prakash',
                email: 'prakash@gmail.com',
                place: 'mumbai'
            },
            {
                Sro: '3',
                name: 'kavita',
                email: 'kavita@gmail.com',
                place: 'pune'
            },]
        }

    }
}
</script>
<style scoped>
#myList {
    list-style-type: none;
    font-size: 2em;
    display: flex;
    flex-direction: row;
}
</style>
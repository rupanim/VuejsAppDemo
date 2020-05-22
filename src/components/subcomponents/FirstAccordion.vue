<template>
    <div>
         <!-- <b-card no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                    <b-button block href="#" v-b-toggle.accordion-1 variant="info">Devices</b-button>
                </b-card-header>
                <b-collapse id="accordion-1" visible accordion="my-accordion1" role="tabpanel">
                    <b-card-body>
                    <ul>
                            <li v-for="deviceCategory in deviceCategories" :key="deviceCategory.id">
                                {{deviceCategory.name}}
                            </li>
                        </ul>
                    </b-card-body>
                </b-collapse>
            </b-card>  -->         
            <b-card no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                    <b-button block href="#" v-b-toggle.accordion-1 variant="info">User Name from Mock API</b-button>
                </b-card-header>
                <b-collapse id="accordion-1" visible accordion="my-accordion1" role="tabpanel">
                    <b-card-body>
                    <div v-if="usersListFromParent == null">
                        <label> No Data from API. Click on button in the 3rd accordion. </label>
                    </div>
                    <ul v-if="usersListFromParent != null">
                            <li v-for="user in usersListFromParent" :key="user.id">
                                {{user.name}}
                            </li>
                        </ul>
                    </b-card-body>
                </b-collapse>
            </b-card>           
    </div>  
</template>

<script>
// import axios from 'axios';

export default {
    name: 'FirstAccordion',
    props:{
        usersListFromParent: Array
    }
    // mounted: function() {
    //         axios.get('https://jsonplaceholder.typicode.com/users')
    //         .then(response => this.apiReturn = response.data);
    //     },
    // data(){
    //     return {
    //          apiReturn: null,
    //     }
    // }
}
</script>

<style scoped>

</style>
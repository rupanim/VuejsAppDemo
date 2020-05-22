<template>
  <div>
            <b-card no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                    <b-button block href="#" v-b-toggle.accordion-3 variant="info">Input Form</b-button>
                </b-card-header>
                <b-collapse id="accordion-3" visible accordion="my-accordion3" role="tabpanel">
                    <b-card-body>
                        Family<br />                                            
                            <b-form-select v-model="selected" :options="options"></b-form-select>
                            <br />
                            <div class="mt-2">
                                RMS Delay Spread Scale (ns)<br />
                                <b-form-select v-model="selectedRMS" :options="optionsRMS"></b-form-select>                                                
                            </div>
                            <div class="mt-2">
                                <b-button @click="getAPICall">Click to make API call</b-button>       
                            </div>
                    </b-card-body>
                </b-collapse>
            </b-card> 
    </div>  
</template>

<script>

import axios from 'axios';

export default {
    name: 'ThirdAccordion',
    data() {
        return {
            apiReturn: null,
            selected: null,
                selectedRMS: 10,
                optionsRMS: [                    
          { value: '10', text: '10' },
          { value: '30', text: '30' },
          { value: '100', text: '100' },
          { value: '1000', text: '1000' }
                ],
                options: [
                    { value: null, text: 'Select Propagation Model Family' },
          { value: 'a', text: 'CDL-A' },
          { value: 'b', text: 'CDL-B' },
          { value: { C: '3PO' }, text: 'CDL-C' },
          { value: 'd', text: 'CDL-D', disabled: true }
                ],
        }
    },
    methods :{
        getAPICall(){            
           // alert('get api call');
            axios.get('https://jsonplaceholder.typicode.com/users')
            .then(response => {
                this.apiReturn = response.data;
                
                this.$emit('childToParent', response.data);
                
                });           
        }
    }
}
</script>

<style scoped>

</style>

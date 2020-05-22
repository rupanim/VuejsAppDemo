<template>
<div>
    <div class="row col-md-12" style="padding-top: 15px">           
        <div class="col-md-4">            
            <FirstAccordion :usersListFromParent="apiReturn" />           
        </div>
        <div class="col-md-4">   
           <SecondAccordion />            
        </div>
        <div class="col-md-4">  
            <ThirdAccordion @childToParent="getCallInParent"/>
        </div>
    </div>
</div>
</template>

<script>
import PdpPlot from "../components/subcomponents/PdpPlot.vue"
import InputForm from "../components/subcomponents/InputForm.vue"
import FirstAccordion from "../components/subcomponents/FirstAccordion.vue";
import SecondAccordion from "../components/subcomponents/SecondAccordion.vue";
import ThirdAccordion from "../components/subcomponents/ThirdAccordion.vue";

    export default {
        name: 'Emulation',       
        components: {
            PdpPlot,
            InputForm,
            FirstAccordion,
            SecondAccordion,
            ThirdAccordion
        },
        methods: {
            getCallInParent(data){
                this.apiReturn = data;                      
            }
        },
        data() {
            return {                
                imgLink :  '../../../public/images/emulator_back_mt.svg',
                apiReturn: null,
                deviceCategories: [
                    {
                        id: '1',
                        name: 'Channel Emulator'
                    },
                    {
                        id: '2',
                        name: 'Base Station'
                    },
                    {
                        id: '3',
                        name: 'Mobile Station'
                    }
                ]
            }
        }
    };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.custom{
    background-color: #1171a3;
    border: 1px solid #1171a3;
    color: #fff;
}
.customDevices{
    background-color: #1171a3;
    border: 1px solid #1171a3;
    color: #fff;
}
</style>
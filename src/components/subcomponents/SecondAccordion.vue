<template>
     <b-card no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                    <b-button block href="#" v-b-toggle.accordion-2 variant="info">Testbed</b-button>
                </b-card-header>
                <b-collapse id="accordion-2" visible accordion="my-accordion2" role="tabpanel">
                    <b-card-body>
                    <svg width="550" height="480" data-ng-attr-viewBox="0 0 550 480" class="svgTransform">                                                                        
                        <g transform="matrix(1,0,0,1,0,0)" opacity="1" fill-rule="inherit">
                            <image preserveaspectratio="none"
                                    xlink:href="../../../public/images/emulator_back_mt.svg"
                                    
                                    height="400"
                                    width="375"
                                    x="85"
                                    y="-10">
                            </image>
                        </g>
                    </svg>
                    </b-card-body>
                </b-collapse>
            </b-card>          
</template>

<script>
export default {
    name: 'SecondAccordion',
}
</script>

<style scoped>

</style>
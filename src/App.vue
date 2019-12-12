<template>
  <div id="app">
    <div style="margin:10% 25%; width:250px;" >

    <!-- diacritic filtering code snippet -->
    <ejs-combobox :dataSource='dataItem' 
    placeholder='Select a value' popupWidth="250px" 
    popupHeight="200px" allowFiltering='true' :ignoreAccent='true'>
    </ejs-combobox>

    <!-- grouping and filtertypes code snippet -->
    <!-- <ejs-combobox :dataSource='dataItem' :fields='dataFields' 
    placeholder='Select a value' popupWidth="250px" 
    popupHeight="200px" allowFiltering='true' filterType='Contains'
    :ignoreCase='false'>
    </ejs-combobox> -->
    </div>
  </div>
</template>

<script>
import Vue from "vue";
import { ComboBoxPlugin} from '@syncfusion/ej2-vue-dropdowns';
Vue.use(ComboBoxPlugin);
export default Vue.extend({
  data: function() {
    return {
      // diacritics filtering data source
      dataItem: [
            'Aeróbics',
            'Aeróbics en Agua',
            'Aerografía',
            'Aeromodelaje',
            'Águilas',
            'Ajedrez',
            'Ala Delta',
            'Álbumes de Música',
            'Alusivos',
            'Análisis de Escritura a Mano'
      ]
      // grouping and filtertypes data source

      // dataItem: [
      //   { Name: 'Cabbage', Category: 'Leafy and Salad', Id: 'item1' },
      //   { Name: 'Spinach', Category: 'Leafy and Salad', Id: 'item2' },
      //   { Name: 'Wheat grass', Category: 'Leafy and Salad', Id: 'item3' },
      //   { Name: 'Yarrow', Category: 'Leafy and Salad', Id: 'item4' },
      //   { Name: 'Pumpkins', Category: 'Leafy and Salad', Id: 'item5' },
      //   { Name: 'Chickpea', Category: 'Beans', Id: 'item6' },
      //   { Name: 'Green bean', Category: 'Beans', Id: 'item7' },
      //   { Name: 'Horse gram', Category: 'Beans', Id: 'item8' }
      //   ],
      // dataFields: { 
      //   groupBy: 'Category', 
      //   text: 'Name', 
      //   value: 'Id' }    
    };
  }
});
</script>




<style>
@import url(https://cdn.syncfusion.com/ej2/material.css);
</style>

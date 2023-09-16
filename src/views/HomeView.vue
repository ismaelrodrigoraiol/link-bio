<script setup>
import { ref, onMounted } from 'vue'
import Item from '../components/Item.vue'
import dados from '../assets/dados/db.json'

let servicos = ref(null)

    
  
  onMounted(() =>{
    servicos.value = dados
    //*let target = "https://raw.githubusercontent.com/yurimarcon/link-services/main/src/Dados/Services.json";
    //fetch(target)
      //.then(res => res.json())
      //.then(res => servicos.value = res)
      //.catch(e => console.log(e))
  })
</script>

<template>
  <div><img alt="Profile" src="https://lh3.googleusercontent.com/fife/AKsag4OyDU8MQCUjcg06wiTxDlU8Cr6ewQtGbKDJ32OHATlwyjsJUq8GbxjqkqWcE-5QLtboXQQAR9S0y-KQeA1D3hihfG22qTb0Y23w8jFSCQxa7uTrqa0O9tIlBEZpJ_BibWmJ-e8g289Q_dTasIdOB2cUQca5ctwAo9epkQ-J5gn92BlGd5b74oTPPX0CtWJQZ1ICW4mEX79AmLBna135YNsPdzEIWoQdbne_h0Ig6tFt-L3d8p82VFWiI7iDDJd5tbYOV8uE0h9k4Sph4kUwv6pOA9IGJoo2igEJ_3h_lpusQ2XdUosgLowpMLwOOSsK8ypatA7UVK76URZ7MKX-jLdDDQHqj_7ewOSqfPCK_fhgEY9vdBL_QVlty_loXOPSiCmWpjOZdH3RFoCK373_8KaxRrNYVg0lqHYtdVgCwm1lgZ3udX8C66L7lEUff8Cwy_688aAO5CTwAA0RK3BzQlmYiom83JAerTrQV3fkz51JS8CTt0ZegNkjdDJrPqrrlDZQMPK_DbzUA2ZT4z3_ubEMy6Kq9bgdF2KseNz9NsSmsYPIvz9Jbv4-50XffhXyjVgOQbE6roUhXHLlFEP-CPukLvykVoIBXAFVfw8z3X8GKTMCyVbTMUVSO2_56G6d7S-_pB6OA79vjeP_NgpQjy8dvpx16ErxssjwZvhsmXz6E_EJhMI85gxKZrWLohodcBxzWPZ5leKUkUBmXzyZU1PTMHPACZggNecsXJcDD6JgLZxG-YWI16WszaAqPWsiWFrURRs6jhZ70lUhwtZZKEyIRIV6_kHfmP1zNxQccuz_UDIxSoKcQnPzPVuqoA6vWf9Q7DoanLgd2OIKwAHUH8qWXc5q5LeTSBksoW45sx5ThJp_HOAW4f08y0kF4VhNJzK-lxTLkX36BHadzo2YWkfizedpp59FM5qPaenzELtNwb2dMJrmphpTVDjFPpAJ3sAFSWl-wT6JXMzH67KFvOhJLpEi9uk6AAn9C6CtmYxo21t7XHnKFgR7VOdKJmV8g4rOg-JoLU5cPA-DvyIe30KAElnRm2DgZo9FpIooIUs3uukPi1TXIK_sEhjl6pcep5z8jdwvUhI_Azgalr_zvh3l_g8Iu_oACLc1QqN_ImhGn2SJgykusDtoB-HuPDLsuw6r-dtOc0hWh2dPfa4VMOrbs26ZsY-YMVvemjbHYivsYIvayaCnaP8pEAsbTnYUbxhQNhIq9QsS4QYN7ZSgGukMZGv11f_oz_7uNlHY5GIqnb_xm1r4YUdhiAFHzMULmiPquH9mGOxGaQ_EHIrFGUvsrFvQnoWaQpM2M7adh-wKmy8f1H5EWlbMN3_0cjVQ1hA1o9SPhFG8V17qEMhKxwvK9Qx41wbFFOa713Pg08UenD3NSPwl08--w1VoVD5WIv9VSyUqGR37rPxkFK_96vjE7GYdbkGXfRC8HGBs1PJu4ydlqam_R3Q3gTLp7qVgdZQqi2vIgoeNBbrCF55WBOukLHzWnSZlk3HRTFqwfYZLvzPbcXylAqiec6H9Kk5SmpqWtiOJ=w1360-h657"/></div>
  
  
  <h1>Ismael Rodrigo Raiol</h1>
  <hr/>
  <blockquote cite="Mahatma Gandhi">
    <p>
      "Seja a mudança que você quer ver no mundo"
      <small> - Mahatma Gandhi - </small>
    </p>
  </blockquote>
  
  <div class="items">
    <Item 
    v-for="servico, index in servicos"
    :key="index"
    :item="servico"
    />
   </div>
  </template>

  <style scoped>
  .items{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

  img {
    padding-top: 1%;
    width:250px; 
    border-radius:115%;
  }
  
  </style>


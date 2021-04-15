<template>


 <div id="CV">

        <div id="infoPersonnel">        
            <h4>{{form1.name}}</h4>
            <p>{{form1.age}}</p>
            <p>{{form1.address}}</p>
            <p>{{form1.phone}}</p>
            <email>{{form1.email}}</email>
        </div>

           <div id="title">       
              <h2>{{form1.specialité}}</h2>
          </div> 

        <div id="pics">
           <img src="../assets/user.png" />
        </div>

    





<div class="formation">       
  <h4>FORMATION</h4>
</div>
<div class="info-formation">
  <div style=" width: 20%; margin: auto;">
    <div class="langue">
    <h5 class="lg">{{form2.date1}}</h5>
    <p class="lg">{{form2.formation1}}</p>
    </div>

    <div class="langue">
    <h5 class="lg">{{form2.date2}}</h5>
    <p class="lg">{{form2.formation2}}</p>
    </div>
    <div class="langue">
    <h5 class="lg">{{form2.date3}}</h5>
    <p class="lg">{{form2.formation3}}</p>
      </div>
  </div>
</div>


    
<div class="formation">       
  <h4>EXPÉRIENCES PROFESSIONNELLES</h4>           
</div> 

<div class="info-formation">
  <div style=" width: 20%; margin: auto;">
      <div class="langue">
    <h5 class="lg">{{form3.date1}}</h5>
    <p class="lg">{{form3.experience1}}</p>
      </div>
      <div class="langue">

    <h5 class="lg">{{form2.date2}}</h5>
    <p class="lg">{{form2.formation2}}</p>
      </div>
   <div class="langue">
    <h5 class="lg">{{form3.date2}}</h5>
    <p class="lg">{{form3.experience2}}</p>
      </div>
</div>
</div> 

<div class="formation">       
  <h4>LANGUES</h4>         
</div>

<div class="info-formation">
  <div style=" width: 20%; margin: auto;">
  <div class="langue">
    <h5 class="lg">{{form4.type1}}</h5>
    <p class="lg">{{form4.langue1}}</p>
</div>
<div class="langue">
    <h5 class="lg">{{form4.type2}}</h5>
    <p class="lg">{{form4.langue2}}</p>
</div>
<div class="langue">
    <h5 class="lg">{{form4.type3}}</h5>
    <p class="lg">{{form4.langue3}}</p>
</div>
<div class="langue">
    <h5 class="lg">{{form4.type4}}</h5>
    <p class="lg">{{form4.langue4}}</p>
</div> 
</div>
</div>
<div class="formation">       
  <h4>CENTRES D’INTERET</h4>         
</div>
<div class="info-formation">
    <div style=" width: 20%; margin: auto;">
      <div class="langue">
    <p>{{form3.experience1}}</p>
      </div>
    <div class="langue">
    <p>{{form5.loiser2}}</p>
    </div>
    <div class="langue">
    <p>{{form5.loiser3}}</p>
      </div>
    </div>
</div> 
</div> 


     


</template>


 <script>
  export default {



    data() {
      return {

        form1: {},
        form2: {},
        form3: {},
        form4: {},
        form5: {},

      }
    },
    mounted() {

      this.form1 = JSON.parse(localStorage.getItem('form1'))
      this.form2 = JSON.parse(localStorage.getItem('form2'))
      this.form3 = JSON.parse(localStorage.getItem('form3'))
      this.form4 = JSON.parse(localStorage.getItem('form4'))
      this.form5 = JSON.parse(localStorage.getItem('form5'))

    }

  }
</script>
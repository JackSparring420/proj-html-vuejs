<template>
  <section>
    <div class="pink"></div>
    <div class="blue"></div>
    <div id="dj-avada">
        <h4>RESIDENT DJ</h4>
        <h2>dj avada</h2>
        <button>VIEW PROFILE</button>
    </div>
    <div id="dj-blondie">
        <h4>SPECIAL GUEST DJ</h4>
        <h2>dj blondie</h2>
        <button>VIEW PROFILE</button>
    </div>
  </section>
</template>


<script>
export default {
  name: "Dj",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section{
    text-align: left;
    #dj-avada{
        float: left;
        width: 50%;
        height: 600px;
        background-image: url("../assets/img/avada-nightclub-resident-profile.jpg");
        background-size: cover;
        background-position: center;

        h4 {
         color: #f53c81;
         margin: 50px 50px 20px 50px;
        }
    
        button{

            background-color: #4da4dd;
            color: white;
            border: 1px solid #4da4dd;
            padding: 10px 20px;
            margin: 25px 50px;
        }
    }
    #dj-blondie{
        float: left;
        width: 50%;
        background-image: url("../assets/img/avada-nightclub-lisahouse-inset-new.jpg");
        height: 600px;
        background-size: cover;
        background-position: top;

        h4 {
        color: #4da4dd;
        margin: 50px 50px 20px 50px;
        }
    
        button{
            background-color: #f53c81;
            color: white;
            border: 1px solid #f53c81;
            padding: 10px 20px;
            margin: 25px 50px;
        }
    }
    .pink {
        width: 50%;
        float: left;
        height: 5px;
        background-color: #f53c81;
    }
    .blue {
        width: 50%;
        float: left;
        height: 5px;
        background-color: #4da4dd;
    }
    
    h2 {
        font-size: 50px;
        margin: 0 50px ;
    }
}
section::after{
  content: "";
  display: table;
  clear: both;
}
</style>
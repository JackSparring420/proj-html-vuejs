<template>
    <section>
        <div id="contain">
            <div>
                <h4>BECOME A VIP TONIGHT</h4>
                <h2>exlusive vip lounge</h2>
            </div>
            <button> <strong>JOIN THE CLUB</strong> </button>
        </div>
    </section>
</template>

<script>
export default {
  name: 'VipLonge',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    section{
        background-image: url("../assets/img/avada-nightclub-vip-hero-new.jpg");
        background-size: cover;
        background-position: center;
        text-align: left;
        #contain {
            width: 70%;
            margin: auto;
            display: flex;
            justify-content: space-between;
            padding: 100px;
            h4{
                color: #4da4dd;
            }
            h2{
                font-size: 45px;
            }
            button {
                    height: 50px;
                    background-color: #f53c81;
                    color: white;
                    border: 1px solid #f53c81;
                    padding: 0 60px;
              }
        }
    }
</style>

<template>
  <div>
    <div class="container"><h1>Parallax Image Effect </h1> 
    </div>
    <div class="container"><h6>Cengiz Efe Acet</h6></div>
    <p>
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Magnam sequi
      rerum tempore, ea fugit obcaecati natus minima ut suscipit velit. Autem
      distinctio natus, voluptatum nulla ipsa saepe corporis. Facere itaque unde
      illum tenetur repudiandae rem, pariatur ipsam quis maiores laborum aut
      porro vero atque velit necessitatibus quibusdam fuga blanditiis eum, culpa
      dicta quam cum ullam dolor! Quod alias suscipit velit inventore dolor vel
      eaque ex quae, corporis aliquid, obcaecati sequi dicta nihil placeat odit
      odio. Ab nemo quisquam magnam aut perspiciatis, asperiores inventore
      doloribus iste ratione. Deserunt maxime debitis dignissimos voluptates
      similique numquam nisi recusandae necessitatibus magnam, natus nihil, ex
      reiciendis, dolorum assumenda deleniti eveniet voluptas dolores delectus
      ipsam. Repellat tempora corrupti tempore quasi aut blanditiis adipisci
      laborum saepe, non eius illum obcaecati perspiciatis accusantium fugit
      dolores iure beatae omnis similique sunt aliquid repellendus incidunt.
      Doloribus similique minima voluptatum incidunt, fugiat quam hic facilis,
      omnis inventore ab soluta officiis eligendi voluptates aliquam dignissimos
      unde corrupti nobis est maiores debitis magni ipsa eos ea cumque! Sunt
      placeat fugit, earum quasi ad fuga odit ea excepturi exercitationem minus.
      Placeat distinctio optio error officia ut delectus modi officiis at,
      maiores itaque est assumenda doloremque nobis adipisci corporis
      dignissimos numquam. Illo pariatur dolorum blanditiis!
    </p>
    <div
      class="container"
    >
      <parallax-image
        :imageUrl="'/sky.jpg'"
        :intensity="0.15"
        :width="'50vw'"
        height="200px"
        :direction="'Horizontal'"
        :transition="'transform 0.3s ease-out'"
      ></parallax-image>
    </div>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis,
      autem? Itaque sit ipsam iste culpa eveniet sed, repellendus quas repellat
      labore harum ex saepe cupiditate asperiores delectus, tenetur dolorum nam
      ad. Voluptatum consectetur veritatis voluptate aliquid dolorum esse maxime
      temporibus deleniti dolores eum laudantium similique animi exercitationem,
      sed ut illo ea, veniam fuga ipsa voluptates? Labore obcaecati, similique
      perspiciatis, tempora sed libero, hic maxime voluptates quos vel illo
      quaerat praesentium blanditiis dolore? Consequuntur dolores adipisci
      veritatis. Expedita exercitationem officia quos sint ullam minima
      consectetur iusto dignissimos fugiat nostrum. Tempore, modi atque porro
      debitis distinctio soluta dignissimos ducimus odit voluptatem? Omnis
      laudantium minus libero, sed excepturi magnam dolor. Quaerat quidem
      nostrum, cum veniam nobis ipsum eligendi nemo temporibus ea voluptas
      aliquid, asperiores cupiditate doloribus unde tenetur saepe perspiciatis
      alias adipisci reiciendis laborum non odit. Commodi doloremque tenetur
      aspernatur temporibus, saepe velit ipsum consectetur illo voluptatibus
      incidunt dolore nostrum? Incidunt hic enim eaque obcaecati doloremque
      blanditiis harum placeat natus eos pariatur culpa molestias iure neque
      quia eius ad rem vero aperiam, sed in esse accusamus fugiat magni
      praesentium. Nemo blanditiis dignissimos asperiores, ex voluptas esse
      fugit quod doloribus repellat recusandae odit! Harum excepturi neque modi
      hic quos, placeat inventore aliquid enim dolorem?
    </p>
    <div class="container">
       <parallax-image
      :imageUrl="'/building.jpg'"
      :intensity="0.1"
      :width="'50vw'"
      height="500px"
      :direction="'Vertical'"
      :transition="'transform 0.3s ease-out'"
    ></parallax-image>
    </div>
   <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus id inventore fugit natus porro quod earum. Praesentium ab et culpa, esse eligendi veniam dolores. Vel aliquid praesentium distinctio quam eius, saepe assumenda adipisci dolorum corporis at voluptas delectus doloremque quas fugiat molestiae nisi dolorem? Ut odio exercitationem labore ea ex sit doloribus adipisci ullam rem amet eos odit minus natus saepe blanditiis recusandae omnis, dolores asperiores reprehenderit magni quod earum repellendus! Explicabo perferendis vel officia omnis, minima, impedit, quisquam corporis quas tenetur illum perspiciatis! In, commodi veritatis voluptatum earum impedit expedita sint, fugiat ut accusamus iusto exercitationem facere repudiandae optio vero aspernatur officiis nulla natus iure, sunt sequi ipsa? Esse saepe iste tempora tenetur? Distinctio, hic, tenetur, optio assumenda maxime aliquid sint nemo iste voluptate reprehenderit aspernatur corrupti quas beatae? Non incidunt minima, itaque ex aperiam enim placeat, adipisci quasi facilis eum repudiandae ullam aut, consectetur quod sint. Quis rerum nisi ipsum voluptates unde sequi obcaecati, ipsam pariatur repellendus cumque voluptatem delectus dolorum cupiditate praesentium ratione eum expedita amet beatae quidem possimus tenetur fuga provident distinctio illo? Sunt voluptatem magni commodi soluta libero dolorem magnam similique aut deserunt ex quod, blanditiis eligendi, ipsa necessitatibus consequuntur quasi porro. Excepturi, commodi vel.</p>
  </div>
</template>

<script>
import ParallaxImage from "./components/parallaxImage.vue";

export default {
  name: "App",
  components: {
    ParallaxImage,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100vw;
}
h6{margin: 0;}
</style>

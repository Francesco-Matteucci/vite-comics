<script>
export default {
  data() {
    return {
      name: 'AppMain',
      curiosities: [
        "In origine Superman non poteva volare. Nel primo albo a fumetto del 1938 il supereroe in compenso poteva fare dei salti molto potenti arrivando ad altezze incredibili.",
        "Nel 2018 Wonder Woman è stato il film di origine di supereroi con il più alto incasso, è stato anche il film della prima guerra mondiale con i guadagni più alti.",
        "Joaquin Phoenix ha basato la sua risata nel film 'Joker' su persone che avevano davvero un disturbo patologico di risate.",
        "Il nome Bruce Wayne, l'alter-ego di Batman, deriva dall'unione di due personaggi storici: Re Bruce I di Scozia e Anthony 'Mad' Wayne, un eroe della rivoluzione americana.",
        "Nel 2008, il sindaco della città di Batman, in Turchia, ha fatto causa a Christopher Nolan e alla Warner per aver usato il nome della sua città senza chiedere il permesso.",
        "Bruce Wayne, comunemente conosciuto come Batman, possiede il Daily Planet, la testata giornalistica dove lavora Clark Kent, cioè Superman.",
        "La DC e la Marvel hanno realizzato un crossover nel quale Hulk viene sconfitto da Batman.",
        "Nel 1996 DC e Marvel hanno prodotto una serie crossover dove Wolverine e Batman sono un unico personaggio di nome Dark Claw."
      ],
      selectedCuriosity: ''
    };
  },
  methods: {
    generateCuriosity() {
      const randomIndex = Math.floor(Math.random() * this.curiosities.length);
      this.selectedCuriosity = this.curiosities[randomIndex];
    }
  }
};
</script>

<template>
   <main>
    <div class="content container">
      <button class="btn my-3" @click="generateCuriosity">
        Curiosità su DC
      </button>
        <p class="curiosity-text mt-4" v-if="selectedCuriosity">{{ selectedCuriosity }}</p>
    </div>
  </main>
</template>
  
<style scoped lang="scss">
@use '../../style/_variables.scss' as variables;

main {
  padding: 10px;
  background-color: variables.$footer-background-color;
  color: variables.$background-color;
  text-align: center;
}

.content {
  font-size: 20px;
  button {
    border-color: variables.$primary-color;
    color: variables.$title-color;
    transition: background-color 0.3s ease, transform 0.3s ease;

    &:hover {
      background-color: variables.$background-color;
      color: variables.$primary-color;
      transform: scale(1.05);
      box-shadow: 0px 4px 15px rgba(0, 123, 255, 0.6);
    }
  }
}

.curiosity-text {
  font-size: 18px;
  font-weight: bold;
  margin-top: variables.$margin-base;
  color: variables.$primary-color;
}

</style>
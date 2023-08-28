<script>
export default {
  name: "resas",
  data() {
    return {
      date: null,
      heure: "",
      tableauHoraires: [],
      horairechoisi: "",
    };
  },
  methods: {
    viewDate() {
      console.log(this.date);
      const creneau = new Date(this.date);
      console.log(creneau);
      creneau.setHours(18, 0);
      console.log(creneau);

      this.tableauHoraires.push(creneau);
      console.log(this.tableauHoraires);

      //   let i = 18;
      //   let j = 0;
      //   do {
      //     creneau.setHours(i, j);
      //     if (i === 18) {
      //       j = 30;
      //     } else if (j === 30) {
      //       i += 1;
      //       j = 0;
      //     } else if (j === 0) {
      //       j = 30;
      //     }
      //     this.tableauHoraires.push(creneau);
      //   } while (i < 24);
      //   console.log(this.tableauHoraires);
      let newcreneau = new Date();
      do {
        const last = this.tableauHoraires[this.tableauHoraires.length - 1];
        console.log(last);
        let minutes = last.getMinutes();
        console.log(minutes);
        minutes += 30;
        newcreneau = new Date(last);
        newcreneau.setMinutes(minutes);
        console.log(newcreneau);
        this.tableauHoraires.push(newcreneau);
      } while (newcreneau.getHours() !== 23);
      console.log(this.tableauHoraires);
    },

    formatTime(dateTime) {
      const hours = dateTime.getHours().toString().padStart(2, "0");
      const minutes = dateTime.getMinutes().toString().padStart(2, "0");
      return `${hours}:${minutes}`;
    },
    viewHour(horaire) {
      this.horairechoisi = horaire;
      console.log(`horaire choisi : ${this.horairechoisi}`);
      //   return this.horairechoisi;
    },
  },
};
</script>

<template>
  <div class="maxhigh">
    <div>
      <div>
        <p>Dans quel restaurant souhaitez vous réserver ?</p>
        <select v-model="selected">
          <option disabled value=""></option>
          <option>Lille</option>
          <option>Rouen</option>
        </select>
        <p>Votre restaurant : {{ selected }}</p>
      </div>

      <input type="date" v-model="date" class="btn-horaire" />
      <div @click="viewDate" class="btn-horaire">voir la date choisie</div>
      <!-- <p>la date de votre réservation : {{ date }}</p> -->
    </div>
    <div class="englobeur-btn-horaire">
      <!-- <input type="time" v-model="heure" /> -->
      <div class="btn-horaire" v-for="item in tableauHoraires">
        <span @click="viewHour(item)">{{ formatTime(item) }}</span>
      </div>
    </div>
    <p>
      Voulez-vous bien reserver une table le {{ date }} à {{ horairechoisi }} ?
    </p>
  </div>
</template>

<style>
.btn-horaire {
  background-color: #faf5d0;
  width: fit-content;
  padding: 0.5rem;
  border-radius: 0.5rem;
  margin: 0.5rem;
}
.btn-horaire:hover {
  background-color: #d3ce9d;
  cursor: pointer;
}
.englobeur-btn-horaire {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
.maxhigh {
  position: relative;
  height: 100%;
  box-sizing: border-box;
}
</style>